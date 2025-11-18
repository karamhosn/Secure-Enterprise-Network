# Secure Enterprise Network Design and Implementation

## Author

- Full Name: Karam Aboul-Hosn

## Introduction

This repository contains all of the files and documentation for the design and implementation of a secure enterprise network. 

Under the `docs/` folder, you will find a `.pdf` file containing the project description and an overview of the features implemented for this meticulously planned system. You will also find another `.pdf` file containing addressing tables for this particular network design.

## How To Open The Project

Under the `packet.tracer/` folder, find and download the `.pkt` file and open it using Cisco Packet Tracer version 9.0.0.

## Configuration and Verification Files

Under the `configs/` folder, you will find `.txt` files where I have included some configuration and verification IOS commands specific to each step taken during the project implementation. 

Note that all of the devices in the `.pkt` file are *already* configured properly. The inclusion of configuration details is *strictly* for documentation purposes, as some key configurations for re-implementation are purposely not included. 

## Network Topology

Under the `images/` folder, you will find a `.png` file containing the network topology diagram.

## Exceptions

The DMZ has a single point of failure since it's designated L2 switch is only connected to one Cisco ASA Firewall. Implementing redundancy would require the utilization of both Cisco ASA Firewalls, which is not included in this particular network design. 

The firewall ACLs are configured to only allow HTTP web traffic, DNS, and ICMP with the appropriate security zones and levels. When it comes to the firewalls, part of this lab's educational focus was on *how* to configure firewall ACLs, rather than taking the time to fully configure them. It is understood that HTTP provides insecure web-communication as compared to its HTTPS counterpart.

Simple passwords that use common words or phrases and that lack complexity are used in this demo for routers, switches, WiFi networks, and accounts. This is for demo purposes only; in a real-world environment, strong passwords should be used and enforced through a rigorous password policy.
