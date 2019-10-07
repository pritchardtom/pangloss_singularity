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
  * BUSCO
    - Augustus

### RECIPE:

- A few paths need setting in `%post`
- Environment PATHs need setting in `%environment`

- Need to sort out transfer of test pangloss data
- Need to sort out the GeneMark-ES key, and copy it to relevant location.

## DONE

- BioPython
- Exonerate
- GeneMark-ES and deps:
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
- R Packages
  * ggplot
  * ggrepel
  * UpSetR
  * KaryoploteR
