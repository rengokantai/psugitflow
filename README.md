#### psugitflow

install on windows:  
First, copy getopt.ext into git/bin.  
[install getopt.exe](http://gnuwin32.sourceforge.net/downlinks/util-linux-ng-dep-zip.php)
[install dll libintl](http://gnuwin32.sourceforge.net/downlinks/libintl-dep-zip.php)
[install dll libintl](http://gnuwin32.sourceforge.net/downlinks/libiconv-dep-zip.php)
```
git clone --recursive git://github.com/nvie/gitflow.git
cd gitflow
contrib\msysgit-install.cmd "C:\Program Files (x86)\Git"
```

start.
```
git flow init
```
