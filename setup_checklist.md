# AWS Amplify React+Vite Setup Checklist

Follow these steps to set up your AWS Amplify web application

## 1. AWS Account Setup
- [ ] Check if user has AWS Account and if not ask `user` to [Create AWS Account](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html)
- [ ] Check if AWS CLI is available `aws --version` and if not install AWS CLI: `brew install awscli` or follow instructions [here](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) for your operating system

## 2. AWS Amplify Setup
- [ ] Ask `user` to setup new github repo
- [ ] Push current repo to that remote
- [ ] Ask `user` to open [this](https://eu-west-2.console.aws.amazon.com/amplify/create/add-repo) page to setup AWS Amplify with the new github repository
- [ ] After deployment is completed ask `user` to download `amplify_outputs.json` to local repository from 'Deployments / Deployed backend resources' page. Click on Deployment to get to that screen.

## 3. Configure Sandbox for local development
- [ ] Check if user has default AWS profile setup in `~/.aws/config` if no follow the instructions below
- [ ] Follow the instructions in [this]((https://docs.amplify.aws/react/start/account-setup/)) guide 1 step at a time asking `user` to complete each step
- [ ] Set up Identity Center
- [ ] Create user with Amplify permissions
- [ ] Create password for user
- [ ] Set up local AWS profile
    Use this info to guide user how to fill in the required information in this step
     | Choose Enable with AWS Organizations
     | SSO session name (Recommended): amplify-admin
     | SSO start URL: <START SESSION URL> - take this from `IAM Identity Center page` (eg: https://<your-company>.awsapps.com/start), can be renamed to user specific domain
     | SSO region: <your-region> - User AWS account region
     | SSO registration scopes [sso:account:access]: <leave blank>
     | Default client Region [us-east-1]: - User AWS account region
     | CLI default output format (json if not specified) [json]: <leave blank>
     | Profile name [amplify-policy-<your-account>]: - IMPORTANT to use `default` as profile name
- [ ] Bootstrap your AWS account. Ask user to run `npx ampx sandbox` and confirm all is good.

## 4. Local Development
- [ ] Ensure Node.js v22 is installed
- [ ] Start AWS Amplify backend sandbox using interactive terminal `npx ampx sandbox`
- [ ] Start development frontend application using interactive terminal `npm run dev`
- [ ] Test the application at http://localhost:5173

## 5. Deployment
- [ ] Push changes to github remote repository

## 6. Production Considerations
- [ ] Set up a custom domain (if needed)