To build BitSafe you'll need a workin Debian Wheezy installation on a i386 or x64 architecture.

First, make sure that you have the needed tools:

# aptitude install live-build gettext

you can then edit bitsafe.build.conf and bitsafe.live.conf in the root directory.
These are the files with the most relevant configuration options.

You can then launch the build process

# lb build

This will take about 15-30 mins. At the end of the process, you'll find the binary.img file
in the root directory. You can flash that one directly with dd

# dd if=binary.img of=/dev/sd...

WARNING: This will cancell everything you have on the media, including the persistent
storage partition!!!
If you don't want to wipe the drive with the above command, you can just overwrite the
"live" directory on your target device with the one in the "binary" subdir in this same
directory.

If you want to rebuild your image, remember to clean before configuring.

# lb clean
