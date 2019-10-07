# Pangloss Singularity Container

This is a work-in-progress recipe to install [Pangloss](https://github.com/chmccarthy/Pangloss) in a Singularity
container.

## Dependency Tree

- Pangloss
  * BioPython
  * Exonerate
  * GeneMark-ES
    - YAML::Any              (Perl modules)
    - Hash::Merge
    - Logger::Simple
    - Parallel::ForkManager
  * TransDecoder
  * Blast+
  * BUSCO
    - Hmmer
    - Augustus
      * samtools
      * various `apt-get` packages
  * Muscle
  * PAML
  * InterProScan
  * GOATools
  * R Packages:
    - ggplot
    - ggrepel
    - UpSetR
    - KaryoploteR

## TO-DO

### INSTALL:

- Pangloss
  * GeneMark-ES (sort key file out too)
  * BUSCO
    - Augustus
  * R Packages
    - ggplot
    - ggrepel
    - UpSetR
    - KaryoploteR

### RECIPE:

- A few paths need setting in `%post`
- Environment PATHs need setting in `%environment`


## DONE

- BioPython
- Exonerate
- GeneMark-ES Dependencies:
  * YAML::Any            
  * Hash::Merge
  * Logger::Simple
  * Parallel::ForkManager
- TransDecoder
- Blast+
- Hmmer
- Muscle
- PAML
- GOATools
- Samtools
