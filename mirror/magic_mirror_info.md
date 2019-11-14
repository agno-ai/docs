# Basic commands to start & stop mirror
### References
https://github.com/MichMich/MagicMirror/wiki/Auto-Starting-MagicMirror

## Definitions 
PM2 is a production process manager for Node.js applications with a built-in load balancer. <br>
It allows you to keep applications alive forever, to reload them without downtime and to facilitate common system admin tasks. <br>
In this case we will use it to keep a shell script running.

## Start Magic Mirror
execute: ```$ magic_mirror_start.sh```

## Exit Magic Mirror 
1. Press Ctrl-q
2. Then type following command in terminal (otherwise magic mirror will restart after a couple of seconds)
3. ```$ pm2 stop MagicMirror```, or (via ssh) ```$ stopmagic```

## Miscellaneous
### Restarting your MagicMirror
    ```$ pm2 restart mm```
### Stopping your MagicMirror
    ```$ pm2 stop mm```
### Show the MagicMirror logs
    ```$ pm2 logs mm```
### Show the MagicMirror process information
    ```$ pm2 show mm```


## Configuration
Configuration file can be found as under ```/home/pi/MagicMirror/config/config.js```

