# Testing Terraform Code

## TFLint und Rule Sets

```bash
# see https://github.com/terraform-linters/tflint
# see https://github.com/terraform-linters/tflint-ruleset-aws

$ cd aws
$ terraform init
$ terraform plan

$ tflint
```

## Checkov

```bash
# see https://github.com/bridgecrewio/checkov

$ checkov --directory aws
```

## Snyk

```bash
# Installation and usage instructions
# https://docs.snyk.io/snyk-cli/install-the-snyk-cli

$ cd aws
$ snyk iac test main.tf
```

## Terratest

```bash
# see https://terratest.gruntwork.io/docs/getting-started/quick-start/#example-1-terraform-hello-world
$ cd basic && go test

# see https://terratest.gruntwork.io/docs/getting-started/quick-start/#example-2-terraform-and-aws
$ cd aws && go test
```
