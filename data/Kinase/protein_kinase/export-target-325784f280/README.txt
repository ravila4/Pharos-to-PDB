
This file describes the column headings in the CSV files obtained when
downloading targets, diseases or ligands. Each section below
corresponds to individual entity files. The url for this export is as
follows:

https://pharos.nih.gov/idg/targets?facet=IDG+Development+Level/Tchem&facet=IDG+Development+Level/Tclin&facet=DTO%20Protein%20Class%20(1)/Protein%20kinase&action=download

The export was performed on Wed Jan 30 20:16:41 EST 2019 by Pharos build
a759bb7. The TCRD version was 5.4.0.

diseases.csv
------------

This file describes the diseases associated with a target. Each row
corresponds to one disease 

Column Headers -

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/)
to get the complete URL. 
Uniprot ID - the Uniprot ID of the target associated with this disease
DOID - the Disease Ontology identifier for this disease
Name - name of the disease
Description - description of the disease
ZScore - the Jensen Lab text mining Z-score
(http://www.sciencedirect.com/science/article/pii/S1046202314003831) 
Confidence - the Jensen Lab text mining confidence
(http://www.sciencedirect.com/science/article/pii/S1046202314003831) 
Link - link to the entry for this disease/target association in the
DISEASES database

expression.csv
--------------

This file lists the tissue expression levels associated with a target.
Each line is a single tissue expression level for a single target.

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/)
to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
Source - source of the expression data
Tissue - the name of the tissue
NumericValue - the numeric expression level
QualitativeValue - the qualitative expression level
Confidence - confidence in the expression value
Evidence - evidence for the expression value

generifs.csv
------------

This file lists the Gene RIFs
(http://www.ncbi.nlm.nih.gov/gene/about-generif) associated with a
target. Each line is a single target - Gene RIF association.

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/) to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
PMID - Pubmed ID for the article from which the Gene RIF was obtained
Abstract - the abstract of the article

goterms.csv
-----------

This file lists the GO (http://geneontology.org/) terms associated
with a target. Each line is a single target-GO term association.

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/) to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
GOTerm - the term name
GOType - the GO term type (process, function or cellular location)

ligands.csv
-----------

This file lists the ligands associated with a target. Each line is a
single target-ligand association. 

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/) to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
Name - ligand name
Type - ligand type
Description - ligand description
SMILES - the SMILES representation of the ligand structure
Link -
ChEMBL Activity - numeric activity value from ChEMBL
ChEMBL Activity Type - text string indicating the type of activity (e.g., Ki)

pathways.csv
------------

This file lists pathways associated with a target. Each line is a
single target-pathway association. 

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/)
to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
Name - pathway name
Source - source database for the pathway
Link - link to this pathway in the source database

publications.csv
----------------

This file lists publications associated with a target, obtained via
text mining. Each line is a target-publication association.

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/) to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
PMID - Pubmed ID for the article from which the Gene RIF was obtained
Title - article title
Abstract - the abstract of the article

targets.csv
-----------

This file lists information associated with a target. Each line is a
single target.

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/)
to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
Name - name of target from Uniprot
Description - description from Uniprot
Development Level - target development level (e.g., Tdark)
DTOClass - Drug Target Ontology assigned to the target
PantherClass - Panther Ontology assigned to the target
Novelty - novelty score
Target Family - target family (e.g., kinase, GPCR)
PatentCount - number of patents referring to this target
AntibodyCount - number of antibodies available for this target
PubmedCount - number of articles associated with the target (obtained
via text mining)
Knowledge Availability - an indicator of the total knowledge known
about the specific target
PubmedScore - derived from text mining a set of Pubmed
abstracts. See https://pharos.nih.gov/idg/pmscore for more details
PubtatorScore - a score characterizing the occurence of the target in
biomedical literature. See
https://www.ncbi.nlm.nih.gov/CBBresearch/Lu/Demo/PubTator/ for more
details
PMIDS - comma separated list of Pubmed IDs for the associated articles

uniprot-keywords.csv
--------------------

This file lists Uniprot keywords associated with a target. Each line
is a single target-keyword association.

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/)
to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
Keyword - the Uniprot keyword
Link - link to the keyword on Uniprot

harmonizome.csv
---------------

This file lists the cumulative distribution function (CDF) values
obtained from the Harmonizome
(http://amp.pharm.mssm.edu/Harmonizome/). In contrast to the other
files, this is in "long" format so that CDF values for a given target
are on seperate lines.

URL - the partial URL to the disease entry on the Pharos website. You
should prepend it with the host name (e.g., https://pharos.nih.gov/)
to get the complete URL.
Uniprot ID - the Uniprot ID of the target associated with this disease
Data Source - the data source used to calculate the CDF
DSURL - the URL to the data source
Data Type - the type of the data source
Attribute Group - the attribute group
Attribute Type - the attribute type
CDF - the value of the CDF for this target with respect to this data
source. High values indicate that this data source has more
associations with this target
