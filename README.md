# Random String, Variables & Outputs

## Overview

Terraform configuration demonstrating the usage of a terraform resource to access variables and produce outputs.
- Declares a variable for the length of the randomly generated string.
- Random String resource accesses random string length varaible.
- Outputs are generated for the Random String resource (marked sensitive).

## Deployment

### Update the randomly generated string
```
terraform apply -replace=random_string.random -auto-approve
```

### Retrieve the randomly generated string
```
terraform state show random_string.random
```