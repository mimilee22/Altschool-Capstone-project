# Altschool-Capstone-project
## AKS Infrastructure with Terraform and GitHub Actions

This repository demonstrates deploying infrastructure to Azure Kubernetes Service (AKS) using Terraform and a CI/CD pipeline built with GitHub Actions.

### Tools Used

* **Infrastructure as Code (IaC):** Terraform
* **Continuous Integration/Continuous Delivery (CI/CD):** GitHub Actions
* **Cloud Platform:** Azure Kubernetes Service (AKS)

### Project Structure

This repository includes the following directories:

* **.github/workflows:** Contains workflow files defining the CI/CD pipeline.
* **terraform:** Contains Terraform configuration files for provisioning the AKS cluster and related resources.
* **variables.tf:** (Optional) Stores sensitive information like Azure credentials outside of version control.
* **README.md:** (This file) Provides an overview of the project.


### Getting Started

1. **Prerequisites:**
    * A GitHub account and repository.
    * An Azure subscription with sufficient permissions.
    * Terraform installed locally ([https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)). 
    * Basic understanding of Terraform syntax.

2. **Configuration:**
    * Update the `variables.tf` file (if used) with your specific Azure credentials and desired configuration values.
    * Review the Terraform files (`*.tf`) to understand the infrastructure being deployed.

3. **Deployment with GitHub Actions:**
    * Push your code to the GitHub repository.
    * The defined workflow in `.github/workflows` will automatically execute on push events.
    * The workflow will perform Terraform initialization, plan, and apply stages.


### Additional Notes

* This is a basic example and can be extended to deploy additional resources within the AKS cluster using tools like Helm.
* Security best practices recommend storing sensitive information like passwords and access keys in secrets management tools instead of version control.


### Contributing

We welcome contributions to this project! Please create a pull request to share your improvements.


### License

This project is licensed under the MIT License. See the LICENSE file for details.
