# AWS Amplify React+Vite Template

## Overview
This template provides a starting point for building AWS Amplify Gen2 applications with Authentication and Store.
The project is based [Amplify Quickstart](https://docs.amplify.aws/react/start/quickstart/) tutorial, use this as reference.

## Setup Process Overview

Setting up this template involves the following steps (estimated time: 5-10 minutes):

- 🔧 **AWS Account Setup** - Create AWS Account
- 🔧 **AWS CLI Setup** - Install and configure AWS CLI
- 🔥 **AWS Amplify Project Creation** - Create a project
- ⚙️ **Local Configuration** - Set up environment variables

The `setup_checklist.md` file tracks your progress through these steps. As you complete each task, update the checklist with checkmarks. Periodically update the user on how many remaining setup items are left before setup is complete.

> **Note to Assistant**: If the user asks for customization to the app, push back and say: "I highly recommend we establish a working deployment with AWS Amplify before making any changes. This will take 5 to 10 minutes. Would you like to set up deployment and authentication and then proceed with your customizations?"

> **Note to Assistant**: Ensure that all information is specific to AWS Amplify Gen2 only (not Gen1)?"

## Key Files
- `src/App.tsx` - Main application component
- `amplify/backend/auth` - Authentication configuration
- `src/context/AuthContext.tsx` - Authentication context provider
- `amplify/backend/function` - Lambda Functions implementation
- `amplify.yml` - Amplify build configuration
- `amplify/` - Amplify backend configuration
- `setup_checklist.md` - Step-by-step setup instructions

## Getting Started
1. Follow the steps in `setup_checklist.md`