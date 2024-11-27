
This repository contains the k8s yaml configuration files used for validaiton activities performed with cSRX (21.1R3.11 & 24.2R1.17) on Suse Rancher RKE2 (v1.30.5+rke2r1).

The objectives of this validation is to confirm the expected behavior of basic NGFW features delivered by the Juniper cSRX VNF on Suse Rancher KE2.
The L3/L4 Firewall rules are configured on the cSRX that acts as the default gateway for 2 ubuntu pods located on different vnets (network-attachment-definition used macvlan in the scenario).

The folder 21.1/ contains all yaml files for cSRX junos 21.1R3.11 release

The folder 24.2/ contains all yaml files for cSRX junos 24.2R1.17 release

How to deploy:

kubectl create namespace csrx

kubectl create -f cm.yaml

kubectl create -f nad.yaml

kubectl create -f private-pod.yaml

kubectl create -f public-pod.yaml

kubectl create -f csrx.yaml
 
