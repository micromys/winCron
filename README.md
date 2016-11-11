# Currently Under Construction
## crontab.py
Crontab for windows

A Windows crontab.py program analogue to linux crontab utility

crontab.py supports all timing-arguments that Linux crontab supports, like:
* * for every every minute,hour,month,day of month,day of week
* comma (,) seperated arguments like 11,12,13 for 11th,12th,13th (minute,hour,mon,dom)
* hyphen (-) seperated argument to specify a range like 12-16 for running jobs between 12:00 and 16:59
* empty lines or lines starting with # are ignored
* **@yearly, @daily, @hourly** are supported but internally converted to 0 0 1 1 *,0 0 * * *,0 * * * *
* @reboot (run at startup) is currently not supported

**Sample crontab.txt**

## see crontab.txt 

## Install crontab.py

* download crontab.py
* create crontab.txt or download crontab.txt and adapt it

## Running crontab.py

* Open CMD box
* python crontab.py [crontab.txt [crontab.log [crontab.pid]]]
* all files are supposed to be in the same folder
* create shortcut on your desktop with: 
  * target: C:\Python27\python.exe crontab.py crontab.txt crontab.log crontab.pid
  * start in: "C:\Users\your name\Desktop"
  * Run: Minimised
  * optionally you can put the shortcut in the startup folder (C:\Users\yourname\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup) to start crontab.py it on startup

The defaults are crontab.txt,crontab.log,crontab.pid

## Running crontab.py as a Service

### Under construction

