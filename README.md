# P5BrainReorg

Recurrence analysis of somatic neuronal DNA rearrangements

## Overview

A series of R-scripts which parse and filter the VCF files for overlapping events.

## Scripts

- `getEventClusters.R` - Filter DELLY2 VCF files for events which pass for coverage and frequency. Filtered events are then intersect and maximal clusters are determined of mutually overlapping events.


- `getEdgeClusters.R` - Filter DELLY2 events as in `getEventsClusters.R` but instead overlap regions centered on the edges of the original event and then intersect these edge regions for maximal cluster.

- `getMutectEvents.R` - Filter MuTECT2 events for total coverate and frequency and then do a simple overlap of the events between samples.

