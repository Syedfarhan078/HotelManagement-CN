# HotelManagement-CN
A hotel management network simulation designed in Cisco Packet Tracer to demonstrate VLAN segmentation, router interconnection, and secure departmental communication across multiple floors.



 🏨 Hotel Management Network (Cisco Packet Tracer)

 🧩 Problem Statement

You are required to design and implement a **Modern Hotel Network** using Cisco Packet Tracer.

The hotel has **three floors**, and each floor hosts specific departments as described below:

### Floor Distribution

- **1st Floor:**
  - Reception — VLAN 80, Network: 192.168.8.0/24  
  - Store — VLAN 70, Network: 192.168.7.0/24  
  - Logistics — VLAN 60, Network: 192.168.6.0/24  

- **2nd Floor:**
  - Finance — VLAN 50, Network: 192.168.5.0/24  
  - HR — VLAN 40, Network: 192.168.4.0/24  
  - Sales/Marketing — VLAN 30, Network: 192.168.3.0/24  

- **3rd Floor:**
  - Admin — VLAN 20, Network: 192.168.2.0/24  
  - IT — VLAN 10, Network: 192.168.1.0/24  

---

### Network Design Requirements

1. There should be **three routers** connecting each floor (all placed in the server room in the IT department).  
2. All routers must be interconnected using **serial DCE cables**.  
3. The **network between routers** should use:
   - 10.10.10.0/30  
   - 10.10.10.4/30  
   - 10.10.10.8/30  
4. Each floor must have **one switch**, located on that floor.  
5. Each floor must include **Wi-Fi networks** connected to laptops and smartphones.  
6. Every department must have **a dedicated printer**.  
7. Each department should belong to a **unique VLAN** as listed above.  
8. Use **OSPF (Open Shortest Path First)** as the **routing protocol** to advertise all routes.  
9. All devices in the network must **obtain IP addresses dynamically**, with their respective routers configured as **DHCP servers**.  
10. Ensure **full communication** between all devices across all floors.  
11. Configure **SSH** on all routers for **remote login**.  
12. In the **IT department**, add a **PC called Test-PC** to port `fa0/1` and use it for testing SSH access.  
13. Configure **port security** on the IT department switch:
    - Allow **only Test-PC** to access port `fa0/1`.  
    - Use the **sticky method** to learn its MAC address.  
    - Set **violation mode** to `shutdown`.

---

Network Topology Created
The network topology below satisfy the user requirements above and everything is verified, tested and working fine.
<img width="1882" height="876" alt="Network Implementation Image" src="https://github.com/user-attachments/assets/66ef70f9-0fb0-403a-88da-0ad0ca84bec7" />


> 💡 **Note:** The above configuration ensures a realistic, secure, and scalable enterprise-level network simulation for a hotel environment.  
> Designed using Cisco Packet Tracer version 8.2 or later.


🧑‍💻 Author

Syed Farhan
🎓 B.Tech in AI & ML — Atria Institute of Technology
📧 LinkedIn — https://www.linkedin.com/in/syed-farhan-581b83314/
