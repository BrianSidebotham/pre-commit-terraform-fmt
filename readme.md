# Terraform fmt Pre-Commit Hook

An example bash pre-commit hook to use `terraform fmt` on commit.

To get started using the pre-commit hook, first install https://pre-commit.com

Then, create a pre-commit config file in your repository:

```yaml
repos:
  - repo: https://github.com/BrianSidebotham/pre-commit-terraform-fmt.git
    rev: v1.0.0
    hooks:
      - id: terraform-fmt
```

Then run a commit and any changed terraform files (`*.tf` and `*.tfvars`) will be formatted by Terraform.

>**NOTE:** You must have the terraform binary available in your environment for this to work.
