
# Instructions


**1. Search for Duplicate MAC Addresses in Logs**

- You no longer need to manually search the logs for duplicate MAC addresses. Simply click the button under **Step 1** to initiate a system-wide search for any duplicate MAC addresses.

**2. Populated IP Devices List**

- If duplicates are found, they will appear in a list format under the **Log Results** section.
- Only the IP addresses related to duplicate MAC address entries will be displayed for easy identification.

**3. Device Information Display**

- Click on any IP address in the **Log Results** section to view detailed information about the device, helping you resolve common issues.



<p align="center">
  <img src="https://github.com/user-attachments/assets/3ee5fea0-1334-4933-a67b-637808378bde" alt="image">
</p>


  The displayed information includes:
  
  - **Camera IP**: The IP address from the Log Results list.
  - **MAC Address**: The MAC address recorded in the Valerus database.
  - **ARP MAC Address**: The correct MAC address retrieved from an `ARP -a` command. If the device is offline, the address will be highlighted in red with an "offline" message.
  - **System Unique ID (SUID)**: The SUID as shown in the Valerus database.


<p align="center">
  <img src="https://github.com/user-attachments/assets/494f6b71-61be-4881-8474-42965906c750" alt="image">
</p>


**4. Fixing Duplicate Entries**

- Press the **Replace SUID** button to substitute the existing SystemUniqueID with the correct MAC address.
- Upon completion, a notification will appear in the terminal at the bottom of the screen, confirming the update.



<p align="center">
  <img src="https://github.com/user-attachments/assets/b88c83a7-c48f-419a-bbd1-a36cf3f211bb" alt="image">
</p>


# Changes

**v1.1**
---
- Fixed the error *"Failed to create default config file: Access to the path 'C:\Program Files\Vicon\AppServer\AppConfig.xml' is denied."*
- Arp Mac address textbox is updating the background color properly

**v1.2**
---
- Minor design modification in the debug terminal for clear reading
- AppConfig.xml file now is located in the app folder

**v1.3**
---
- Now the SUID will update when the conditions were: Arp result was offline and the MAC was different
- Arp box showing now "OFFLINE" instead of "device offline"


