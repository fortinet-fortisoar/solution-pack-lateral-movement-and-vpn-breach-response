## Release Information

- Solution Pack Version: 1.0.0
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: No

## Overview

### Introduction

**Lateral Movement and VPN Breach Response Solutions Pack** demonstrates the scenarios and use cases around lateral movement and VPN breach attacks.

Configure ingestion using a connector such as **Syslog**. The ingestion process creates alerts using FortiDeceptor CEF data (containing information such as attacker and victim IP Addresses) and manually triggers the response workflow.

In such an attack technique, the attacker initially gains access to an endpoint and moves deep in the network to avoid detection. Eventually obtaining increased privileges in compromised networks and gaining access to sensitive information.

Refer to Simulation Scenarios - 'FortiDeceptor Alert Integration with Syslog' to experience the use case without having FortiDeceptor configured.

### Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to understand how to Simulate and Reset scenarios.

This Solution Pack ships with the following simulation scenarios. 

**Scenario - FortiDeceptor Alert Integration with Syslog**

The scenario generates a demo alert of Type **Other/Unknown**

Navigate to generated alert and observe the following:

- Information such as user, source IP, destination IP is presented for analyzing the case
- FortiDeceptor information (attacker IP Address) is presented as a handy reference

**Investigate Lateral Movement & VPN Breach Detection:**

Launch the **Investigate Lateral Movement & VPN Breach Detection** playbook and observe various investigation activities such as

- Fetching asset details related to malicious IP address
- Investigation for VPN breaches and block malicious IP
- Quarantine of the malicious IP endpoint on FortiClient EMS
- Fetching compromised users' details to block them on Microsoft Active directory

## Prerequisite

Ensure that the below solution packs are deployed:

|**Solution Pack**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules and Action playbooks|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector| [Click here](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/README.md)|

## Contents

1. Connector(s)

    |**Sr. No.**|**Connector**|
    | :- | :- |
    |1|Microsoft Active Directory|
    |2|Fortinet FortiSIEM|

    **Warning:** After deployment, this Solution Pack will install or upgrade the stated connectors list.

2. Record Set(s)
    - Scenario(1): FortiDeceptor Alert Integration with Syslog
    - Assets(4)

3. Playbook Collection(s)

    - 02 - Use Case - Lateral Movement & VPN Breach Response(2):

    |**Playbook Name**|**Description**|
    | :- | :- |
    |Generate - FortiDeceptor Alerts for Lateral Movement | Generate Alert from FortiDeceptor CEF|
    |Investigate Lateral Movement & VPN Breach Detection | Investigates a FortiDeceptor Malicious IP Lateral Movement and performs containment and remediation tasks if a breach is detected.|

     **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
