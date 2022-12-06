# Jabra Evolve 75 Headset

Needed pulseaudio-bluetooth bluez

```
sudo systemctl enable --now bluetooth

scan on
pair <MAC>
connect <MAC>
trust <MAC>
```

Couldn't get the headset mic to show up in the syncs, needed missing codecs
Clue:
https://www.reddit.com/r/Jabra/comments/toiuah/use_jabra_evolve_75_on_linux/

`paci gst-libav gst-plugins-{base,bad,good,ugly}`

This ended up making the mic available
