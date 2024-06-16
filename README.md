# What's this?
This is simple ARM emulator called uARM, implemented by Dmitry Grinberg.
(http://dmitry.gr/index.php?r=05.Projects&proj=07.%20Linux%20on%208bit)

# How to compile

## get codes

```
$ git clone https://github.com/syuu1228/uARM.git
```

## compile

just run make.

```
$ make
```
Or, if your system installed BSD make, you'll need to run GNU make like this:
```
$ gmake
```

You will get ./uARM as an executable binary.

## uncompress image

```
$ bzcat jaunty.rel.v2.bz2 > jaunty.rel.v2
```

## boot linux up.

```
$ ./uARM jaunty.rel.v2
```

You will get shell prompt after 10 second.

## enjoy in the sandbox.

You can terminate by using ```killall uARM``` on terminal.
I don't know how to shutdown safely.

## removed files  
* jaunty.rel.v2.bz2  
* jaunty.rel.v2  
* .o  
* uARM  
* uARM.hex  
* zImage  

## TODO  
* weibo  
```
我把syuu1228/uARM跑通了（一个ARM模拟器，但不是uclinux），
在ubuntu14下运行效果如下——不过因为太多arm模拟器了，
这个又不是uclinux，所以没兴趣，可能以后再研究，
这个应该比较轻量级，跑linux 2.6
```
* original: https://github.com/syuu1228/uARM  
* How to build zImage and get jaunty.rel.v2 ?  
