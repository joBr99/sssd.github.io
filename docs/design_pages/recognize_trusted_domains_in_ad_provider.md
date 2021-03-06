---
version: 1.10.x
---

# Recognize trusted domains in AD provider

Related tickets:

  - [RFE Recognize trusted domains in AD provider](https://github.com/SSSD/sssd/issues/1406)

## Problem Statement

With the current LDAP lookups the SSSD AD provider can only find users and groups in the local domain. With Global Catalog lookups ([Design page](global_catalog_lookups.md)) this will be extended to all users and groups of the local forest. Using the PAC helps to avoid group membership lookups ([RFE Use MS-PAC to retrieve user's group list](https://github.com/SSSD/sssd/issues/2600)).

What is missing are lookups of users and groups in trusted forests and password based authentication of users from trusted forests. For this the names of the trusted forests and additional suffixes managed by the forest are needed. The names the

## Overview view of the solution

## Implementation details

## How to test

## Author(s)

Sumit Bose \<sbose@redhat.com\>
