# DCJ-INDEL
DCJ-INDEL is a computational model to simulate genome evolution under various conditions.

This repository contains the DCJ-INDEL computational framework, developed in Python, for simulating genome evolution under various parameterized conditions. The core Python script, DCJ-INDEL.py, allows users to specify the number of generations and customize the probability distributions and sets of genomic operations (e.g., insertions, deletions, inversions, transpositions) to reflect different evolutionary scenarios. The model then transforms one genome configuration into another using the user-given parameters which allows us to predict how a certain genome will evolve under certain conditions. The framework also incorporates a Java-based algorithm that leverages breakpoint graph analysis to calculates the genomic distance, defined as the minimal number of operations needed to convert genome A into genome B, and outputs these distances along with gene content into text files. Large-scale simulations—up to 20,000 iterations—are efficiently handled within an hour through parallelized processing and runtime optimizations.

Additional analysis scripts are provided:

graphing.py: Generates visualizations of the genomic distance and gene content from the simulation outputs.

variance.py: Calculates and plots the variance in genomic distance.

capturing_parsimony.py: Computes the time at which genome evolution escapes parsimony, providing insights into evolutionary dynamics.
