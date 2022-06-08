# MINE 2.0: enhanced biochemical coverage for peak identification in untargeted metabolomics

MINEs (Metabolic *In silico* Network Expansions) are databases of predicted biological compounds. These compounds are predicted by applying biochemical reaction rules to known metabolites. The set of rules used to build MINE 2.0 is much more comprehensive than that used for MINE 1.0 (see the published ruleset [here](https://pubmed.ncbi.nlm.nih.gov/33662575/)).

This repo contains all code used to generate results reported in the MINE 2.0 paper. If you use this code or MINE 2.0 itself, please cite the [MINE 2.0 paper](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btac331/6589885?login=true). If you don't have access to *Oxford Bioinformatics*, e-mail me at jonstrutz11@gmail.com, and I will be happy to send you a copy!

Finally, the MINE 2.0 website can be accessed [here](https://minedatabase.ci.northwestern.edu/#/home).

## Notebooks
All notebooks located in `./02 Analyzed data/Notebooks_Final`.

### Table 1
- No notebooks. All calculations for Table 1 were made by directly querying the MINE MongoDB.

### Table 2
- `Mass_Bank_Coverage_KEGG.ipynb`
- `Mass_Bank_Coverage_KEGG1.0.ipynb`
- `Mass_Bank_Coverage_KEGG2.0.ipynb`
- `Mass_Bank_Coverage_PubChem.ipynb`
- `PubChem_Unique_Formulas.ipynb`

### Table 3
- `Sauer_Coverage_KEGG.ipynb`
- `Sauer_Coverage_KEGG1.0.ipynb`
- `Sauer_Coverage_KEGG2.0.ipynb`
- `Sauer_Coverage_EcoCyc1.0.ipynb`
- `Sauer_Coverage_EcoCyc2.0.ipynb`
- `Sauer_Coverage_PubChem.ipynb`

### Other Notebooks
- `KEGG_Dataset_SMILES_to_Mass.ipynb` (calculate mass for all KEGG compounds)
- `MassBank_MS2_Search_KEGG2.0` (for MS2-based search results in SI)

## Final Notes

Note that to run most of the notebooks, I used a direct connection to our MongoDB database (rather than going through the MINE API) with my credentials stored in a `credentials.txt` file. To replicate this work, you will need to use the [MINE API](https://mine-api.readthedocs.io/en/latest/) instead. You will also need to install [minedatabase](https://github.com/tyo-nu/MINE-Database).

Also note that some large files are not present in this repo (see .gitignore) but are available upon request.