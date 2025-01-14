# VLC for Unity documentation

- [User documentation](#user-documentation)
- [Make a release](#make-a-release)
- [Platform support](#platform-spport)

## User documentation

Given that VLC for Unity is based on LibVLCSharp, it shares 99% of the same APIs which means the LibVLCSharp documentation applies. You can find it [here](https://code.videolan.org/videolan/LibVLCSharp/-/blob/3.x/docs/home.md).

A basic explanation of the demo scenes provided in the asset is detailed in the [documentation text file](..\Assets\VLCUnity\documentation.txt).

## Make a release
 
This is a list of things to check until the release is more automated. Though the "uploading to the store" step cannot be scripted currently.

- plugins.dat generation,
- avoid js files,
- trial ftp upload,
- check that editor and standalone demo scenes work,
- check final package size size (~50MB),

### Android

To be complete, the android asset for every ABIs needs:

- classes.jar (only one file for all arch)
- libc++_shared.so (per arch)
- libvlc.so (per arch)
- libVLCUnityPlugin.so (per arch)
- LibVLCSharp and related DLLs (one file for all platform and architectures)

## Platform support

Currently the only supported platforms are:

- Windows classic (win64, not UWP),
- Android (all ABIs).