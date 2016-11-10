# Currently Under Construction
## winCron
Crontab for windows

A Windows crontab.py program analogue to linux crontab utility

winCron supports all timing-arguments that Linux crontab supports, like:
* * for every every minute,hour,month,day of month,day of week
* comma (,) seperated arguments like 11,12,13 for 11th,12th,13th (minute,hour,mon,dom)
* hyphen (-) seperated argument to specify a range like 12-16 for running jobs between 12:00 and 16:59
* empty lines or lines starting with # are ignored
* @yearly	(0 0 1 1 *), @daily	(0 0 * * *), @hourly	(0 * * * *) and reboot (run at startup) are currently not supported

**Sample crontab.txt**

see crontab.txt 

## Install winCron

* download winCron.py
* create crontab.txt

## Running winCron

* Open CMD box
* python winCron.py [crontab.txt [crontab.log [crontab.pid]]]
* all files are supposed to be in the same folder

The defaults are crontab.txt,crontab.log,crontab.pid



