# computing_notes

## make movie from image files
`ffmpeg -r 30 -i img_%05d.tiff -vcodec libx264 -vb 2.5M -vf "crop=1300:1300:1800:1000, scale=650:650" movie.mpg`
- note: -i does not accept img_*.tiff or similar
- -r 30, set framerate
- -vcodec libx264, codec to use
- -vb 2.5M, bitrate of output file (controls quality)
