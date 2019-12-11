# nsxt-terraform-three-tier-app

This repo contains a demostration of combining NSX-T Terraform provider and vSphere Terraform provider in order to create fully secured three tier application.
It creates NSX-T T1 router, web, app, and db logical switches. The web LS uses a routable subnet and the other two private subnets. We can access them using NAT configures by Terraform.
It also creates different security components like Groups based on VM tags, FW Section with multiple FW rules.

I changged this to remove the VM deployment and to work with:
  Terraform v0.12.17
  + provider.nsxt v1.1.2

https://www.terraform.io/docs/providers/nsxt/
