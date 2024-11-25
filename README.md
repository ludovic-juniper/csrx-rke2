
This repository contains the k8s yaml configuration files use dfor validaiton activities performed with cSRX (21.1R3.11) on Suse Rancher RKE2 (v1.30.5+rke2r1).

The objectives of this validation is to confirm the expected behavior of basic NGFW features delivered by the Juniper cSRX VNF on Suse Rancher KE2.
The L3/L4 Firewall rules are configured on the cSRX that acts as the default gateway for 2 ubuntu pods located on different vnets (network-attachment-definition used macvlan in the scenario).
