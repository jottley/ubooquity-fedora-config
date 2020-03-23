# Ubooquity Config for Fedora

This are the config files I'm using for my [Ubooquity](https://vaemendis.net/ubooquity/) server. The shell script for starting and stopping the server is based on the [run-ubooquiity.sh](http://vaemendis.net/ubooquity/downloads/scripts/) script.

The modifications I've made are to point to the locations I have the jar file, add remoteadmin, and set where I want the data and log files written.  I've also added a servive file so that the ubooquity server can be started and stopped as part of the system on reboot.

My file layout is
```
.
├── etc
│   ├── systemd
│   │   └── system
│   │       └── ubooquity.service
│   └── ubooquity
│       └── ubooquity.sh
├── srv
│   └── ubooquity
│       └── Ubooquity.jar
└── var
    ├── log
    │   └── ubooquity.log
    └── local
        └── ubooquity
            └── <ubooquity data files>
```