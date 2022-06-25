# DMS Ansible Playbook Examples

This repository provides a series of Ansible playbooks that performs an end-to-end zero downtime migration using Cirrus Data's **Cirrus Migrate On-Prem
v2022** (DMS).

# Prerequisites

Before you start, you should have:

- Sufficient knowledge on Ansible, including how to execute Ansible Playbooks, specify variables, etc.
- Sufficient knowledge on SAN environments
- Hands-on experiences with DMS using GUI/cli and/or sufficient understanding on DMS concepts including insertion methods, migration, cutover process,
  uninsertion., etc.

# Demo Environment

This example is written to run in an environment as described below. To use the playbooks from this repository on your environment, you will have to modify the
relevant parts to fit into your environment using the concept demonstrated in these playbooks.
You can also [contact us](mailto:info@cdsi.us.com) to try this out using our Cirrus Data Lab-as-a-Service (LABaaS) environment.

In this environment:

- A Linux **host** with 2 initiator ports is connected to two independent Cisco fabrics (2 switches).
- A **source storage** with 2 target ports is connected to two independent Cisco fabrics.
    - Cirrus Data's Phoenix Storage Server is used in this example.
    - In your environment, source storage will be whatever storage that is currently in production in which you will be migration from.
- A pair of **DMS** with 2 nexus. One nexus is connected to the first fabric (both upstream and downstream port) and the second nexus is connected to the second
  fabric.
- **Destination storage** with 2 target ports connected to the two fabrics respectively
    - Pure Storage FlashArray is used as the destination storage (migration target) in this example.



# Playbooks
Multiple playbooks are included in this repository. 



# Customization

This example is written to run in an environment as described below. To use the playbooks from this repository on your environment, you will have to modify the
relevant parts to fit into your environment using the concept demonstrated in these playbooks.

To customize the playbooks 
