Etherpad-APB
======================

An APB for deploying [etherpad lite](https://github.com/ether/etherpad-lite).  
Adapted from https://github.com/yatesr/playbook-etherpad

## What it does
* Installs nodejs, mysql-server, nginx, etherpad-lite.
* Deploys etherpad application to Openshift

## Requirements
* Must have docker installed and parameters to authenticate against OCP cluster

## Running the application
`docker run -e "OPENSHIFT_TARGET=<openshift_target>" -e "OPENSHIFT_TOKEN=<token>" ansibleplaybookbundle/etherpad-apb provision`
## Tearing down the application
`docker run -e "OPENSHIFT_TARGET=<openshift_target>" -e "OPENSHIFT_TOKEN=<token>" ansibleplaybookbundle/etherpad-apb deprovision`
