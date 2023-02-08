# virt-workshop-testing

## Configurations and a script to fully test a new NVIDIA Cumulus Linux Virtual Workshop (aka Test Drive)

This repository is meant to be cloned into the `/home/ubuntu` directory on the `oob-mgmt-server`. Once cloned, change directories into the `/home/ubuntu/virt-workshop-testing` directory and execute:

`./runtests.sh`

The script will run and send all output to the console. This output can be checked to see if all `ping`, `traceroute` and other verification steps complete properly.

## Prerequisites

1. Run the CI/CD workflow located [here](https://gitlab.com/lsimpson762/virt-workshop-snapshot-creation).
2. The CI/CD workflow will create a snapshot and a live simulation (clone) in order to test the snapshot.
3. Use the live simulation and login to its `oob-mgmt-server`.