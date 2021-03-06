# Configuration Files

[up](README.md)

OpenEmbedded is configured through "conf" files. These exist at various
[places](https://www.yoctoproject.org/docs/2.5.1/mega-manual/mega-manual.html#user-configuration)
in the sources. At the top level of the project are several files that
contain high level, or build specific configuration options. For the Yoe
project, these files include:

- **conf/auto.conf**: This file is automatically generated by the the build system
  and should not be modified.
- [**conf/site.conf**](../conf/site.conf): This file includes Yoe defaults and
  project specific changes that you want to store in git.
  This [file](../conf/site.conf.sample) includes samples of things you might want to add.
- **conf/local.conf**: This file includes changes that are specified to a user to build
  machine, and are not checked into git. This [file](../conf/local.conf.sample) includes
  samples of things you might want to add.

The above configuration files are included into the build by the
[bitbake.conf](https://github.com/YoeDistro/openembedded-core/blob/master/meta/conf/bitbake.conf#L744) file in the OpenEmbedded Core layer.

For a full list of variables available in the OpenEmbedded build system, see the
[Variables Glossary](https://www.yoctoproject.org/docs/2.5.1/mega-manual/mega-manual.html#ref-variables-glos).
