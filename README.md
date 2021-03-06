
## Deploying the infrastructure using Terraform:

1. Terraform init 
```
$ terraform init
```
2. Terraform plan
```
$ terraform plan
```
3. Terraform apply
```
$ terraform apply
```

## azure-fortigate-vpn

#### Topology
![alt text](https://github.com/Dinoyan/azure-terraform/blob/main/Design.png?raw=true)

IP Table

|     Azure     |       IP      |
| ------------- | ------------- |
|   Main-Vnet   | 10.10.0.0 / 24|
|   GW-Subnet   | 10.10.0.0 / 27|

On-Prem
|     On-Prem      |       IP      |
| -------------    | ------------- |
|   Fortigate WAN  |     x.x.x.x   |
|   Fortigate Local| 10.10.0.1 /24|
|   Windows VM     | 10.10.0.2 /24|

Fortigate VM and Windows VM are on a single LAN segment


## Hub-Spoke
#### Topology
![alt text](https://github.com/Dinoyan/azure-terraform/blob/main/Hub-spoke%20network/hub-spoke.png?raw=true)



