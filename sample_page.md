## Characterizing vermicompost microbiome based on shotgun and amplicon sequecing

**Project description:** This project aimed to compare inferences from metagenomic and metataxonomic 
data to characterize the diversity of the bacterial and fungal communities associated with vermicomposting.
Vermicomposting takes advantage of the synergistic effects of worms and microorganisms (bacteria and fungi) 
to decompose organic waste. Furthermore, worms can enrich the microbial communities of the resulting compost,
enhancing subsequent production as a richer form of organic fertilizer, thus offering a sustainable alternative 
to chemicals while converting waste products into fertilizer. 


### 1. What kind of data was I dealing with?

Microbial profiles were obtained by shotgun sequencing of genomes and through amplicon sequencing of 16S rRNA for bacteria and ITS for fungi.


### 2. How was data processed?

Data from 16S and 18S sequencing were processed using the R package [*dada2* version 1.12](https://www.nature.com/articles/nmeth.3869). 
Then, the standard dada2 pipeline was applied to perform amplicon sequence variant (ASV)
inference, merge paired reads, and identify chimeras. Taxonomic assignment for 16S was
performed against the [Silva v132 database](https://doi.org/10.1093/nar/gks1219) using the dada2-formatted
training files for taxonomy and [species-level assignment](https://zenodo.org/record/1172783#.Y4l5PuzMI6A). Taxonomic
assignment for 18S was performed against the [Silva v132 Eukaryotic 18S database](https://zenodo.org/record/1447330#.Y4l5jOzMI6A).

Data from ITS sequencing were processed differently due to the variable size of the ITS region.
Raw reads from ITS sequencing were first subject to adapter trimming by cutadapt version
2.3 (Martin, 2011) which removed primer sequences due to read-through. Taxonomic assignment for ITS was performed
against the UNITE version 18.11.2018 database (UNITE Community, 2019)

For the resulting 16S, 18S, and ITS dada2-processed data, ASV sequences were aligned using
MAFFT (Katoh and Standley, 2013) and used to build a tree with FastTree (Price et al., 2010). The resulting data were imported into phyloseq
(McMurdie and Holmes, 2013) for further analysis.

### 3. Support the selection of appropriate statistical tools and techniques

<img src="images/dummy_thumbnail.jpg?raw=true"/>

### 4. Provide a basis for further data collection through surveys or experiments

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 

[//]: # (For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).)
