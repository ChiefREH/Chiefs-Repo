# SET A MANUAL IP ADDRESS IN RASPBERRY PI OS

## Applies to:
Raspberry Pi OS (Desktop version)

---

## 1. Open Network Settings

- Click the network icon in the top-right corner of the desktop panel.
- Select **Advanced Options**
- Click **Edit Connections…**

---

## 2. Select Your Connection

- Choose:
  - **Wired connection 1** (for Ethernet), or
  - Your Wi-Fi network name
- Click **Settings** (or **Edit**)

---

## 3. Configure IPv4 Settings

- Select the **IPv4 Settings** tab.
- Change **Method** from:

  Automatic (DHCP)

  to:

  **Manual**

---

## 4. Enter Static IP Information

Click **Add**, then enter:

- Address: 192.168.1.your_IP_address
- Netmask: 255.255.255.0
- Gateway: 192.168.1.1

In the **DNS servers** field, enter:

  192.168.1.1, 8.8.8.8

---

## 5. Save and Reconnect

- Click **Save**
- Disable and re-enable the network connection  
  OR reboot:

>**sudo reboot**

---

## 6. Verify the IP Address

Open a terminal and type:

>hostname -I

You should now see your assigned static IP address.

---

## Important Notes

- The IP address must:
  - Be on the same subnet as your router
  - Be outside the router’s DHCP range
  - Not already be assigned to another device