AraPPISite
=======================
AraPPISite is an integrated database presenting fine-grained protein-protein interaction site annotations for Arabidopsis thaliana.

Explanation/Example
------------------------
* classification_of_protein-protein_interactions.xlsx

The classification_of_protein-protein_interactions.xlsx file contains four sheets: Experiment, HMPC, PRISM and DDI_and_DMI. You can find the protein-protein interactions whose complex structures are experimentally determined in the Experiment sheet; the protein-protein interactions whose complex structures are predicted using Homology Modeling of Protein Complex (HMPC) in the HMPC sheet; the protein-protein interactions whose complex structures are predicted using Protein Interactions by Structural Matching (PRISM) in the PRISM sheet; and the protein-protein interactions whose domain-domain interaction (DDI) and domain-motif interaction (DMI) are annotated in the DDI_and_DMI sheet.

* protein_complex_structures folder

The protein_complex_structures folder contains the PDB files of 3,050 protein complex structures in AraPPISite. The PDB files are named using two TAIR identifiers of an interacting protein pair. In a PDB file, chain A represents the first interacting protein and chain B represents the second interacting protein.

For example:
File name: AT1G01040-AT1G09700.pdb 
Chain A represents AT1G01040 and chain B represents AT1G09700 in the PDB file.

* protein_interaction_sites folder

The protein_interaction_sites folder contains the protein interaction sites for 3,050 protein-protein interactions whose protein complex structures are stored in the folder of protein complex structures. The files are named using two TAIR identifiers of an interacting protein pair. There are six columns in a file. Each line shows an interacting residue pair.

For example:
File name: AT1G01040-AT1G09700.txt
File content: AT1G01040	SER	979	AT1G09700	GLN	111
Column 1: AT1G01040 (The TAIR identifier of the first interacting protein)
Column 2: SER (The name of one interacting residue from AT1G01040)
Column 3: 979 (The residue sequence number of the interacting residue in the Column 2)
Column 4: AT1G09700 (The TAIR identifier of the second interacting protein)
Column 5: GLN (The name of the other interacting residue from AT1G09700)
Column 6: 111 (The residue sequence number of the interacting residue in the Column 5)

* domain-domain_and_domain-motif_interaction_annotations folder

The domain-domain_and_domain-motif_interaction_annotations folder contains all domain-domain and domain-motif interactions for 4,286 PPIs whose protein complex structures are unknown in AraPPISite. The files are named using two TAIR identifiers of an interacting protein pair. There are four columns in a file. Each line shows a domain-domain/motif interaction.

For example:
File name: AT1G01040-AT3G20550.txt
File content: AT1G01040_AT3G20550	LIG_FHA_1	PF00498	89-95,352-358,369-375,644-650,723-729,810-816,920-926,1160-1166,1303-1309,1355-1361,1608-1614,1758-1764,1864-1870	219-299
Column 1: AT1G01040_AT3G20550 (The name of protein-protein interaction)
Column 2: LIG_FHA_1 (The name of one interacting motif from AT1G01040)
Column 3: PF00498 (The name of the other interacting domain from AT3G20550)
Column 4: 89-95,352-358,369-375,644-650,723-729,810-816,920-926,1160-1166,1303-1309,1355-1361,1608-1614,1758-1764,1864-1870 (The sequence range of the interacting motif in the Column 2)
Column 5: 219-299 (The sequence range of the interacting domain in the Column 3)
=======================
Hong Li, Shiping Yang, Chuan Wang, Yuan Zhou, and Ziding Zhang. (2015) AraPPISite: a database of fine-grained protein-protein interaction site annotations for Arabidopsis thaliana. http://systbio.cau.edu.cn/arappisite/.

Corresponding authors: Yuan Zhou (soontide6825@163.com) and Ziding Zhang (zidingzhang@cau.edu.cn)
