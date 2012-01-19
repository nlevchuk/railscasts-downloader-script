# Railscasts downloader script (only FREE videos)

##Description

**railscasts_downloader** is a script for lightweight download, display names and descriptions episode(s) from Railscasts.com (only FREE content). Written on Ruby for linux and MacOS.

##Instalation

 Clone git repository:
 -> git clone <git_repos>

 Change directory:
 -> cd <git_repos>

 Run bundler:
 -> bundle install

 Then move railscasts script to directory where you want to contain download episodes. You can move it to directory that exist other episodes and download the missing one.

##Dependencies

- ruby(1.8.7 and higher);
- rubygems (gem nokogiri, open-uri, timeout);
- curl;

##Usage

 Run in terminal: **./railscasts-downloader <command> [[OPTION] <number of episodes>] [<episode(s)>] [--with-desc]**

Command:

- **-s** : show name of episode(s)
- **-d** : download episode(s)

Option:

- **first/last <count>** : show or download first/last <count> episode(s)
- **all** 		 		 : download all(missed) episode(s)
- **--with-desc** 		 : display description selected episode(s) (only -s command)

##Examples

  '-s first 5'        - show first 5 eposides
  '-d 137',           - download only 137 episode
  '-d 4-8',           - download from 4 to 8 episodes
  '-d last 3'         - download last 3 episodes
  '-s 5 --with-desc'  - show episode number 5 with description
  '-d all'			  - download all(missing) episodes
