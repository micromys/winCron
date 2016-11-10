# winCron
Crontab for windows

A Windows crontab.py program analogue to linux crontab utility

winCron supports all timing-arguments that Linux crontab supports, like:
* * for every every minute,hour,month,day of month,day of week
* comma (,) seperated arguments like 11,12,13 for 11th,12th,13th (minute,hour,mon,dom)
* hyphen (-) seperated argument to specify a range like 12-16 for running jobs between 12:00 and 16:59
* other arguments are currently not supported

Sample crontab.txt

m		h			dom		mon		dow		command

m		minute			0-59	*/2 every two minutes, 2,4,6: minute 2,4,6; 5-10: between 5th and 10th minute including

hour	hour			0-23	*/2 every two hours (00:00,02:00,...) ; 2,4,6: 02:00,04:00,06:00; 12-18: between 12:00 and 18:59

dom		day of month	1-31	*/3 every 3rd day (3,6,9,...); 11,18,24: day 12,18,18; 19-31: between day 19 and 31

mon		month			1-12	*/2 every even month (Feb,Apr,Jun,Aug,Oct,Dec); 4,6: April, June; 5-7: May,June and July	(1=Jan,...,12=Dec)

dow		day of week		0-6		*/2: every even day of the week (0,2,4,6); 0,3,6: Mon,Thu,Sun; 3-5: Thu,Fri,Sat				(0=Mon,...,6=Sun)

command							command windows can understand

m		h			dom		mon		dow		command

30 		10,13,16	*		*		*		"C:\Program Files\FreeFileSync\FreeFileSync.exe" "D:\Documenten\FreeFileSync\Sync_DS.ffs_batch"

00		11,15		*		*		*		"C:\Program Files\FreeFileSync\FreeFileSync.exe" "D:\Documenten\FreeFileSync\sync_d2n.ffs_batch"

00		17			*		*		*		"C:\Program Files\FreeFileSync\FreeFileSync.exe" "D:\Documenten\FreeFileSync\sync_pc.ffs_batch"

50		11,15		*		*		*		echo  "test"

