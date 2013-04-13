OMXPlayer-Sync
==============

OMXPlayer-Sync facilitates synchronization of multiple OMXPlayer 
instances over the network in a master/slave fashion.

Usage
-----

```
$ ./omxplayer-sync -h
Usage: omxplayer-sync [options] filename

Options:
  -h, --help            show this help message and exit
  -m, --master          
  -l, --slave           
  -x DESTINATION, --destination=DESTINATION
  -u, --loop            
  -v, --verbose
```

**master**

```
omxplayer -v -m -x 255.255.255.255 movie.mp4
```

**slave**

```
omxplayer -v -l movie.mp4
```


Settings
--------

```
OMXPLAYER = 'omxplayer'
PORT = 1666
TOLERANCE = 0.2
ADJUST_OMXPLAYER = -0.1
ADJUST_MASTER = 0.1
ADJUST_SLAVE = 0.3
SKIP_SIZE = 5
```
