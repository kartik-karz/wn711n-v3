This is a driver for TP-link WN722N wireless adapter v3

I had tried all the drivers that was provided and I wasn't able to get it working
in the latest linux kernels for Kali Linux and thus I had to port out the older
code taken from the Tp link website and get it working for my system.

I just thought others who were in similar position might find it helpful
and thus am uploading it.

CAUTION:
This was ported by a sleep deprived idiot who just wanted monitor mode to
work as fast as possible and thus I leave it up to you to how many
programming conventions I might have broken.

If you still want to proceed then

```
1.make clean
2.make
3.make install   // This should few files including the .ko file

// if make install fails for some reason then you can do this
insmod ./8188eu.ko
```

