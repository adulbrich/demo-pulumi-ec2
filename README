# Pulumi EC2 Webserver Demo

This repository is based on the following tutorial: https://www.pulumi.com/templates/virtual-machine/aws/

Make sure Pulumi is installed/up-to-date on your system.

```
brew install pulumi
brew update && brew upgrade pulumi
```

Pulumi can run using many programming languages. Here we chose Typescript.

As this is a Node-based project, you need `node` and `npm` installed as well. We recommend using `nvm` to manage your node installation, see https://github.com/nvm-sh/nvm.

Once `node`/`nvm` is installed, run:

```
npm install
```

It will install dependencies in `package.json`, including the core Pulumi package, and the AWS extension.

Before proceeding, you'll need to configure your AWS credentials.

In your AWS Academy Learner Lab, start your lab, click "AWS Details", and finally "Show" for the AWS CLI. Copy the credentials to `~/.aws/credentials`.

Now you can run:

```
pulumi up
```

Let Pulumi do its thing and approve the creation of resources if everything looks good.

You can select your stack with `pulumi stack select <your_stack>` and query the outputs using `pulumi stack output <output_variable>` for example.

In our case, we can open the deployed web page using:

```
pulumi stack select dev
open $(pulumi stack output url)
```

Once you're done, we can take down everything with:

```
pulumi destroy
```