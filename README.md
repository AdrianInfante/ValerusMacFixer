
### Instructions

**1. Search for Duplicate MAC Addresses in Logs**

- You no longer need to manually search the logs for duplicate MAC addresses. Simply click the button under **Step 1** to initiate a system-wide search for any duplicate MAC addresses.

**2. Populated IP Devices List**

- If duplicates are found, they will appear in a list format under the **Log Results** section.
- Only the IP addresses related to duplicate MAC address entries will be displayed for easy identification.

**3. Device Information Display**

- Click on any IP address in the **Log Results** section to view detailed information about the device, helping you resolve common issues.

  ![image](https://github.com/user-attachments/assets/3ee5fea0-1334-4933-a67b-637808378bde)

  
  The displayed information includes:
  
  - **Camera IP**: The IP address from the Log Results list.
  - **MAC Address**: The MAC address recorded in the Valerus database.
  - **ARP MAC Address**: The correct MAC address retrieved from an `ARP -a` command. If the device is offline, the address will be highlighted in red with an "offline" message.
  - **System Unique ID (SUID)**: The SUID as shown in the Valerus database.
  - 
  ![image](https://github.com/user-attachments/assets/494f6b71-61be-4881-8474-42965906c750)

**4. Fixing Duplicate Entries**

- Press the **Replace SUID** button to substitute the existing SystemUniqueID with the correct MAC address.
- Upon completion, a notification will appear in the terminal at the bottom of the screen, confirming the update.

![image](https://github.com/user-attachments/assets/b88c83a7-c48f-419a-bbd1-a36cf3f211bb)


---

### Bug Fix Notes

- **Date**: 11/7/24  
- **Issue**: *"Failed to create default config file: Access to the path 'C:\Program Files\Vicon\AppServer\AppConfig.xml' is denied."*

**Description**:  
When launching the application, an error may appear due to insufficient permissions to write in the `C:\Program Files` directory, where elevated privileges are typically required.

**Resolution**:  
To resolve this issue, run the application with Administrator privileges or configure the application to save configuration files to a location with write access.

---

### Known issues
Database error: disk I/O error
