# singularity

Branch|[![Travis CI logo](pics/TravisCI.png)](https://travis-ci.org)
---|---
`master`|[![Build Status](https://travis-ci.org/richelbilderbeek/singularity.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity)

My notes on using Singularity

## One simple rule to learn Singularity

Find out the version you have access to, and read the
documation of that version.

```
singularity --version
2.5.2-dist
```

## Hello world

From [Peregrine tutorial](https://redmine.hpc.rug.nl/redmine/projects/peregrine/wiki/Singularity_containers_-_define_your_own_software_environment)

```
richel@sonic:~/GitHubs/singularity$ sudo singularity image.create hello_world.img
Creating empty 768MiB image file: hello_world.img
Formatting image with ext3 file system
Image is done: hello_world.img
```

```
richel@sonic:~/GitHubs/singularity$ sudo singularity build hello_world.img ubuntu.def
ERROR: hello_world.img is not an image file
Cleaning up...
```

Fails, so use pre-built image instead:

```
richel@sonic:~/GitHubs/singularity$ singularity pull shub://singularityhub/ubuntu
Progress |===================================| 100.0% 
ERROR  : Called singularity_config_get_value on uninitialized config subsystem
ABORT  : Retval = 255
Done. Container is at: /home/richel/GitHubs/singularity/singularityhub-ubuntu-master-latest.simg
```

Fails, so start from [Singularity doc](https://singularity.lbl.gov/docs-build-container):

```
richel@sonic:~/GitHubs/singularity$ singularity build hello_world.simg shub://singularityhub/ubuntu
Cache folder set to /home/richel/.singularity/shub
Progress |===================================| 100.0% 
ERROR  : Called singularity_config_get_value on uninitialized config subsystem
ABORT  : Retval = 255
ERROR: Unsupported file type: /home/richel/.singularity/shub/singularityhub-ubuntu-master-latest.simg
Cleaning up...
```

This error is described [here](https://github.com/sylabs/singularity/issues/1947#issue-358414251) 
as well.

