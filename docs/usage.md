| [Home](https://github.com/fortinet-fortisoar/solution-pack-lateral-movement-and-vpn-breach-response/blob/release/1.0.1/README.md) | 
|--------------------------------------------|

# Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/usage.md) to understand how to simulate and reset scenarios. 
 
To understand the process FortiSOAR follows to respond to Lateral Movement and VPN Breach threats, we have included a scenario &ndash; **FortiDeceptor Alert Integration with Syslog** &ndash; with this solution pack. Refer to the section *FortiDeceptor Alert Integration with Syslog* to understand how this solution pack's automation addresses your needs. 

## FortiDeceptor Alert Integration with Syslog Scenario

This scenario generates an example alert of Type *Other/Unknown* in FortiSOAR's **Alerts** module.

Navigate to the demo alert and note the following:

- The demo alerts created are an example of a data ingestion that used FortiDeceptor CEF data
- The alert is of type *Other/Unknown*
- The reported alert contains the following among other related sources data:
    - user
    - source IP
    - destination IP
    - FortiDeceptor information containing attacker IP Address

Users can launch the **Investigate Lateral Movement & VPN Breach Detection** playbook. These playbooks perform th following automated tasks:

- Fetch asset details related to the malicious IP address
- Investigate VPN breaches and block malicious IP
- Quarantine the malicious IP endpoint on FortiClient EMS
- Fetch compromised users' details to block them on Microsoft Active directory
