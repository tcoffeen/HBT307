# Linux Demo x

## Enabling DHCP(v6) lease scavenging

> Free and backup DHCP and DHCPv6 leases will remain in the database unless **lease scavenging** is enabled. It is disabled by default but can be activated for DHCP and DHCPv6 selectively as desired.

1. Login to the web UI. 

![NIOS Web UI Login](../images/NIOS_webUI_login_2.png)

2. To view expired leases, navigate from the dashboard to *Data Management -> IPAM* then click on an IPv6 prefix that has been configured for DHCPv6.

![NIOS Web UI Lease Scavenging 1](../images/NIOS_webUI_lease_scavenging1.png)

3. Observe the list of available and expired leases for the prefix.

![NIOS Web UI Lease Scavenging 2](../images/NIOS_webUI_lease_scavenging2.png)

4. Next, navigate to *Grid -> Grid Management -> DHCP -> Members*, click the checkbox to select the grid member then select **Edit** in the toolbar.

![NIOS Web UI Lease Scavenging 3](../images/NIOS_webUI_lease_scavenging3.png)

1. Verify that the configuration screen is for Infoblox (Grid DHCP Properties) then make sure *General* and *Advanced* are selected. Scroll down to *IPv6 Properties* and choose the lease scavenging duration (minimum of 6 hours) that fits the overall DHCPv6 operational model Click *Save & Close* and restart grid services.

![NIOS Web UI Lease Scavenging 4](../images/NIOS_webUI_lease_scavenging4.png)
