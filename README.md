​Quick Start

  


Machbase is the fastest time seriesDBMSforIoT&BigData. WithMachbase, you can load 1 million data and retrieve them with SQL in a few seconds. 

Here is how to installMachbase, insert and retrieve data.

  


**List of Contents**

* [Setup System Environment](http://doc.machbase.com/quick-start#Setup System Environment)
* [Package Installation](http://doc.machbase.com/quick-start#Package Installation)

* [Insert Data    ](http://doc.machbase.com/quick-start#Insert Data)
* [Retrieve Data](http://doc.machbase.com/quick-start#Select Data)

  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Set-up System Environment

  


Machbasecan access several files at the same time. Thus, it is required to release limitations on the number of files that can be accessed.

If you want to remove the limits manually, refer to[Operating System Settings](http://doc.machbase.com/quick-start#).

  


The predefined shell file is ready for quick installation. Simply run the shell file below and then, it will automatically set your system.

curl http://www.machbase.com/dist/reduce\_limit.sh \| 

sudo

 sh

  


When you issue the command above, it modifies "/cd .etc/security/limits.conf" file and reboots at the same time.

If it cannot stop with CTRL+C within 30 seconds, the reboot process will start. The settings of limitation will be applied after the reboot.

ulimit

 -Sn

  


You can check values of limitation by running the command above.

  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Package Installation

  


DownloadMachbase package from download page and run the command.

Machbasesupports RPM forCentOS,Redhatand DEB for Debianlinux. Instructions and details are in below. 

  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Installing RPM

  


[Install from rpm packages](http://doc.machbase.com/quick-start#)for detailed information. To download the package and install, run the commands below.

wget

 http://www.machbase.com/dist/machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.rpm

  


sudo

 yum install machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.rpm

If it is installed, it automatically tries to executeMachbase.

  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Installing DEB

  


[Install from deb packages](http://doc.machbase.com/quick-start#)for detailed information. To download the package and install, run the commands below.

wget

 http://www.machbase.com/dist/machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.deb

  


sudo

dpkg

 -i machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.deb

If it is installed,Machbaseare automatically executed. 

  


  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Insert Data

  


For sample data, we use a sample\_data.csv file located in the /home/machbase/machbase\_home/tutorials/csvload. 1,000,000 records are ready for use.

The content of sample\_data.csv file looks like below.

2015-05-20 06:00:00,63.214.191.124,2296,122.195.164.32,5416,12,GET /

twiki

/bin/view/Main/

TWikiGroups

?rev=1.2 HTTP/1.1,200,5162

  


2015-05-20 06:00:07,212.237.153.79,6203,71.129.68.118,8859,67,GET /

twiki

/bin/view/Main/

WebChanges

HTTP/1.1,200,40520

  


2015-05-20 06:00:07,243.9.49.80,344,122.195.164.32,6203,46,GET /

twiki

/bin/view/Main/

TWikiGroups

?rev=1.2 HTTP/1.1,200,5162

  


2015-05-20 06:00:07,232.191.241.129,5377,174.47.129.59,1247,17,GET /mailman/

listinfo

/

hsdivision

HTTP/1.1,200,6291

  


2015-05-20 06:00:07,121.67.24.216,2296,212.237.153.79,6889,68,GET /

twiki

/bin/view/

TWiki

/

WebTopicEditTemplate

HTTP/1.1,200,3732

  


2015-05-20 06:00:07,31.224.72.52,450,100.46.183.122,10541,20,GET /

twiki

/bin/view/Main/

WebChanges

HTTP/1.1,200,40520

  


2015-05-20 06:00:07,210.174.159.227,6180,173.149.119.202,6927,2,GET /

twiki

/bin/

rdiff

/

TWiki

/

AlWilliams

?

rev1

=1.2

&

rev2

=1.1 HTTP/1.1,200,5234

  


2015-05-20 06:00:07,210.174.159.227,10124,16.194.51.72,10512,69,GET /

twiki

/bin/

rdiff

/

TWiki

/

AlWilliams

?

rev1

=1.2

&

rev2

=1.1 HTTP/1.1,200,5234

  


2015-05-20 06:00:07,60.48.99.15,12333,85.183.139.166,12020,64,GET /robots.txt HTTP/1.1,200,68

  


2015-05-20 06:00:07,81.227.25.139,5883,96.128.212.177,2042,56,GET /

twiki

/bin/oops/

TWiki

/

TextFormattingRules

?template=

oopsmore

¶m1=1.37¶m2=1.37 HTTP/1.1,200,11400

  


2015-05-20 06:00:07,166.218.230.17,6203,174.47.129.59,2277,53,GET /

twiki

/bin/view/Main/

LondonOffice

HTTP/1.0,200,3860

  


2015-05-20 06:00:07,71.129.68.118,3648,20.137.26.161,11321,68,GET /

twiki

/bin/view/Main/

TokyoOffice

HTTP/1.1,200,3853

  


2015-05-20 06:00:07,227.106.13.91,266,5.238.208.30,2997,69,GET /

twiki

/bin/view/

TWiki

/

WikiSyntax

HTTP/1.1,200,7352

  


  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Create a table

  


To create a table, you need to design CREATE TABLE statement according to data. For more information, please refer to [Data Types](http://doc.machbase.com/quick-start#) and [Table](http://doc.machbase.com/quick-start#).

```
CREATE TABLE sample_data
( 
  dt        
DATETIME
,
  
srcip
IPV4
, 
  
srcport
   INTEGER, 
  
dstip
IPV4
, 
  
dstport
   INTEGER, 
  protocol  SHORT, 
  
eventlog
VARCHAR
(1024), 
  
eventcode
 SHORT, 
  
eventsize
 LONG
);
```

  


runmachsqland execute CREATE TABLE statement like below.  

```
[mach@
localhost
 ~]$ 
machsql
 -s 
localhost
 -u sys -p manager

=================================================================
    
Machbase
 Client Query Utility
    Release Version 
3.5.0.826b8f2.official
    
    Copyright 
2014
, 
Machbase
 Corporation or its subsidiaries.
    All Rights Reserved.
=================================================================

MACHBASE
_CONNECT_MODE=
INET
, PORT=
5656
Type 'help' to display a list of available commands. 

Mach
>
CREATE TABLE sample_data(dt 
DATETIME
, 
srcip
IPV4
, 
srcport
 INTEGER, 
dstip
IPV4
, 
dstport
 INTEGER, 
             protocol SHORT, 
eventlog
VARCHAR
(1024), 
eventcode
 SHORT, 
eventsize
 LONG);
Created successfully.
Mach
>
 quit
```

###  

![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Load data

  


Now it is ready to insert data and usecsvimporttool like below.

It takes 2.44 seconds to load 1M data and loads 409,836 records per second.

```
[Mach@
localhost
 ~]$ cd $
MACHBASE
_HOME/tutorials/
csvload

[Mach@
localhost
 ~]$ 
csvimport
 -t sample_data -d sample_data.csv -F "dt 
YYYY-MM-DD
HH24
:MI:SS"
-----------------------------------------------------------------
     
Machbase
 Data Import/Export Utility.
     Release Version 3.5.0.826b8f2.official
     Copyright 2014, 
InfiniFlux
 Corporation or its subsidiaries.
     All Rights Reserved.
-----------------------------------------------------------------

NLS
            : 
US7ASCII
            EXECUTE MODE   : IMPORT
TARGET TABLE   : sample_data
DATA FILE      : sample_data.csv
IMPORT_MODE    : APPEND              FILED TERM     : ,
ROW TERM       : \n                  ENCLOSURE      : "
ARRIVAL_TIME   : FALSE               ENCODING       : NONE
HEADER         : FALSE               CREATE TABLE   : FALSE
                                  1000000 records imported,    0 errors 
occured

Import time         :  0 hour  0 min  2.44 sec
Load success count  : 1000000
Load fail count     : 0
```

  


  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Retrieve Data

  


To retrieve data fromMachbase, executemachsqlinlinuxshell and use SQL what you want to.

  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Get total data count

  


  


```
​[mach@
localhost
 ~]$  
machsql
 -s 
localhost
 -u sys -p manager
=================================================================
     
Machbase
 Client Query Utility
     Release Version 3.5.0.826b8f2.official
     Copyright 2014, 
InfiniFlux
 Corporation or its subsidiaries.
     All Rights Reserved.
=================================================================
 
MACHBASE
_CONNECT_MODE=
INET
, PORT=5656
 Type 'help' to display a list of available commands.
Mach
>
 SELECT COUNT(*) FROM SAMPLE_DATA;
 COUNT(*)
 -----------------------
 1000000
 [1] row(s) selected.
 Elapsed time: 0.000
```

  


![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Get count by connection

  


It checks the number of connections, sum and averageeventsize between source IP and destination IP.

When you execute the command below, too many results are displayed.  Here we are displaying only top 10 based on the sum here as shown below.

  


```

Mach
>
 SELECT 
SRCIP
, 
DSTIP
, COUNT(*) as COUNT, SUM(
EVENTSIZE
) as SUM, AVG(
EVENTSIZE
) as AVG FROM SAMPLE_DATA GROUP BY 
SRCIP
, 
DSTIP
 ORDER BY SUM DESC LIMIT 10;
 
SRCIP
DSTIP
           COUNT                SUM                  AVG
 ------------------------------------------------------------------------------------------------------------
 86.45.186.17    121.67.24.216   205                  2598899              12677.6
 96.128.212.177  16.0.123.104    190                  2541955              13378.7
 16.194.51.72    7.234.88.67     199                  2529420              12710.7
 115.18.128.171  96.128.212.177  203                  2512405              12376.4
 161.28.150.105  98.25.97.158    206                  2504865              12159.5
 129.55.140.243  212.237.153.79  202                  2495157              12352.3
 115.18.128.171  239.81.105.222  221                  2481104              11226.7
 245.13.24.17    115.18.128.171  214                  2478371              11581.2
 185.22.195.164  96.128.212.177  209                  2465601              11797.1
 5.114.66.53     122.195.164.32  229                  2465099              10764.6
 [10] row(s) selected.
 Elapsed time: 0.901
 Mach
>
 quit

```

  


For more information aboutMachbase, please refer to the "[Get Started](http://doc.machbase.com/quick-start#)" page.

