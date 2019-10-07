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
  * Muscle
  * PAML
  * InterProScan
  * GOATools
  * R Packages:
    - ggplot
    - ggrepel
    - UpSetR
    - KaryoploteR

