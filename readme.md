# TT Backup
My personal script to back up TT servers on Linux.

## Notes
* The directory /home/tt/*.xml (by default) is where the script assumes your TeamTalk server configuration files are stored, as that is my setup. I use [Doug Lee and Daniel Nash's TT script](https://www.dlee.org/teamtalk/tt) for my TeamTalk server manager of choice.

* Currently it only backs up XML files. If you would like it to back up everything, remove the "/*.xml" from the script.

* Note: You will have to run this in a cronjob (see below).

## Running in a Cronjob
The following line (added to your crontab with `crontab -e`) will run the script at 03:00 daily, and assumes you are running at ./tt-backup/tt-backup.sh:
```
0 3 * * * ./tt-backup/tt-backup.sh
```


## Contributions
Improvements are always welcome; please open an issue or send in a PR!

Enjoy!
