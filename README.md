# FFmpeg Latest Autobuilds for Windows

![Build FFmpeg on push](https://github.com/Citrinae-Lime/ffmpeg-autobuild/workflows/Build%20FFmpeg%20on%20push/badge.svg)
![Build FFmpeg on pull request](https://github.com/AnimMouse/ffmpeg-autobuild/workflows/Build%20FFmpeg%20on%20pull%20request/badge.svg)

[FFmpeg](https://ffmpeg.org/) latest nonfree git/snapshot/development/master/nightly builds with additional libraries/dependencies.

[Downloads](https://github.com/Citrinae-Lime/ffmpeg-autobuild/releases)

#### Schedule

Release builds: Weekly or Every time [ffmpeg-windows-build-helpers](https://github.com/rdp/ffmpeg-windows-build-helpers) updates or I updated the repository.

#### Release Retention Policy
Release builds are kept for two years.\
Last 1 pre-release build are kept every time a release build are released.

ffmpeg, ffprobe, and ffplay are included.

Nonfree builds with Fraunhofer FDK AAC (libfdk_aac).

All builds are static.

Powered by [ffmpeg-windows-build-helpers](https://github.com/rdp/ffmpeg-windows-build-helpers) script to cross compile for Windows on Linux.

Uses [GitHub Actions](https://github.com/features/actions) to automatically compile FFmpeg.

Uses [Dependabot](https://dependabot.com/) to automatically update submodules.

For latest bug fixes, new improvements, cutting edge, use git/snapshot/development/master/nightly builds.

For stable release builds for Windows, goto [ffmpeg-stable-autobuild](https://github.com/AnimMouse/ffmpeg-stable-autobuild)

For other builds of FFmpeg built by others, goto [List of FFmpeg Binaries](https://www.animmouse.com/p/ffmpeg-binaries/).

### Configuration
```
    --pkg-config=pkg-config
    --pkg-config-flags=--static
    --enable-version3
    --disable-debug
    --disable-w32threads
    --arch=x86_64
    --enable-libcaca
    --enable-gray
    --enable-libtesseract
    --enable-fontconfig
    --enable-gmp
    --enable-libass
    --enable-libbluray
    --enable-libbs2b
    --enable-libfreetype
    --enable-libfribidi
    --enable-libgme
    --enable-libgsm
    --enable-libilbc
    --enable-libmp3lame
    --enable-libopus
    --disable-encoder=opus
    --enable-libsnappy
    --enable-libsoxr
    --enable-libspeex
    --enable-libtheora
    --enable-libvorbis
    --disable-encoder=vorbis
    --enable-libwebp
    --enable-libzimg
    --enable-libopenjpeg
    --enable-libopenh264
    --enable-libsrt
    --enable-libxml2
    --enable-opengl
    --enable-libdav1d
    --enable-cuda-llvm
    --enable-gnutls
    --enable-libvpx
    --enable-libaom
    --extra-libs=-lharfbuzz
    --extra-libs=-lm
    --extra-libs=-lshlwapi
    --extra-libs=-lmpg123
    --extra-libs=-lpthread
    --extra-cflags=-DLIBTWOLAME_STATIC
    --extra-cflags=-DMODPLUG_STATIC
    --extra-cflags=-DCACA_STATIC
    --disable-amf
    --enable-libmfx
    --enable-gpl
    --enable-frei0r
    --enable-libx264
    --enable-libx265
    --enable-libxvid
    --enable-libdavs2
    --enable-libxavs2
    --enable-libxavs
    --extra-cflags='-march=core2'
    --extra-cflags=-O2
    --enable-static
    --disable-shared
    --enable-nonfree
    --enable-libfdk-aac
```