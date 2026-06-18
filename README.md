# Kiro Workshop - Lab Environment Setup

## Prerequisites

This lab runs on an Ubuntu-based EC2 instance. Two setup steps are required before following the workshop instructions.

## Step 1: Download Workshop Assets

Go to the workshop assets repo:

https://github.com/perryjm07/kiro-workshop-assets

Go to Code and Download Zip

There are two zip files available:
- **kiro-workshop-assets.zip** — contains the base workshop code (built for macOS)
- **kiro-workshop-assets-fix.zip** — USE THIS ONE. This contains the updated code that works on this Linux environment


## Step 2: Update EC2 Instance Profile

The EC2 instance role does not have sufficient permissions for CDK bootstrap and deploy by default. You must manually attach the `AdministratorAccess` policy:

1. Open the AWS Console
2. Go to **IAM > Roles**
3. Search for the role attached to this instance (e.g. `kiro-ide-remote-en-InstanceRole-*`)
4. Click **Add permissions > Attach policies**
5. Search for and attach **AdministratorAccess**

## Step 3: Deploy the Application

Follow the workshop instructions to manually deploy the infrastructure:

https://catalog.workshops.aws/kiro-immersion/en-US/15-sample-application/151-deploy-application

## Step 4: Generate Steering Documents

After the deploy completes, generate steering documents for the project:

1. In Kiro, look for the **AGENT STEERING & SKILLS** section in the sidebar
2. Click the **+** (plus sign) next to it
3. Select **Project Steering Files**
4. Kiro will generate steering files at the root of the project that you can review

> **Note**: There is no dedicated "Generate Steering Documents" button. You must use the **+** icon next to AGENT STEERING & SKILLS.

## Continue the Workshop

From here, continue using the workshop instructions with this lab environment:

https://catalog.workshops.aws/kiro-immersion/en-US

