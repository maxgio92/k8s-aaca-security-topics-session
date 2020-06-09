## Providers

| Name | Version |
|------|---------|
| aws | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:-----:|
| attributes | Additional attributes (e.g. `1`) | `list(string)` | `[]` | no |
| cluster\_apiserver\_allowed\_ip\_class | The IP class allowed to connect to the API server | `string` | `"0.0.0.0/0"` | no |
| cluster\_apiserver\_port | The port the API server listens on externally | `number` | `6443` | no |
| cluster\_master\_disk\_size | EBS volume size of the cluster nodes | `number` | `8` | no |
| cluster\_master\_instance\_type | EC2 instance type of the cluster nodes | `string` | `"t3.micro"` | no |
| cluster\_master\_size | Number of cluster nodes | `number` | n/a | yes |
| cluster\_ssh\_allowed\_ip\_class | The IP class allowed to connect via SSH to the cluster nodes | `string` | `"0.0.0.0/0"` | no |
| cluster\_ssh\_keypair\_public\_key\_path | The path of the public key to associate to the SSH key pair of the cluster EC2 instances | `string` | `"~/.ssh/id_rsa.pub"` | no |
| cluster\_worker\_disk\_size | EBS volume size of the cluster nodes | `number` | `8` | no |
| cluster\_worker\_instance\_type | EC2 instance type of the cluster nodes | `string` | `"t3.micro"` | no |
| cluster\_worker\_size | Number of cluster nodes | `number` | n/a | yes |
| delimiter | Delimiter to be used between `name`, `namespace`, `stage`, etc. | `string` | `"-"` | no |
| name | Solution name, e.g. 'app' or 'cluster' | `string` | n/a | yes |
| namespace | Namespace, which could be your organization name, e.g. 'eg' or 'cp' | `string` | n/a | yes |
| pod\_cidr\_block | Pod CIDR block | `string` | `"10.200.0.0/16"` | no |
| region | AWS Region | `string` | n/a | yes |
| stage | Stage, e.g. 'prod', 'staging', 'dev' or 'testing' | `string` | n/a | yes |
| tags | Additional tags (e.g. `map('BusinessUnit`,`XYZ`) | `map(string)` | `{}` | no |
| vpc\_cidr\_block | VPC CIDR block | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| cluster\_master\_nodes\_private\_dns | n/a |
| cluster\_master\_nodes\_private\_ips | n/a |
| cluster\_master\_nodes\_public\_dns | n/a |
| cluster\_master\_nodes\_public\_ips | n/a |
| cluster\_master\_size | n/a |
| cluster\_worker\_nodes\_private\_dns | n/a |
| cluster\_worker\_nodes\_private\_ips | n/a |
| cluster\_worker\_nodes\_public\_dns | n/a |
| cluster\_worker\_nodes\_public\_ips | n/a |
| cluster\_worker\_size | n/a |

