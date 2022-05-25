# Terraform fmt Pre-Commit Hook

An example bash pre-commit hook to use `terraform fmt` on commit.

To get started using the pre-commit hook, first install https://pre-commit.com

Then, create a pre-commit config file in your repository:

```yaml
repos:
  - repo: ../pre-commit-terraform-fmt
    rev: 7e82c01e36b35da05d959286542e5352f70dd530
    hooks:
      - id: terraform-fmt
```

Then run a commit and any changed terraform files (`*.tf` and `*.tfvars`) will be formatted by Terraform.

>**NOTE:** You must have the terraform binary available in your environment for this to work.
