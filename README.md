# FFmpeg Sample Commands

### Desaturate
Turn every colors off from video
```bash
ffmpeg -i input -vf hue=s=0 output
```

### Grayscale
```bash
ffmpeg -i input -vf format=gray output
```

### Something I'm trying to get VIVID effect from Lightroom
Note: use multiple filters with comma separation
Filters: https://ffmpeg.org/ffmpeg-filters.html

```bash
ffplay -i i11.jpg -vf "transpose=1,scale=1080:-1,eq=contrast=1.22:brightness=0:saturation=1.11,vibrance=+0.40"
```