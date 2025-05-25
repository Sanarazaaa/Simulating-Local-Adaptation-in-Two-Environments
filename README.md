# Simulating-Local-Adaptation-in-Two-Environments

# Population Genetics Simulation: Allele Frequency Evolution

## Introduction

This project provides a computational model to explore the fundamental principles of population genetics, specifically focusing on how natural selection can drive changes in the genetic composition of a population over time. By simulating the evolution of a single gene's allele frequency under different environmental pressures, I can gain insights into the mechanisms of adaptation and genetic variation.

## Project Goal

The primary goal of this project is to visually demonstrate the effect of natural selection on allele frequencies. I simulate the evolution of a gene with two alleles ('A' and 'a') in two distinct environmental conditions, one where allele 'A' provides a selective advantage and one where there is no selective pressure. The output plot allows for a direct comparison of these two scenarios.

## Theoretical Background

The simulation is based on core concepts from population genetics, including:

-   **Allele Frequency:** The proportion of a specific allele (e.g., 'A') in a population.
-   **Genotype:** The combination of alleles an individual possesses (e.g., AA, Aa, aa).
-   **Fitness:** The relative reproductive success of a genotype. In this simulation, fitness values determine the probability of individuals of a certain genotype contributing to the next generation.
-   **Natural Selection:** The differential survival and reproduction of individuals based on their heritable traits (genotypes), leading to changes in allele frequencies over generations.
-   **Hardy-Weinberg Principle (as a starting point):** The initial population is generated assuming Hardy-Weinberg equilibrium, which describes the theoretical conditions under which allele and genotype frequencies remain constant in a population across generations in the absence of evolutionary influences like selection, mutation, gene flow, and genetic drift. Our simulation then introduces selection to show deviations from this equilibrium.

## Simulation Model

The simulation follows a discrete-generation model. In each generation:

1.  A population is generated based on the current allele frequencies, assuming random mating.
2.  Individuals are selected to reproduce based on the defined fitness values for their genotypes. Genotypes with higher fitness have a greater chance of being selected.
3.  The allele frequencies of the selected individuals are calculated.
4.  The next generation is then created based on these new allele frequencies.

This process is repeated for a set number of generations, and the frequency of allele 'A' is recorded at each step.

## Dependencies

The project requires the following Python libraries:

-   `numpy==1.23.5`: For numerical operations, particularly for generating random choices based on probabilities.
-   `matplotlib==3.7.1`: For plotting the allele frequencies over generations.

These dependencies are commonly available in Colab environments. If running locally, you can install them using pip:
