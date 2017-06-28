PCSensor
========

PCSensor / TEMPer2 driver for linux

This is based on 
* PCSensor v. 1.0.1 by Juan Carlos Perez
* PCSensor / TEMPer2 driver for linux  by Peter Farsinsen (https://github.com/peterfarsinsen/pcsensor)


### Build
Clone
```
git clone https://github.com/timmson/pcsensor.git
```

#### Make
##### Requirements 
* [usb.h](http://libusb.org/)

```
cd pcsensor && autoconf && ./configure && make && sudo make install
```
 
 ### Usage
 ```
 sudo ./pcsensor -h

 pcsensor version 1.0.1
       Aviable options:
           -h help
           -v verbose
           -l[n] loop every 'n' seconds, default value is 5s
           -c output only in Celsius
           -f output only in Fahrenheit
           -a[n] increase or decrease temperature in 'n' degrees for device calibration
           -m output for mrtg integration
 ```
 
 #### Output
 ```
 sudo ./pcsensor -c

 2017/06/27 22:30:48
 Temperature (internal) 28.62C
 Temperature (external) -0.00C
 ```