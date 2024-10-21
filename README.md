# UniNuvola

Phases to build the cluster:

Pre-requisites:

- Some machines with Ubuntu 22.04 installed and connected to the same network. The network should have connectivity to the internet.

Steps:

- Phase 1: Create the k8s cluster using the ansible playbooks contained in the `ansible` submodule.
- Phase 2: Deploy the UniNuvola constituents using the `uninuvola-init` submodule.
- Phase 3: Deploy the UniNuvola applications using the `k8s` submodule.