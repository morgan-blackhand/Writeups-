

# Lab Instructions

## Introduction
This lab involves configuring switches and routers to handle spanning tree protocol, setting up hostnames and timeouts, configuring interfaces, and setting up VLANs and DHCP pools.

## Step 1: Understand the Lab Directions
Refer to the following image to understand the directions of this lab:
![Lab Directions](https://imgur.com/a/Im6fYqI)

## Step 2: Configure Switches
First, we need to paste our configuration script into our switches so they can automatically handle spanning tree, and we can have an easier time later with hostnames and timeouts already set up.

```plaintext
conf t
vtp domain OGIT
int range fa0/11, fa0/22
switchport mode trunk
end
```

Refer to this image for detailed configuration:
![Switch Config](https://imgur.com/a/MsjoQp3)

## Step 3: Configure Interfaces
We will configure the interfaces of the switches. The Layer 2 switches use the same ports to connect, so they will use the same commands. For the Layer 3 switch, we’ll enable encapsulation and configure trunking. Also, ensure to create the required VLANs (10, 20, and 777) on each switch.

Refer to this image for VLAN creation and assignment:
![VLAN Configuration](https://imgur.com/a/vyCNy3s)

## Step 4: Setup DHCP
For the final step of setting up DHCP, we need to configure our DHCP pools and the helper addresses on the Layer 3 router.

Refer to this image for DHCP configuration:
![DHCP Configuration](https://imgur.com/a/plTyt1e)

---

This markdown write-up provides a structured and clear guide for configuring the lab setup.
