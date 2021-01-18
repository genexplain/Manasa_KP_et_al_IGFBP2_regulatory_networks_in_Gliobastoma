# Manasa_KP_et_al_IGFBP2_regulatory_networks_in_Gliobastoma
Links to computational workflows, supplementary research data and results of the study\
doi: 10.20944/preprints202010.0046.v2

**The Workflow**\
In the study, we developed a computational workflow for analysis of publicly available datasets of Glioblastoma multiforme to understand the gene regulatory networks driving short survival. To understand such gene regulatory networks, the Genome Enhancer (https://ge.genexplain.com) pipeline developed on the basis of open source BioUML platform (www.biouml.org). The pipeline used the Upstream Analysis protocol described earlier [https://pubmed.ncbi.nlm.nih.gov/30999858/], which integrates promoter and pathway analysis, to identify signalling molecules as potential drug targets of the studied pathology. Datasets used in the study, clinical info and workflow descriptions are described here as well as in the manuscript cited below. Results and the computational workflow are provided with public access.  

**Data Folder**\
Contains (a) cleaned up expression data (b) Sample info (c) Limma and (d) list of upregulated genes for GSE dataset (GSE108474  & GSE53733) and TCGA-GBM microarray dataset. 
The GSE_upregulated(0.5).txt and TCGA_upregulated(0.5).txt both can be used as input to the workflow. TCGA-GBM microarray data were used to validate the observations.

**Study result**\
The results reported in the article can be accessed and viewed **[here](https://ge.genexplain.com/#de=data/Projects/Regulatory_Networks_of_Glioblastoma_survival/Data/GSE_dataset/Outputs/CMAWK%20on%20enhancers%20output/Feedback%20Controlled%20Master%20Regulators)

**Workflows**\
The computational workflow applied in the study can be inspected here

**Workflow execution**\ 
To run the workflow please click here. Drag and drop the input file of upregulated genes– “GSE dataset/ GSE_uprergulated(0.5)” onto the workflow execution box. The results are generated and will be accessible under Results_new/Output/ folder 

**Workflow result**\
This automated workflow, generates a results folder –Results of the workflow will be in  Results_new/output/ folder. 

1.	*CMAWK on Enhancers* - Contains results of Transcription factor binding site analysis and CMA analysis 
  a. Optimization summary – List of transcription factor binding motifs enriched in the promoters of dysregulated genes – defined in Methods section 4.5 
  b. CMA with factors and Description – Applying Composite Module Analyst combinations of TF motifs (from TRANSFAC®) whose sites are most frequently clustered together in the regulatory regions of the studied genes  
  c. Feedback controlled Master regulators – List of master regulators identified in the study
  d. CMA Modules – Which contains details of CMA analysis along with identification of master regulators – “Keynodes for best model annotated ranked filtered” and corresponding visualization of the regulatory network mapped onto gene expression values - Keynodes for best model viz_express

2.	 *Functional classification of Ensembl genes* – Functional annotation of the given set of genes based on integrated databases of geneXplain platform – Biological process, Cellular  component and Molecular function based on HumanPSD database along with TRANSPATH Pathway enrichment 
3.	*CMA with factors* – Representation of binding sites for the identified Transcription factor on the promoters of the input DE genes
4.	*The final full report of the workflow* – It gives the full description of the analysis, shows the major results, gives lists of found potential master-regulators – drug targets and gives and overview of known or repurposing drugs in this disease targeting identified targets. 
