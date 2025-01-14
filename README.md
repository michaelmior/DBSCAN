# DBSCAN
[![Test](https://github.com/michaelmior/DBSCAN/actions/workflows/ci.yml/badge.svg)](https://github.com/michaelmior/DBSCAN/actions/workflows/ci.yml)

Lightweight Java implementation of density-based clustering algorithm DBSCAN

## Download/Building

You can download the latest jar file from the releases page.

To build the library, you can either compile the sources manually or use maven (`mvn package`).

## Usage

* Implement a distance metric for the data type to be clustered (using the interface `io.github.michaelmior.dbscan.DistanceMetric`; for an example see the implementation `io.github.michaelmior.dbscan.metrics.DistanceMetricNumbers` or consult the tests).
* Instantiate `DBSCANClusterer`.
* Invoke `performClustering()` to retrieve the clustered inputs. See tests for examples.
