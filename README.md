# Audiobooks

Getting audiobooks on youtube music.

1. Download the clips from <http://audiobookbay.ws/>

2. Split the clips into chunks smaller than 300MB

```bash
# 21600 seconds = 6h
ffmpeg -i 'Emily Nagoski - Come as You Are The Surprising New Science That Will Transform Your Sex Life.mp3' -f segment -segment_time 21600 -c copy come_as_you_are%03d.mp3
```

3. upload them to youtube music: your profile > upload music
