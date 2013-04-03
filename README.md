### GMF. Go Media Framework. 

Original project, hosted here (https://code.google.com/p/gmf) looks abandoned.
This is a patched version that compiles against Go 1.0.3 and ffmpeg-0.8.

This is "AS IS" version, i was able to compile it, but there is a lot of questions and TODOs.

#### Installation

The installation is pretty straightforward. Just define the ffmpeg include path.
```
export CGO_LDFLAGS="-L$FFMPEG_ROOT/lib/ -lavcodec -lavformat -lavutil -lswscale"
export CGO_CFLAGS="-I$FFMPEG_ROOT/include"

go get github.com/3d0c/gmf
```

