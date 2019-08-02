# singularity_examples

Branch|[![Travis CI logo](pics/TravisCI.png)](https://travis-ci.org)
---|---
`master`|[![Build Status](https://travis-ci.org/richelbilderbeek/singularity.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity)

My Singularity examples.

## One simple rule to learn Singularity

Find out the version you have access to, and read the
documation of that version.

To see your version of Singularity:

```
singularity --version
```

Where            |Version
-----------------|-----------------------
Lubuntu Disco    |`2.5.2-dist`
Travis CI Xenial |`2.5.0-HEAD.g50d254da5`
Peregrine        |`3.2.1-1.el7`

## Examples

[![Travis CI logo](pics/TravisCI.png)](https://travis-ci.org)|Description
-------|-----------------------------------------------------
[![Build Status](https://travis-ci.org/richelbilderbeek/singularity_example_1.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity_example_1) | [1: Use newest Singularity](https://github.com/richelbilderbeek/singularity_example_1)
[![Build Status](https://travis-ci.org/richelbilderbeek/singularity_example_2.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity_example_2) | [2: Use default Singularity](https://github.com/richelbilderbeek/singularity_example_2)
[![Build Status](https://travis-ci.org/richelbilderbeek/singularity_example_3.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity_example_3) | [3: cowsay on Ubuntu 18.40](https://github.com/richelbilderbeek/singularity_example_3)
[![Build Status](https://travis-ci.org/richelbilderbeek/singularity_example_4.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity_example_4) | [4: NCBI tool on Ubuntu 18.40](https://github.com/richelbilderbeek/singularity_example_4)
[![Build Status](https://travis-ci.org/richelbilderbeek/singularity_example_5.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity_example_5) | [5: Ubuntu 19.04 (disco)](https://github.com/richelbilderbeek/singularity_example_5)
[![Build Status](https://travis-ci.org/richelbilderbeek/singularity_example_6.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity_example_6) | [6: City of Thieves](https://github.com/richelbilderbeek/singularity_example_6)
[![Build Status](https://travis-ci.org/richelbilderbeek/singularity_example_7.svg?branch=master)](https://travis-ci.org/richelbilderbeek/singularity_example_7) | [7: ndsmake](https://github.com/richelbilderbeek/singularity_example_7)
--- | 8: Zork
--- | 9: MXE

## Notes to self

### Why not to use `Richèl` as author name

When doing this:

```
%labels

    AUTHOR Richèl J.C. Bilderbeek
```

The `è` gets turned to Unicode:

```
richel@sonic:~/GitHubs/singularity_example_3$ singularity inspect ubuntu_cowsay.simg 
{
    "AUTHOR": "Rich\u00e8l J.C. Bilderbeek",
```

## Links

 * Singularity documentation: [https://sylabs.io/docs/](https://sylabs.io/docs/)
 * Singularity v2.5 documentation: [https://sylabs.io/guides/2.5/user-guide/](https://sylabs.io/guides/2.5/user-guide/)
