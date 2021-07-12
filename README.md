## AWS CloudFormation 101 - Workshop

[![Website cfn101.workshop.aws](https://img.shields.io/website-up-down-green-red/http/cfn101.workshop.aws.svg)](https://cfn101.workshop.aws/)

## Workshop site

Go to [https://cfn101.workshop.aws](https://cfn101.workshop.aws/) to start a workshop.

## Developer Guide

This workshop is built with markdown as a static HTML site using [hugo](http://gohugo.io).

To install hugo, use your operating system's package manager (e.g. `brew install hugo`) or follow [the instructions on the hugo website](https://gohugo.io/getting-started/installing).

You'll find the content of the workshop in the [workshop](./workshop) directory.

Lab resources can be found in the [code](code) directory.

You will need to bring in the project's requirements using git submodules:

```bash
git submodule init
git submodule update
```

You can start up a local development server by running:

```bash
cd workshop
hugo serve
```

Once the server is running, you can open <http://localhost:1313> in your browser.

## Website Infrastructure

The workshop is available at https://cfn101.workshop.aws. It's a static website
hosted via [AWS Amplify](https://aws.amazon.com/amplify/).

The infrastructure is deployed using [AWS CloudFormation](https://aws.amazon.com/cloudformation/). The CloudFormation template is in the [infrastructure](./infrastructure) directory.

To deploy the workshop into your own account, you need to create an environment file and run the script:

```bash
cd infrastructure/

# Create an `.env` file and populate it with your own values
cp .env.example .env

# run the deployment script
./deploy.sh
```

## License

This library is licensed under the MIT-0 License. See the LICENSE file.


## Labs 

#### WORKSHOP PART 01
- [Workshop Part 01](/workshop/content/30-workshop-part-01/_index.md)
- [CloudFormation Fundamentals](/workshop/content/30-workshop-part-01/10-cloudformation-fundamentals/_index.md)
- [Template Anatomy](/workshop/content/30-workshop-part-01/10-cloudformation-fundamentals/100-template-anatomy/_index.md)
- [Lab 01: Template and Stack](/workshop/content/30-workshop-part-01/10-cloudformation-fundamentals/200-lab-01-stack/_index.md)
- [CloudFormation Features](/workshop/content/30-workshop-part-01/20-cloudformation-features/_index.md)
- [Lab 02: Resources](/workshop/content/30-workshop-part-01/20-cloudformation-features/100-lab-02-resources/_index.md)
- [Lab 03: Intrinsic Functions](/workshop/content/30-workshop-part-01/20-cloudformation-features/200-lab-03-functions/_index.md)
- [Lab 04: Mapping](/workshop/content/30-workshop-part-01/20-cloudformation-features/300-lab-04-mappings/_index.md)
- [Lab 05: Outputs](/workshop/content/30-workshop-part-01/20-cloudformation-features/400-lab-05-outputs/_index.md)
- [Launching an EC2 Instance](/workshop/content/30-workshop-part-01/30-launching-ec2/_index.md)
- [Lab 06: Multi Region Latest AMI](/workshop/content/30-workshop-part-01/30-launching-ec2/100-lab-06-ami/_index.md)
- [Lab 07: SSM - Session Manager](/workshop/content/30-workshop-part-01/30-launching-ec2/200-lab-07-session-manager/_index.md)
- [Lab 08: User Data](/workshop/content/30-workshop-part-01/30-launching-ec2/300-lab-08-user-data/_index.md)
- [Lab 09: Helper Scripts](/workshop/content/30-workshop-part-01/30-launching-ec2/400-lab-09-helper-scripts/_index.md)

#### Workshop Part 02
- [Workshop Part 02](/workshop/content/40-workshop-part-02/_index.md)
- [Nested Stacks](/workshop/content/40-workshop-part-02/10-nested-stacks/100-lab-10-nested-stacks/_index.md)
- [Lab 10: Nested Stacks](/workshop/content/40-workshop-part-02/10-nested-stacks/_index.md)
- [Layered Stack](/workshop/content/40-workshop-part-02/20-layered-stack/_index.md)
- [Lab 11: Layered Stack](/workshop/content/40-workshop-part-02/20-layered-stack/100-lab-11-layered-stack/_index.md)
- [Package and Deploy](/workshop/content/40-workshop-part-02/30-package-and-deploy/_index.md)
- [Lab 12: Package and Deploy](/workshop/content/40-workshop-part-02/../50-next-steps/_index.md)