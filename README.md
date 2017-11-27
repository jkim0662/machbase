# ​Quick Start {#quick-start}

Machbase is the fastest time series DBMS for IoT & BigData. With Machbase, you can load 1 million data and retrieve them with SQL in a few seconds.

Here is how to install Machbase, insert and retrieve data.

**List of Contents**

* [Setup System Environment](http://doc.machbase.com/quick-start#Setup System Environment)
* [Package Installation](http://doc.machbase.com/quick-start#Package Installation)
* [Insert Data    ](http://doc.machbase.com/quick-start#Insert Data)
* [Retrieve Data](http://doc.machbase.com/quick-start#Select Data)

### ![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Set-up System Environment

Machbasecan access several files at the same time. Thus, it is required to release limitations on the number of files that can be accessed.

If you want to remove the limits manually, refer to[Operating System Settings](http://doc.machbase.com/quick-start#).

The predefined shell file is ready for quick installation. Simply run the shell file below and then, it will automatically set your system.

`curl http://www.machbase.com/dist/reduce_limit.sh | sudo sh`

When you issue the command above, it modifies "/cd .etc/security/limits.conf" file and reboots at the same time.

If it cannot stop with CTRL+C within 30 seconds, the reboot process will start. The settings of limitation will be applied after the reboot.

`ulimit -Sn`

You can check values of limitation by running the command above.

### ![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Package Installation

DownloadMachbase package from download page and run the command.

Machbasesupports RPM forCentOS,Redhatand DEB for Debianlinux. Instructions and details are in below.

#### ![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Installing RPM

[Install from rpm packages](http://doc.machbase.com/quick-start#) for detailed information. To download the package and install, run the commands below.

`wget  http://www.machbase.com/dist/machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.rpm`

`sudo  yum install machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.rpm`

If it is installed, it automatically tries to execute Machbase.

#### ![](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw== "Anchor")Installing DEB

[Install from deb packages](http://doc.machbase.com/quick-start#)for detailed information. To download the package and install, run the commands below.

`wget`[`http://www.machbase.com/dist/machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.deb`](http://www.machbase.com/dist/machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.deb)

`sudo dpkg -i machbase-std-3.5.0.826b8f2.official-LINUX-X86-64-release.deb`

If it is installed,Machbaseare automatically executed.

