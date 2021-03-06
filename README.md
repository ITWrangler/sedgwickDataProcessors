

# Sedgwick Data Processors
This repository contains the tools used to convert SNBase text exports (these are custom and designed by Sedgwick Museum) to structured JSON data ready for bulk import to elasticsearch.
The 'target' for this data is an angular.js based online public access catalogue.

## Pre-requisities
* requires node.js >5.4.x

## Installation
* download repository (zip or git pull)
* `npm install` in the target directory (to install required npm packages from package.json)

## Usage (\*nix or OSX)
A bash script is supplied to run all conversions in order.

e.g.

./runprocs.sh trec5e

will take the file trec5e-up.txt through 4 stages (pre, data, remap, and espre processors) creating the final file trec5e-esbulk.txt.

## Usage (Windows/DOS/CMD)
A CMD script is supplied to run all conversions in order.

e.g.

runprocs.cmd trec5

will take the file trec5e-up.txt through 4 stages (pre, data, remap, and espre processors) creating the final file trec5edited-esbulk.txt.

## Background
I talk about the general approach in this [article](http://www.datarefinery.io/blog/2015-08-28/). I go on to talk about the pre-processor (preproc.js) [here](http://www.datarefinery.io/blog/2015-11-08/) and then the 'data processor' (dataproc.js) [here](http://www.datarefinery.io/blog/2015-11-11/).
