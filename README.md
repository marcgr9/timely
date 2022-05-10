# timely

mac command line utility to limit the amount of time an executable can be kept open. it's mac-only just because of the alerts that use applescript

main idea is that after x minutes of working on something your productivity decreases a lot if you don't take a break

this utility automatically closes any application after the amount of time you specified


# build
give exec permission to ```build/build``` and run it

it will install all the necessary config in ```/usr/local/etc/timely``` and the executable in ```/usr/local/bin/timely```


# usage
```timely add [executable]``` - adds executable to list of restricted apps
  
```timely remove [full path to executable]``` - removes all restrictions for the given app

```timely list``` - get full path of all restricted apps

```timely set {time | extra} [value]``` - change preferences

```timely preferences``` - view current config values
      
# config

config file is ```/usr/local/etc/timely/.preferences```

* time - the amount of minutes the app will be kept open

* extra - the amount of minutes the app will be kept open after you were notified that it'll close soon

# todo

- [x] ```timely set (time | extra) value``` - change settings by commands
- [ ] keep a list of currently running timelies
- [ ] check the time remaining of a particular timely
- [ ] gui ??? maybe not

# bugs
1. ~~adding an executable by providing a full path usually doesn't work~~
