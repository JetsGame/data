Data
====

This repository contains a range of jet-related data sets.

There are 3 types of processes, simulated with Pythia 8.223:

* Top jets (using ttbar events with tops decaying to hadrons)
* W jets (using WW events with W decaying to hadrons)
* QCD jets (using dijet events)


For each of these processes we cluster anti-kt jets, taking the two
hardest jets with rapidity |y|<2.5 and transverse momentum above 200
GeV, 500 GeV or 2 TeV (depending on the data set).


A data set is given at parton level (turning off MPI and
hadronisation), at hadron level (turning off MI), and at truth level.

The different folders contain:
* train: training data sets of 500k jets each.
* valid: validation data sets of 50k jets each.
* test: test data sets of 50k jets each.
* declusterings: files containing the lists of declusterings of the jets.
* histograms: text file output from the runs, with some associated histograms.

Each file is a zipped json file where each line corresponds to a
separate jet, given as a list of four-momenta of its constituent
particles.