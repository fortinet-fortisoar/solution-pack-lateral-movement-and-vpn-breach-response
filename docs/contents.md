| [Home](https://github.com/fortinet-fortisoar/solution-pack-lateral-movement-and-vpn-breach-response/blob/release/1.0.1/README.md) | 
|--------------------------------------------|

# Contents

## Connectors

|Connector|Description|
| :- | :- |
|Microsoft Active Directory| Helps directly query AD to retrieve information about users, groups, and computers, in an organization, by using the Lightweight Directory Access Protocol (LDAP)|
|Fortinet FortiSIEM| FortiSIEM provides integrations that allow you to query and make changes to the CMDB, query events, and send incident notifications.|

>**Warning:** After deployment, this Solution Pack will install or upgrade the stated connectors list.

## Record Sets

|Record Set|Description|
| :- | :- |
|Scenario|FortiDeceptor Alert Integration with Syslog|
|Assets|Four demo/example endpoints demonstrate the Lateral Movement and VPN Breach threat|

## Playbook Collection

|02 - Use Case - Lateral Movement & VPN Breach Response|
|:-|

|Playbook Name|Description|
| :- | :- |
|Generate - FortiDeceptor Alerts for Lateral Movement | Generate Alert from FortiDeceptor CEF|
|Investigate Lateral Movement & VPN Breach Detection | Investigates a FortiDeceptor Malicious IP Lateral Movement and performs containment and remediation tasks if a breach is detected.|

>**Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
