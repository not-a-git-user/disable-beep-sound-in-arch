simply do 
```
sudo rmmod pcspkr
sudo rmmod snd_pcsp
```
don't worry if it gives the error snd_pcsp is not currently loaded

then to prevent the modules from loading the next boot cycle create ```
/etc/modprobe.d/nobeep.conf```
and add
```
blacklist pcspkr
blacklist snd_pcsp
```
