## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.13.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_google"></a> [google](#provider\_google) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [google_compute_firewall.firewall](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_firewall) | resource |
| [google_compute_network.vpc_network](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_network) | resource |
| [google_compute_subnetwork.subnetworks](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_subnetwork) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_firewall_allow_tcp_ports"></a> [firewall\_allow\_tcp\_ports](#input\_firewall\_allow\_tcp\_ports) | Lista do objeto de firewall | `list` | `[]` | no |
| <a name="input_firewall_allow_udp_ports"></a> [firewall\_allow\_udp\_ports](#input\_firewall\_allow\_udp\_ports) | Lista do objeto de firewall | `list` | `[]` | no |
| <a name="input_firewall_name"></a> [firewall\_name](#input\_firewall\_name) | n/a | `string` | `""` | no |
| <a name="input_project"></a> [project](#input\_project) | nome do projeto existente no google cloud | `string` | `""` | no |
| <a name="input_subnetworks"></a> [subnetworks](#input\_subnetworks) | Lista do objeto de network | <pre>list(object({<br>    name          = string<br>    ip_cidr_range = string<br>    region        = string<br>  }))</pre> | n/a | yes |
| <a name="input_vpc_name"></a> [vpc\_name](#input\_vpc\_name) | nome da vpc | `string` | `""` | no |

## Outputs

No outputs.
