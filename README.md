# BIOL 432 — Assignment 8: Dragon Phylogeny

This is my Assignment 8 work for **BIOL 432: Computation and Big Data in Biology** at Queen's University.

## What I did

For this assignment I worked with the Dragon Phylogeny character matrix from the Colautti Lab. I added three dragons — Drogon, Rhaegal, and Viserion — to the existing dataset and used the character data to see where they fall in a phylogenetic tree.

I first calculated pairwise distances between the dragons and then used the Neighbor-Joining method to build a tree. I also grouped the original dragons by the names in the dataset so the tree could be easier to look at.

## Data

The original character matrix is from the [Colautti Lab Dragon Phylogeny project](https://github.com/ColauttiLab/DragonPhylogeny). The original matrix contains 77 dragons and 78 binary characters. The version used here adds the three dragons from the assignment.

## Main methods

- R
- `ape` for reading the Nexus file and building the Neighbor-Joining tree
- Binary character data
- Pairwise distance calculation
- Neighbor-Joining (`nj()`)
- `ggplot2` for the distance matrix
- `ggtree` for the final tree

## Files

- `A8_Lasrado_20283881.Rmd` — main analysis
- `Data/DragonMatrix.nex` — original character matrix used for the assignment
- `input/nexus_with_dragons.csv` — updated matrix after adding the three dragons

## Running the analysis

Open `A8_Lasrado_20283881.Rmd` in RStudio and knit it to HTML or run the chunks individually.

The analysis does not install packages automatically. The required packages are `ape`, `ggplot2`, and `ggtree`.

The tree is a course exercise using a fictional dragon dataset. It should be interpreted as a demonstration of how character data can be used to build and visualize a phylogeny, rather than as a real evolutionary history.
