
# Building AI

Detection of seizure activity from EEG recordings

## Summary

This project works towards automatic annotation of electrophysiological recordings based on the presence of epileptic activity. The idea is to use AI methods and large sets of supervised data in order to come up with a well generalized model.

## Background

Some instances of epileptic seizures are not as apparent as others. These are not noticeable from a patient's behavior, but the abnormal brain activity does however appear on EEG recordings. The identification and annotation of seizure activity is not trivial and requires an expert. Since this expertise is not always widely available, an automated annotation algorithm could prove useful.

## How is it used?

A classifier should first be trained using labeled EEG data consisting of both seizure and seizure-free segments. The classifier can then be fed unseen data, which it subsequently annotates (for example by labeling each second of data). Such application could be used in a clinical setting in order to support and speed up the work of the experts.

## Data sources and AI methods

The considered data comes from a dataset of neonatal EEG recordings (see acknowledgements). It contains 19-channel EEG recordings from 79 neonates that were annotated by three different experts. The data was originally collected at the Helsinki University Hospital.

The main objective of this project is assigning labels to segments of time series data. AI methods for classification will be used, more specifically binary classification.

## Challenges

EEG data is often noisy, meaning some form of preprocessing should be applied. Which specific features that are extracted from the data will influence the performance of the classifier and should be chosen accordingly. The selection of which EEG channel to consider is also not trivial. A selection method (see acknowledgements) could be used for this.

## What next?

This project could improve by making use of more complex AI techniques that are tailored towards this specific problem. More advanced courses in AI but also neuroscience could be considered to do so.

## Acknowledgments

This project is inspired by the Building AI course from Introduction of AI, as well as courses from the master Biomedical Engineering from KU Leuven.

[Neonatal EEG data] (https://www.nature.com/articles/sdata201939)

[Seizure channel selection] (https://www.frontiersin.org/articles/10.3389/fnins.2020.00593/full)
