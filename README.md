# terraform-aws-tardigrade-iam-account

Terraform module to manage AWS account password policy

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| account\_alias | Name of the IAM account alias | string | `""` | no |
| allow\_users\_to\_change\_password | Whether to allow users to change their own password | bool | `"true"` | no |
| create\_iam\_account | Controls whether to configure the IAM account settings | bool | `"true"` | no |
| hard\_expiry | Whether users are prevented from setting a new password after their password has expired (i.e. require administrator reset) | bool | `"false"` | no |
| max\_password\_age | The number of days that an user password is valid | string | `"90"` | no |
| minimum\_password\_length | Minimum length to require for user passwords | string | `"14"` | no |
| password\_reuse\_prevention | The number of previous passwords that users are prevented from reusing | string | `"24"` | no |
| require\_lowercase\_characters | Whether to require lowercase characters for user passwords | bool | `"true"` | no |
| require\_numbers | Whether to require numbers for user passwords | bool | `"true"` | no |
| require\_symbols | Whether to require symbols for user passwords | bool | `"true"` | no |
| require\_uppercase\_characters | Whether to require uppercase characters for user passwords | bool | `"true"` | no |

