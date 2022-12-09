## Finding Potential Epitope sites on COVID-19 S Protein

**Project description:** At the height of the COVID-19 pandemic, our goal was to find a site that a neutralizing antibody can bind to that is crucial for viral entry of the cell and prevent it from entering the host cell. Hence, our primary target was the S protein as it plays a key role in viral attachment, fusion, entry, and transmission. Host cell entry depends on the binding of the viral S proteins to cellular receptors and [S protein priming by host cell proteases](https://pubmed.ncbi.nlm.nih.gov/32142651/). Particularly, our focus was on the S1 subunit which consisted of the receptor-binding domain (RBD) which is crucial for [binding to host cells](https://pubmed.ncbi.nlm.nih.gov/32249063/). We wanted to find an epitope site on the SARS-CoV-2 S protein sequence where a neutralizing antibody can bind to and this site would ideally be important for viral cell entry and contain a possible proteolytic cleavage site. Furthermore, a strongly neutralizing antibody is one that competes for both cell entry and protease cleavage. 

### 1. How was data processed?

SARS-CoV-2 S protein crystal structure sequence was pulled from GenBank (PDB ID: 6X6P) and is composed of three identical subunits. To map possible epitope surfaces on the sequence, it was analyzed on [BepiPred 2.0](10.1093/nar/gkx346) which is a web server for predicting B-cell epitopes on an antigenic sequence. Epitopes that were accepted were above the default parameter value of 0.5 and only picked within the S1 subunit. To see if there were other possible proteolytic cleavage sites on the SARS-CoV-2 sequence, we analyzed the crystal structure sequences using software such as [iProt-Sub](https://doi.org/10.1093/bib/bby028) and [Procleave](10.1016/j.gpb.2019.08.002) as means to cross-compare results from each. 

The proteases were chosen based on their ability to activate SARS-CoV and other coronaviruses based on current literature, as there were not much information regarding the cellular proteases that can activate SARS-CoV-2 (Millet and Whittaker, 2015). The epitope sites and cleavage sites were then mapped on Chimera (Pettersen et al., 2004) for visualization on the SARS-CoV-2 S protein. The epitope and cleavage sites were color-coded
according to their positions (as seen on the home page of the project).


### 2. How was data analyzed?
Click [here](https://docs.google.com/presentation/d/1umXnbUF3ZsVV_Ev_eEH5UHNSQbRNiTryFM7SetCvnSU/edit#slide=id.p) for the final analyses of this project. 
Our conclusion was that the furin cleavage site is of interest to us as it is not found in SARS-CoV and is unique to SARS-CoV-2 due to its prime location nestled within the receptor-binding motif which is crucial for the viral entry into the host cell.


<!--- For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/). -->
