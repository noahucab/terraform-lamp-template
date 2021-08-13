# Provisioning an AWS instance using Infrastructure as Code with Terraform

As part of our improving our workflows and automating repeatable steps in our processes, this code will provision a web server without going through tedious steps when setting up web server instance using GUI. Streamlining our processes would help us focus on the business process and prioritizing what is important.

In this code, it will setup a LAMP-stack based server. All the necesary toolings and libraries will be installed when you execute the code or template.

## Getting Started

Before you can run the code in the following sections, you need to download and install the follwoing:

1. [Terraform CLI](https://www.terraform.io/downloads.html)

## How to run

First, we need to create a plan. This will generate a file. Inside this file, it is a preview of what services will be added, updated, and deleted.

`$ terraform plan -out newplan.tfplan`

After creating the plan with the new resources, we can now execute the plan. To apply this plan,

`$ terraform apply "newplan.tfplan"`

This will update the **state** file file containing the updated configuration for your infrastructure.
## Important Note:

This is an initial documentation. If you notice there are some steps missing or any suggestions (which is I would highly recommend) that we need to add with the current setup, you can message me and lets collaborate to improve this template and documentation.
