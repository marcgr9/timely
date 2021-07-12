# timely

unix/mac command line utility to limit the amount of time an executable can be kept open

main idea is that after x minutes of working on something your productivity decreases a lot if you don't take a break

this utility automatically closes any application after the amount of tinme you specified


# build
give exec permission to build/build and run it

it should install all the necessary files in /usr/local/


# usage
 > timely add [executable]
 
      adds executable to list of restricted apps
 > timely remove [full path to executable]
 
      removes all restrictions for the given app

 > timely list 
 
      get full path of all restricted apps
      
# config

config file is /usr/local/etc/timely/.preferences

time - the amount of minutes the app will be kept open

extra - the amount of minutes the app will be kept open after you were notified that it'll close soon

path - path to config folder
