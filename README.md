# UniNuvola

## Repo structure:

- `core`: Contains the core components of the UniNuvola project. Each component is a submodule and contains the code and configuration files for the component. This directory is meant to be used as a quick reference to other repositories in the UniNuvola organization.
- `docs`: Contains the documentation for the project.
- `operations`: Contains all the tools and scripts used to manage an UniNuvola cluster.
- `phase1`: Contains the ansible playbooks to create a kubernetes cluster whit the necessary configurations to deploy the UniNuvola constituents.
- `phase2`: Contains the scritps to deploy the UniNuvola constituents over the kubernetes cluster.
- `phase3`: Contains the scripts to deploy the UniNuvola applications 
over the kubernetes cluster.
- `testing`: Contains the scripts to test the UniNuvola applications and configurations.

## Phases to build the cluster:

Pre-requisites:

- Some machines with Ubuntu 22.04 installed and connected to the same network. The network should have connectivity to the internet.

Steps:

- Phase 1: Create the k8s cluster using the ansible playbooks contained in the `ansible` submodule.
- Phase 2: Deploy the UniNuvola constituents using the `uninuvola-init` submodule.
- Phase 3: Deploy the UniNuvola applications using the `k8s` submodule.