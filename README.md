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

start.(developer 1)
```
git flow init
git pusg origin master
```

clone all files without build new folder(developer 2)
```
git clone git@git.com:rengokantai.git .
git checkout develop
git flow feature start
git flow init
git flow feature start branchname
git flow feature publish branchname   //push branch
```

checkout from repo(develooper 3)
```
git flow feature track branchname
git add,commit...
git push (if same branch)
```

close a branch
```
git flow finish branchname
```

create release
```
git flow release start sprint1-release
```

other people can start working base on this release
```
git flow release track sprint1-release
```

finish:
```
git flow release finish sprint1-release
git push --tags
```

developer: create a hotfix
```
git flow hotfix start issuename
git commit.
git flow hotfix finish issuename //type your message
git checkout master
git push --all origin
```


other possible commands:
```
git flow hotfix publish
git flow hotfix track
```

