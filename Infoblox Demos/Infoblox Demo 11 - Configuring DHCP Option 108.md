# Linux Demo 11

## Configuring DHCP Option 108 to Support IPv6-Mostly

1. After logging in to the UI, navigate to *Data Management -> DHCP -> DHCP Options* then select the checkbox for **DHCP** and click the pencil/edit icon.

![NIOS Web UI Data Management DHCP Option Spaces](../images/NIOS_webUI_data_mgmt_DHCP_options.png)

2. The **DHCP (Option Space)** configuration panel appears. Click the plus sign next to options to add a new DHCP option.

![NIOS Web UI Data Management DHCP Option Spaces 2](../images/NIOS_webUI_data_mgmt_DHCP_options2.png)

3. Scroll to the bottom of the list of options where a new blank one should appear. Click in the area under the **Name** column heading and enter a descriptive name. In this example, *ipv6-mostly* is entered.

![NIOS Web UI Data Management DHCP Option Spaces 3](../images/NIOS_webUI_data_mgmt_DHCP_options3.png)

4. Next, click in the area under the **Code** column heading and enter a value. In this example, *108* for DHCP Option 108.

![NIOS Web UI Data Management DHCP Option Spaces 4](../images/NIOS_webUI_data_mgmt_DHCP_options4.png)

5. Next, click in the area under the **Type** column heading and select a value from the pull-down menu. In this example, *32-bit Unsigned Integer* is selected

![NIOS Web UI Data Management DHCP Option Spaces 5](../images/NIOS_webUI_data_mgmt_DHCP_options5.png)

6. Verify that the new option has all the correct values then click **Save & Close**.

![NIOS Web UI Data Management DHCP Option Spaces 6](../images/NIOS_webUI_data_mgmt_DHCP_options6.png)

7. Next click on **Grid DHCP Properties** in the toolbar.
   
![NIOS Web UI Data Management DHCP Option Spaces 7](../images/NIOS_webUI_data_mgmt_DHCP_options7.png)

8. On the **(Infoblox) Grid DHCP Properties** configuration panel that appears, select **IPv4 DHCP Options** in the left column, then scroll down to the **Custom DHCP Options** item.
   
![NIOS Web UI Data Management DHCP Option Spaces 8](../images/NIOS_webUI_grid_DHCP_prop.png.png)

