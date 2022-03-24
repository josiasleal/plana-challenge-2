
# iaC Challenge



## Author

- [@josiasleal](https://www.github.com/josiasleal)


# Prerequisites

- an [AWS account](https://portal.aws.amazon.com/billing/signup?nc2=h_ct&src=default&redirect_url=https%3A%2F%2Faws.amazon.com%2Fregistration-confirmation#/start) with the IAM permissions listed on the [EKS module documentation](https://github.com/terraform-aws-modules/terraform-aws-eks/blob/master/docs/iam-permissions.md)
- a configured AWS CLI
- kubectl

## Mac Install aws CLI

```
$ brew install awscli
```

After you've installed the AWS CLI, configure it by running aws configure.

When prompted, enter your AWS Access Key ID, Secret Access Key, region and output format.

```
$ aws configure
AWS Access Key ID [None]: YOUR_AWS_ACCESS_KEY_ID
AWS Secret Access Key [None]: YOUR_AWS_SECRET_ACCESS_KEY
Default region name [None]: YOUR_AWS_REGION
Default output format [None]: json
```
# Terraform

In your terminal, clone the following repository. It contains the example configuration used in this tutorial.


```bash
  $ git clone https://github.com/josiasleal/plana-challenge-2.git && cd plana-challenge-2
```


Initialize Terraform workspace
```bash
  $ terraform init
```

Run plan to see what are the resources you will be provisioning
```bash
  $ terraform plan
```

Run terraform apply if you´re satified with the plan (add the flag -auto-approve to skip the interactive approval of plan)
```bash
  $ terraform apply -auto-approve
```

Run terraform destroy to clean up your workspace
```bash
  $ terraform destroy
```

## Acknowledgements

 - [Hashcorp tutorial](https://learn.hashicorp.com/tutorials/terraform/eks#kubectl)
 - [AWS provider docs](https://registry.terraform.io/providers/hashicorp/aws/2.52.0/docs/resources/eks_cluster)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)

