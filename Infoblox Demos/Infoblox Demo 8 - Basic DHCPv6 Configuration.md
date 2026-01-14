# Infoblox Demo 8

## Basic DHCPv6 Configuration

1. Login to the web UI. 

![NIOS Web UI Login](../images/NIOS_webUI_login_2.png)

2. Select **Grid**.

![NIOS Web UI Dashboard](../images/NIOS_webUI_dashboard_grid.png)

3. Select **Grid Manager**, make sure **DHCP** is selected and under **Services** check the box next to the grid member name (in this example `infoblox.hexabuild.net`). Click on the pencil icon to edit the DHCP settings.

![NIOS Web UI Grid Manager Services DHCP](../images/NIOS_webUI_grid_mgr_serv_DHCP.png)

4. The **Member DHCP Properties** screen appears. Verify that on the **General** tab, IPv6 (along with IPv4) is enabled for the LAN1 interface.

![NIOS Web UI Grid Manager Services DNS Properties](../images/NIOS_webUI_grid_mgr_serv_DHCP_prop.png)

5. If any changes were made, click **Save & Close**.