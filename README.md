# TRANSIT 2.0.2_zhang

**For TTP analysis ONLY** - use latest version for statistical analysis of post-TPP .wig files. 

**New in Version 2.0+**
 - Support for Tn5 datasets.
 - New analysis methods.
 - New way to export normalized datasets.

**Version 2.0.2 changes (August, 2016)**
- Added support for for custom primers in TPP.
- Added support for annotations in GFF3 format.
- Ability to specify pseudocounts in resampling.
- Misc. Bug fixes
- **New [mailing list](https://groups.google.com/forum/#!forum/tnseq-transit/join)**

**Verision 2.0.2_zhang changes (October, 2019)**
- change hardcoded values in tpp.py to match Zhang/Niederweis protocol
  - ADAPTER2="CGACCACGACC"
  - const1 = "GTCAAGTCTCGCAGATGATAAGG"
  - const2 = "CTTGGTTTGGTCGTGGTCG"
  - const3 = "TAACAGGTTGGCT"
  

## v2.0.2_zhang: hardcoded alternate set of adapter/const sequences.

The easiest way to install/run this is to use Anaconda3 to create a transit enviroment, including all dependencies,
```
conda create -n transit233 -c bioconda transit=2.3.3 bwa
```

Then git clone this branch of this repository
```
git clone https://github.com/rusalkaguy/transit.git transit_v2.0.2_zhang
cd transit_v2.0.2_zhang
git checkout v2.0.2_zhang
```

Finally, activate the environment, but then run the cloned TRANIST/TPP (```./transit_v2.0.2_zhang/src/tpp.py ...```)

This version should only be used for processing .fastq files into .wig files. 

Once you have your .wig files, please **conduct statistical analyses with the latest avaiable version of TRANSIT**.


# Welcome

Welcome! This is the distribution for the TRANSIT and TPP tools developed by the Ioerger Lab.

TRANSIT is a tool for the analysis of Tn-Seq data. It provides an easy to use graphical interface and access to three different analysis methods that allow the user to determine essentiality in a single condition as well as between conditions.

## Mailing List

You can join our mailing list to get announcements of new versions, discuss any bugs, or request features! Just head over to the following site and enter your email address:

https://groups.google.com/forum/#!forum/tnseq-transit/join




## Instructions

For full instructions on how to install and run TRANSIT (and the optional pre-processor, TPP), please see the documentation included in this distribution ("doc" folder) or visit the following web page:


http://saclab.tamu.edu/essentiality/transit/transit.html


## Datasets

The TRANSIT distribution comes with some example .wig files in the data/ directory, as well as an example annotation file (.prot\_table format) in the genomes/ directory. Additional genomes may be found on the following website:

http://saclab.tamu.edu/essentiality/transit/genomes/


## Copyright Information

Source code for TRANSIT and TPP are available open source under the terms of the GNU General Public License (Version 3.0) as published by the Free Software Foundation. For more information on this license, please see the included LICENSE.md file or visit their website at:

http://www.gnu.org/licenses/gpl.html
