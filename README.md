# Lateral Movement and VPN Breach Response Solution Pack

## Overview

### Introduction

This article describes the Lateral Movement and VPN Breach Response Solutions Pack. The solution pack demonstrates the scenarios and use cases around lateral movement and VPN breach attacks.

This scenario generates demonstration alerts for lateral movement and VPN breach attacks using FortiDeceptor CEF data which is received from Syslog.

In such an attack technique, the attacker initially gains access to an endpoint and moves deep in the network to avoid detection. Eventually obtaining increased privileges in compromised networks and gaining access to sensitive information.

### Usage

More information about the usage of the Lateral Movement and VPN Breach Response Solution Pack [here](https://github.com/fortinet-fortisoar/solution-pack-lateral-movement-and-vpn-breach-response/blob/develop/docs/solution-pack-guide.md).

## Version Information

- Solution Pack Version: 1.0.0
- FortiSOAR™ Version Tested on: 7.2.0
- Authored By: Fortinet
- Certified: No

## Prerequisite

Ensure that the below solution packs are deployed:

**Solution Pack**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules and Action playbooks|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector| [Click here](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/README.md)|

## Contents

1. Connectors

**Solution Pack**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|Active Directory|2.2.0|[Click Here](https://docs.fortinet.com/document/fortisoar/2.2.0/active-directory/154/active-directory-v2-2-0)|
|IPFortinet FortiSIEMStack|4.3.0|[Click Here](https://docs.fortinet.com/document/fortisoar/4.3.0/fortinet-fortisiem/187/fortinet-fortisiem-v4-3-0)|

**Warning:** After deployment, this Solution Pack will install or upgrade the existing connectors, mentioned above.

2. Playbook Collection(s)

    - 02 - Use Case - Lateral Movement & VPN Breach Response 
Following is a list of playbooks under “02 - Use Case - Lateral Movement & VPN Breach Response”

    **Playbook Name**|**Description**
    | :- | :- |
    |Generate - FortiDeceptor Alerts for Lateral Movement|Generate Alert from FortiDeceptor CEF|
    |Investigate Lateral Movement & VPN Breach Detection|Investigates a FortiDeceptor Malicious IP Lateral Movement and performs containment and remediation tasks if a breach is detected.|
