| [Home](https://github.com/fortinet-fortisoar/solution-pack-lateral-movement-and-vpn-breach-response/blob/release/1.0.1/README.md) | 
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.    
2. From the list of solution pack that appears, search for and select **Lateral Movement and VPN Breach Response**. 
3. Click the **Lateral Movement and VPN Breach Response** solution pack card.    
4. Click the **Install** button on the bottom to begin installation.

## Prerequisite

The **Lateral Movement and VPN Breach Response** solution pack depends on the following solution packs. 

|**Solution Pack**|**Purpose**|
| :- | :- |
|SOAR Framework|Required for Incident Response modules and Action playbooks|
|SOC Simulator|Required for Scenario Module and SOC Simulator connector|ß

# Configuration

For optimal performance of **Lateral Movement and VPN Breach Response** solution pack, install and configure a data ingestion process from a data source and convert them into actionable items, such as alerts, in FortiSOAR.
- To configure and use the Syslog connector for data ingestion, refer to [Configuring Syslog Connector](https://docs.fortinet.com/document/fortisoar/1.1.1/syslog/1/syslog-v1-1-1#Configuration_parameters).

The ingestion process creates alerts using FortiDeceptor CEF data &ndash; containing information such as attacker and victim IP Addresses &ndash; and manually triggers the response workflow.
