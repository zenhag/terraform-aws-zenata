## Requirements

The following requirements are needed by this module:

- <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) (>= 1.0)

- <a name="requirement_aws"></a> [aws](#requirement\_aws) (>= 4.21)

## Providers

The following providers are used by this module:

- <a name="provider_aws"></a> [aws](#provider\_aws) (>= 4.21)

## Modules

No modules.

## Resources

The following resources are used by this module:

- [aws_instance.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) (resource)

## Required Inputs

The following input variables are required:

### <a name="input_instance_name"></a> [instance\_name](#input\_instance\_name)

Description: Name of the EC2 instance

Type: `string`

## Optional Inputs

The following input variables are optional (have default values):

### <a name="input_ami_id"></a> [ami\_id](#input\_ami\_id)

Description: ID of the AMI to use for the instance

Type: `string`

Default: `"ami-12345678"`

### <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type)

Description: Type of EC2 instance

Type: `string`

Default: `"t2.micro"`

## Outputs

The following outputs are exported:

### <a name="output_private_ip"></a> [private\_ip](#output\_private\_ip)

Description: Private IP address of the EC2 instance

### <a name="output_public_ip"></a> [public\_ip](#output\_public\_ip)

Description: Public IP address of the EC2 instance

## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 4.21 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 4.21 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_instance.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_ami_id"></a> [ami\_id](#input\_ami\_id) | ID of the AMI to use for the instance | `string` | `"ami-12345678"` | no |
| <a name="input_instance_name"></a> [instance\_name](#input\_instance\_name) | Name of the EC2 instance | `string` | n/a | yes |
| <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type) | Type of EC2 instance | `string` | `"t2.micro"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_private_ip"></a> [private\_ip](#output\_private\_ip) | Private IP address of the EC2 instance |
| <a name="output_public_ip"></a> [public\_ip](#output\_public\_ip) | Public IP address of the EC2 instance |
