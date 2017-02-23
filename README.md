# BIAMI-DEV2EE
Easy way to migrate your BIAMI DEV to EE (for testing, pre-prod and production purposes)

Requirements:
Linux or Unix

Paramteres:
- tomcat

  Specify BIAMI EE tomcat folder
  
  Example 1 (local): "/var/www/html/"
  
  Example 2 (remote with ssh keys set up previously): "username@remote_host:/var/www/html/"

Google Spreadsheet Script: https://docs.google.com/spreadsheets/d/1Z4aUeo7n2TUn4LoRizqnXu74snJsRNp_ivUugTmTMW0/edit?usp=sharing

Import to BIAMI DEV: 
Download import.tsv file into temp directory and run ./core_run.sh --context_param cmd=import or import it directly from Google Spreadsheet:  ./core_run.sh --context_param cmd=import --context_param script="https://docs.google.com/spreadsheets/d/1Z4aUeo7n2TUn4LoRizqnXu74snJsRNp_ivUugTmTMW0/export?gid=0&format=tsv"
