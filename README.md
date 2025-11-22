# noto-fonts-tarball
Noto fonts packaged into a tarball for Linux and other Unix-like systems.

Originally created for use in the build system of MassOS.

If you want to obtain Noto fonts, it is strongly recommended to use your distro's packages, or download them directly from [Google Fonts](https://fonts.google.com/noto).

For licensing information, please see the comment at the start of the `package.sh` script.

Note that creating packaging tarballs manually using the `package.sh` script requires downloading around 20GB of data, even though the output tarballs are much smaller. Be aware of this if you are on a connection that is slow and/or metered.

Note also that the `package.sh` script should be run using `fakeroot` (or otherwise blatantly as the root user), so as to ensure the files inside the tarball will be owned by the root user, suitable for extraction into system-wide locations later.
