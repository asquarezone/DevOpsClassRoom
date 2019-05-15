## Basics on Working with Terraform

1. Terraform individual provisioning accepts folder
2. Every TF file in the directory will be picked up
3. Atleast one provider is required
4. Provider accepts inputs in the form of __arguments__
5. Every Provider will have resources
6. Each Resource will accept inputs which are called as __arguments__
7. When the Resource is created some details of the resources are made available using __attributes__
8. Any custom actions in the resources can be acheived using __provisioning__.
9. provisioning might required __connection__ to be created
10. Refer [here](https://www.terraform.io/docs/provisioners/index.html) for provisioners