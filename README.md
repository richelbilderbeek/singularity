# singularity_examples

My Singularity examples.

## One simple rule to learn Singularity

Find out the version you have access to, and read the
documation of that version.

To see your version of Singularity:

```
singularity version
```

Where            |Version
-----------------|-----------------------
Lubuntu Disco    |`2.5.2-dist`
Travis CI Xenial |`2.5.0-HEAD.g50d254da5`
Peregrine        |`3.2.1-1.el7`

## Examples

Description|Singularity version|Ubuntu version
-----------------------------------------------------|---|---
[1: lolcow](https://github.com/richelbilderbeek/singularity_example_1)|v3.2.1|16.04 (xenial)
[2: lolcow on cosmic](https://github.com/richelbilderbeek/singularity_example_2)|v3.2.1|18.10 (cosmic)
[3: cowsay](https://github.com/richelbilderbeek/singularity_example_3)|v3.2.1|18.10 (cosmic)
[4: NCBI tools](https://github.com/richelbilderbeek/singularity_example_4)|v3.2.1|18.10 (cosmic)
[5: lolcow on Ubuntu 19.04 (disco) (fails)](https://github.com/richelbilderbeek/singularity_example_5)|v3.2.1|19.04 (disco) [1]
[6: City of Thieves](https://github.com/richelbilderbeek/singularity_example_6)|v3.2.1|18.10 (cosmic)
[7: ndsmake](https://github.com/richelbilderbeek/singularity_example_7)|v3.2.1|18.10 (cosmic)
[8: Zork](https://github.com/richelbilderbeek/singularity_example_8)|v3.2.1|18.10 (cosmic)
[9: MXE](https://github.com/richelbilderbeek/singularity_example_9)|v3.2.1|19.10 (cosmic)
[10: BBBQ](https://github.com/richelbilderbeek/singularity_example_10)|v3.2.1|110.10 (cosmic)

 * [1] does not work: will not upgrade from cosmic to disco

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
