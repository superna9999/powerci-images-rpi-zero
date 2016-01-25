Linaro Test Images for ARMv6
======

```
$ mkdir openembedded
$ cd openembedded
$ git clone git://git.linaro.org/openembedded/jenkins-setup.git
$ cd jenkins-setup
$ bash init-and-build.sh
```

`$ cp meta-linaro_meta-linaro_conf_machine_genericarmv6.conf meta-linaro/meta-linaro/conf/machine/`

Defaults to ARMv8, this should only change the MACHINE declaration to genericarmv6 :

`$ cp build_conf_site.conf build/conf/`

Then build the images :

`$ bitbake linaro-image-minimal-initramfs`

=> tmp-glibc/deploy/images/genericarmv6/linaro-image-minimal-initramfs-genericarmv6.cpio.u-boot
