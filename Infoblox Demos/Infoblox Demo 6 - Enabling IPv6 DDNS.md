# Linux Demo 6

## Enabling IPv6 DDNS

1. Login to the web UI. 

![NIOS Web UI Login](../images/NIOS_webUI_login_2.png)

2. Navigate to *Data Management -> DNS -> Zones (default)* and observe the configured zones.

![NIOS Web UI Data Management DNS Zones](../images/NIOS_webUI_data_mgmt_DNS_zones.png)

3. Select the zone that DDNS updates will apply to. In this example, the authoritative **hexabuild.net** zone is selected by clicking on the hexabuild.net link from the list of zones.

![NIOS Web UI Data Management DNS Zone hexabuild.net](../images/NIOS_webUI_data_mgmt_DNS_zones_hb-net.png)

4. Observe the list of resource records of differing types for the selected zone. Note that none of the records are marked *Dynamic*, indicating that DDNS is likely not enabled for either IPv6 or IPv4.

![NIOS Web UI Data Management DNS Zone hexabuild.net Records](../images/NIOS_webUI_data_mgmt_DNS_zones_hb-net_records.png)

5. Navigate to the *DHCP* tab under *Data Management* and click *Grid DHCP Properties* in the toolbar.

![NIOS Web UI Data Management DHCP Grid Properties](../images/NIOS_webUI_data_mgmt_DHCP_grid_prop.png)

6. On the *Grid DHCP Properties* panel that appears, select *IPv6 DDNS* from the left-hand column. Next, check the box to enable *DDNS Updates* and enter the *DDNS Domain Name* (in this example, **hexabuild.net**). Change the *DDNS Update Method* to **Standard** and near the bottom check the *Lease Renewal Update* box. Click **Save & Close**.

![NIOS Web UI Data Management DHCP Grid Properties IPv6 DDNS](../images/NIOS_webUI_data_mgmt_DHCP_grid_prop_v6_DDNS.png)

7. Restart the service.

![NIOS Web UI Services Restart](../images/NIOS_webUI_services_restart.png)

