# Infra Provisioning

## Need
* Creating multiple environments during your application development/testing/releases
* How do you create multiple environments
    * manual
        * it is time consuming 
        * same state is not guarnteed
    * automated
        * Specific Tools
            * ARM Templates
            * Cloud formation
            * Problem : Very specific to cloud provider. Cannot be reused if you want same automation in different cloud 
        * Generic Tools
            * Packer
            * Terraform
            * Advantage: One way of working with any cloud provider

## Purpose of Image
* Reuse same applications/os in your pipeline
* Packer is generic tool to create reusable images