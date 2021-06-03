# Terraform EKS

```
This provider has files:       provider.tf
                           data.tf
                           eks.tf
                           variables.tf
                           terraform.auto.tfvrs
                           README.md
```

## below is terraform.auto.tfvrs file's code

```
region          = "us-east-1"
cluster_name    = "my-cluster"
cluster_version = "1.18"
instance_type   = "m4.large"
asg_max_size    = 99
asg_min_size    = 1 #min size should be 1
vpc_id          = "vpc-0bdf24213853c8b8b"
subnets = [
  "subnet-06940b50e7a1da7bb",
  "subnet-09472b4c287ef2403",
  "subnet-0a5d9c5c79ba67fa4"
]
tags = {
  Name        = "Cluster"
  Environment = "Dev"
  Team        = "DevOps"
}
```
