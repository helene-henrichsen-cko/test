## Providers

The following providers are used by this module:

- aws

## Required Inputs

The following input variables are required:

### name

Description: The name of the ALB.

Type: `string`

### subnet\_ids

Description: A list of the subnets into which the ALB will place its underlying nodes. Include one subnet per Availability Zone. If the ALB is public-facing, these should be public subnets. Otherwise, they should be private subnets.

Type: `list(string)`

### vpc\_id

Description: The VPC in which this ALB will be placed.

Type: `string`

## Optional Inputs

The following input variables are optional (have default values):

### idle\_timeout

Description: The time in seconds that the client TCP connection to the ALB is allowed to be idle before the ALB closes the TCP connection.

Type: `number`

Default: `60`

### tags

Description: A map of custom tags to apply to the ALB and its Security Group. The key is the tag name and the value is the tag value.

Type: `map(string)`

Default: `{}`

## Outputs

The following outputs are exported:

### alb\_arn

Description: n/a

### target\_group\_arn

Description: n/a
