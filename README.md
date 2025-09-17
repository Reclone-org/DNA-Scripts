# DNA-Scripts (work in progress)

Jupyter Notebook scripts for preparing DNA parts for inclusion in Reclone syntax assemblies or in the Open DNA collection. 
Three main workflows have been produced:

1.  Synthesis of protein-coding parts (codon-optimized) ([Collab Notebook](https://colab.research.google.com/drive/1dfit-8ESbeLiSHSgfPqT7AWx7Xy24Zmt?usp=sharing))

-   Input protein sequences and 5′/3′ Reclone tags.
-   Pipeline reverse-translates, optimizes, enforces constraints, adds Reclone/BbsI adapters, and outputs order-ready DNA parts.
-   Best when you want clean, synthesis-grade CDS parts with early-codon tuning.

2.  Add syntax overhangs & sites by PCR ([Collab Notebook](https://colab.research.google.com/drive/1VJeIK1ndN_PZPeJQTlIKLl9c9099Z6ZA?usp=sharing))

-   You already have a DNA template and want to append Reclone/BbsI ends via PCR.
-   The PCR script generates primer sequences that add the correct Type IIS sites, overhangs, and spacers for cloning---no global re-design or codon optimization.
-   Best for quick cloning from an existing plasmid or for small variants.

3.  Synthesis of non-coding parts (no codon optimization) ([Collab Notebook](https://colab.research.google.com/drive/1m8WpdoqMMZ5ik5TyEyTdxJ12bPv1kDpZ?usp=sharing))

-   For promoters, RBS/UTRs, linkers, terminators, regulatory elements, etc.
-   Takes DNA sequences as-is, adds the appropriate Reclone tags and outer BbsI adapters, checks constraints, and outputs order-ready parts.
-   Best when the sequence must be preserved (no translation/codon constraints).

-   Please add any issues you find to the repository!
