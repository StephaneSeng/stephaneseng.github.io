# stephaneseng.github.io

## Local installation notes

Versions:

```
$ ruby --version
ruby 3.1.3p185 (2022-11-24 revision 1a6b16756e) [x86_64-linux]

$ jekyll --version
jekyll 4.3.1
```

Build and run:

```console
$ bundle exec jekyll serve
```

Generate a GIF from Unity recordings:

```console
$ ffmpeg -i image_001_%04d.png -vf palettegen palette.png
$ ffmpeg -i image_001_%04d.png -i palette.png -lavfi paletteuse capture.gif
```
