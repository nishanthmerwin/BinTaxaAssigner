# BinTaxaAssigner


KrakenHLL outputs kmer frequencies per contig in a bin but user needs to visually compare all the contigs within a bin and decode the most appropiate taxnomic level depends on k-mer frequence. BinTaxaAssigner investigate the quality of a hit at species-level, if a species-level hit fails to meet a certain quality threshold it goes to next taxonomic level up to phylum-level. How to use the function: MAG_TaxaAssigner(krakenHll_output)


#MAG_TaxaAssigner() This is a function to assign proper taxon to each metagenome assembled bin using a unique k-mer count (the HyperLogLog) algorithm from KrakenHLL. please read KrakenHLL for more https://github.com/fbreitwieser/krakenhll
