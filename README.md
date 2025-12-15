# CCNA Study Notes — Questions 1–10

> Format per question: **Question → Answer → Why it’s correct (with CCNA takeaway)**

---

## Question 1
**Question:** Which connector is used with twisted-pair cabling in an Ethernet LAN?

**Answer:** **RJ-45 (8P8C)**

**Why it’s correct:**
- Ethernet over twisted-pair copper (UTP/STP) uses the **RJ-45** style modular connector.
- The other pictured connectors are associated with **coaxial** (e.g., BNC) or **fiber** (e.g., LC/SC) cabling, not copper twisted-pair.

**CCNA takeaway:** *Twisted-pair Ethernet = RJ-45. Fiber = LC/SC. Coax = BNC.*

---

## Question 2
**Question:** Host B (Teachers subnet) sends a packet to Host D (Students subnet). Which Layer 2 and Layer 3 addresses are in the PDUs sent from Host B to the router?

**Answer (first hop, Host B → Router):**
- **Layer 2 destination (MAC):** Router Fa0 MAC **00-00-0c-94-36-ab**
- **Layer 2 source (MAC):** Host B MAC **00-00-0c-94-36-bb**
- **Layer 3 destination (IP):** Host D IP **172.16.20.200**
- **Layer 3 source (IP):** Host B IP **172.16.10.200**

**Why it’s correct:**
- **Layer 3 (IP) addresses stay end-to-end** from the original sender to the final destination (Host B → Host D).
- **Layer 2 (MAC) addresses are hop-by-hop.** On Host B’s LAN, the next hop is the **default gateway** (router Fa0), so the frame’s destination MAC is the router interface MAC, not Host D’s MAC.

**CCNA takeaway:** *IP = end-to-end. MAC = next hop (changes at every routed hop).*

---

## Question 3
**Question:** With QoS implemented, what are the priorities (highest → lowest) for: web page browsing, financial transactions, and live audio conference?

**Answer:** **audio conference → financial transactions → web page**

**Why it’s correct:**
- **Real-time voice/audio** is the most delay- and jitter-sensitive (needs low latency).
- **Financial transactions** are important but can generally tolerate slightly more delay than voice (they need reliability).
- **Web browsing** is typically best-effort and can tolerate delay the most.

**CCNA takeaway:** *Real-time voice/video gets highest priority; best-effort web usually lowest.*

---

## Question 4
**Question:** What will happen if the default gateway address is incorrectly configured on a host?

**Answer:** **The host cannot communicate with hosts in other networks.**

**Why it’s correct:**
- The default gateway is only needed to reach **remote networks** (outside the local subnet).
- Local subnet communication can still work using **ARP** to learn local MAC addresses.
- A bad gateway means traffic for non-local destinations can’t be forwarded correctly.

**CCNA takeaway:** *Wrong gateway = local works, off-subnet fails.*

---

## Question 5
**Question:** Which scenario describes a function provided by the transport layer?

**Answer:** **A student has two web browser windows open; the transport layer ensures the correct web page is delivered to the correct browser window.**

**Why it’s correct:**
- The transport layer (TCP/UDP) provides **multiplexing/demultiplexing** using **port numbers** so data reaches the correct application/session on a host.
- Other options describe different layers:
  - “Unique identifier burned into the phone” = **MAC address (Layer 2)**
  - “Encoded within the transport header” = not a transport function
  - “Formats the screen” = **presentation layer (Layer 6)** concept

**CCNA takeaway:** *Transport layer uses ports to deliver traffic to the right app/process.*

---

## Question 6
**Question:** Which two statements describe features of an IPv4 routing table on a router? (Choose two.)

**Answer (choose two):**
1. **If a default static route is configured in the router, an entry will be included in the routing table with source code `S`.**
2. **It stores information about routes derived from the active router interfaces.**

**Why it’s correct:**
- Static routes appear in `show ip route` with code **S** (default static often shown as **S***).
- A router automatically installs **directly connected routes** for networks on **active** interfaces.
- Incorrect statements:
  - `netstat -r` is a host OS command; CCNA routers use **show ip route**.
  - Routers prefer **lower** metric (after administrative distance), not higher.
  - Routing tables don’t list MAC addresses (that’s ARP/neighbor tables, not routing tables).
  - Directly connected routes are typically **C** (connected) and **L** (local host route), not **C and S**.

**CCNA takeaway:** *Routing table = network prefixes + next hops + codes (C/L/S/D/O/etc.), not MAC addresses.*

---

## Question 7
**Question:** What attribute of a NIC would place it at the data link layer of the OSI model?

**Answer:** **MAC address**

**Why it’s correct:**
- The NIC’s **MAC address** is a **Layer 2** identifier used for Ethernet frame delivery on a LAN.
- IP addresses are Layer 3; cables/ports are physical layer concepts.

**CCNA takeaway:** *Layer 2 = MAC. Layer 3 = IP.*

---

## Question 8
**Question:** Which two statements accurately describe an advantage or a disadvantage of deploying NAT for IPv4? (Choose two.)

**Answer (choose two):**
1. **NAT introduces problems for some applications that require end-to-end connectivity.**
2. **NAT provides a solution to slow down IPv4 address depletion.**

**Why it’s correct:**
- NAT helps conserve public IPv4 addresses by allowing many private hosts to share fewer public addresses (especially with PAT).
- NAT can break/complicate protocols that embed IP info in payloads or require true end-to-end reachability (some VoIP, peer-to-peer, some IPsec scenarios, inbound services).
- Incorrect statements:
  - NAT isn’t about improving packet handling or adding authentication.
  - It doesn’t inherently increase routing table size.
  - Switch performance isn’t the core issue (NAT is usually done on routers/firewalls).

**CCNA takeaway:** *NAT conserves IPv4 but can break “end-to-end” assumptions.*

---

## Question 9
**Question:** Match the header field with the appropriate OSI layer.

**Answer (field → OSI layer):**

| Header/Field | OSI Layer |
|---|---|
| FCS (frame check sequence) | **Layer 2 — Data Link** |
| 802.2 header (LLC) | **Layer 2 — Data Link** |
| Destination MAC address | **Layer 2 — Data Link** |
| Source IP address | **Layer 3 — Network** |
| TTL | **Layer 3 — Network** |
| Destination port number | **Layer 4 — Transport** |
| Acknowledgement number | **Layer 4 — Transport** |

**Why it’s correct:**
- Ethernet/LLC/FCS/MAC addressing are **Data Link (L2)**.
- IP addressing and TTL are part of the **IP header (L3)**.
- Ports and TCP ACKs are **Transport (L4)** concepts.

**CCNA takeaway:** *Ethernet = L2, IP = L3, TCP/UDP = L4.*

---

## Question 10
**Question:** Which subnet would include the address **192.168.1.96** as a usable host address?

**Answer:** **192.168.1.64/26**

**Why it’s correct:**
- A **/26** has a block size of **64** addresses: 0–63, **64–127**, 128–191, 192–255.
- So **192.168.1.64/26** spans **192.168.1.64 to 192.168.1.127**.
  - Network address = **.64**
  - Broadcast address = **.127**
  - Usable hosts = **.65–.126**
- **.96** falls in that usable host range.

**CCNA takeaway:** *Find the block size (256 − mask octet) → locate the subnet range → verify it’s not network/broadcast.*

---

# CCNA Practice Questions 11–20 (Answers + Explanations)

> Format: **Question → Answer → Why it’s correct (CCNA notes)**

---

## Question 11
**Question:** Match the network with the correct IP address and prefix that will satisfy the usable host addressing requirements for each network.

- Network A: **100 hosts**
- Network B: **50 hosts**
- Network C: **25 hosts**
- Network D: **2 hosts**

**Answer (matches):**
- **Network A → 192.168.0.0/25**
- **Network B → 192.168.0.128/26**
- **Network C → 192.168.0.192/27**
- **Network D → 192.168.0.224/30**

**Why it’s correct:**
- A **/25** has 128 total addresses → **126 usable**, enough for 100 hosts.
- A **/26** has 64 total → **62 usable**, enough for 50 hosts.
- A **/27** has 32 total → **30 usable**, enough for 25 hosts.
- A **/30** has 4 total → **2 usable**, perfect for a point-to-point link (2 hosts).

---

## Question 12
**Question:** Match each description to its corresponding term.

**Answer (matches):**
- **Message sizing →** the process of breaking up a long message into individual pieces before being sent over the network  
- **Message encoding →** the process of converting information from one format into another acceptable for transmission  
- **Message encapsulation →** the process of placing one message format inside another message format

**Why it’s correct:**
- **Sizing** is segmentation/chunking so data fits into what lower layers can carry.
- **Encoding** is changing representation (e.g., characters → bits, or encoding scheme).
- **Encapsulation** is adding headers/trailers as data moves down the stack (L4 segment → L3 packet → L2 frame, etc.).

---

## Question 13
**Question:** Public folder is Read-Only for anyone who can log in, but Edit rights only for the network admin group. Which AAA component is addressed?

**Answer:** **Authorization**

**Why it’s correct:**
- **Authentication** = “Who are you?” (login/identity)
- **Authorization** = “What are you allowed to do?” (permissions like read vs edit)
- **Accounting** = “What did you do?” (logging/auditing)
- This scenario is clearly about **permissions** after login → **Authorization**.

---

## Question 14
**Question:** An admin types `config t` and gets “% Invalid input detected…” (prompt shows `Switch1>`). What is the problem?

**Answer:** **The administrator must first enter privileged EXEC mode before issuing the command.**

**Why it’s correct:**
- `Switch1>` means **user EXEC mode**.
- `configure terminal` (and its shortcut `conf t` / `config t`) works from **privileged EXEC** (`Switch1#`).
- Correct sequence:
  - `Switch1> enable`
  - `Switch1# configure terminal`

---

## Question 15
**Question:** What command can be used on a Windows PC to see the IP configuration of that computer?

**Answer:** **`ipconfig`**

**Why it’s correct:**
- `ipconfig` displays a Windows host’s IP settings (IP address, mask, gateway, etc.).
- For more detail (DNS, DHCP info, MAC), use: **`ipconfig /all`**.
- `show ip interface brief` and `show interfaces` are **Cisco IOS** commands, not Windows.

---

## Question 16
**Question:** Which two commands can be used on a Windows host to display the routing table? (Choose two.)

**Answer:** **`netstat -r`** and **`route print`**

**Why it’s correct:**
- **`route print`** shows the Windows routing table directly.
- **`netstat -r`** also displays the routing table (similar output).
- `show ip route` is Cisco IOS, `tracert` shows hop path, `netstat -s` shows protocol statistics.

---

## Question 17
**Question:** Match the description to the IPv6 addressing component.

**Answer (matches):**
- **Used by an organization to identify subnets →** **subnet ID**
- **Equivalent to the host portion of an IPv4 address →** **interface ID**
- **Network portion assigned by the provider →** **global routing prefix**

**Why it’s correct:**
- The **global routing prefix** is typically ISP-assigned and identifies the organization/site globally.
- The **subnet ID** is used internally by the organization to create subnets.
- The **interface ID** identifies the specific interface on the subnet (host-like part).

---

## Question 18
**Question:** PC1 issues an ARP request because it needs to send a packet to PC2. What happens next?

**Answer:** **PC2 will send an ARP reply with its MAC address.**

**Why it’s correct:**
- ARP is used on the **local LAN** to map **destination IP → destination MAC**.
- PC1 sends an **ARP Request (broadcast)**: “Who has PC2’s IP?”
- The device that owns that IP (PC2) responds with an **ARP Reply (unicast)** containing its **MAC address**.
- Switches don’t “answer ARP for hosts” (they forward frames). Routers answer ARP for **their own interfaces** (or with special proxy ARP configs).

---

## Question 19
**Question:** Which two statements are correct about MAC and IP addresses during data transmission if NAT is not involved? (Choose two.)

**Answer (choose two):**
- ✅ **Destination and source MAC addresses have local significance and change every time a frame goes from one LAN to another.**
- ✅ **Destination IP addresses in a packet header remain constant along the entire path to a target host.**

**Why it’s correct:**
- **Layer 2 (MAC) addresses are hop-by-hop.** Each router strips the old L2 header and builds a new frame for the next link → MACs change each hop.
- **Layer 3 (IP) addresses are end-to-end.** Source/destination IP stay the same across the path (unless NAT is used).
- What *does* change at L3 each hop is **TTL/hop limit**, not the destination IP.

---

## Question 20
**Question:** What are two features of ARP? (Choose two.)

**Answer (choose two):**
- ✅ **If a host is ready to send a packet to a local destination device and it has the IP address but not the MAC address of the destination, it generates an ARP broadcast.**
- ✅ **If a device receiving an ARP request has the destination IPv4 address, it responds with an ARP reply.**

**Why it’s correct:**
- ARP Request is typically sent as an **Ethernet broadcast** (destination MAC **FF:FF:FF:FF:FF:FF**).
- The host that owns the target IPv4 address responds with an **ARP Reply** (usually unicast) providing its MAC.
- Hosts consult their **ARP cache/table** (not a switch MAC address table) to avoid repeated broadcasts.

---

# CCNA Practice Questions 21–30 (Answers + Explanations)

> Format: **Question → Answer → Why it’s correct (CCNA notes)**

---

## Question 21
**Question:** Which switching method drops frames that fail the FCS check?

**Answer:** **Store-and-forward switching**

**Why it’s correct:**
- **Store-and-forward** receives the **entire Ethernet frame** into memory, then verifies the **FCS (Frame Check Sequence/CRC)**.
- If the FCS is wrong, the switch **drops** the frame (it does not forward corrupted frames).
- **Cut-through** starts forwarding after reading the destination MAC (low latency) and **may forward** frames before the FCS is checked.

---

## Question 22
**Question:** Users report longer delays during certain times of the week. What should engineers check to see if this is normal network behavior?

**Answer:** **The network performance baseline**

**Why it’s correct:**
- A **baseline** is historical “normal” performance data (latency, throughput, CPU, interface utilization, auth response times, etc.).
- Comparing current performance to the baseline helps determine if slow periods match **expected peak usage** (e.g., Monday morning logins).
- Debugs/packet captures/syslog are useful for troubleshooting, but they don’t tell you what “normal” looked like over time.

---

## Question 23
**Question:** A new admin entered a banner message on a Cisco device. What is the fastest way to test whether the banner is properly configured?

**Answer:** **Exit privileged EXEC mode and press Enter.**

**Why it’s correct:**
- Banners (like **banner motd**) appear when a session starts (console/VTY) or at the **login/connection prompt**.
- The quickest test is to **end/exit the current session context** and trigger the “start” screen again (pressing **Enter** after exiting).
- Rebooting/power cycling also shows the banner, but that’s much slower and disruptive.

> CCNA note: In real life, you can also test by opening a **new SSH/Telnet (if enabled) / console session** to see the banner immediately.

---

## Question 24
**Question:** Match the application protocols to the correct transport protocols.

**Answer (matches):**
- **FTP → TCP**
- **HTTP → TCP**
- **SMTP → TCP**
- **DHCP → UDP**
- **TFTP → UDP**

**Why it’s correct:**
- **TCP** is used where reliability/ordered delivery is important (FTP, HTTP, SMTP).
- **UDP** is used for lightweight request/response or simple transfers:
  - **DHCP** uses UDP (client/server broadcasts, speed, simple exchange).
  - **TFTP** uses UDP (simple file transfer with minimal overhead).

---

## Question 25
**Question:** A local user account (username + secret) exists for SSH. Which three additional steps are required to accept only encrypted SSH connections? (Choose three.)

**Answer (choose three):**
- ✅ **Configure the IP domain name on the router**
- ✅ **Generate the SSH keys**
- ✅ **Enable inbound vty SSH sessions**

**Why it’s correct:**
- SSH requires RSA keys; Cisco IOS needs:
  - `ip domain-name <domain>` (used when generating keys)
  - `crypto key generate rsa`
  - VTY lines set to SSH only: `line vty 0 4` → `transport input ssh`
- You **do not** enable inbound Telnet if the goal is “only encrypted SSH”.
- DNS configuration is not required just to accept SSH connections (it’s optional for name resolution).
- “Two-way pre-shared keys” is not how standard SSH access is configured on IOS.

---

## Question 26
**Question:** Which information does the `show startup-config` command display?

**Answer:** **The contents of the saved configuration file in the NVRAM**

**Why it’s correct:**
- **startup-config** = saved config in **NVRAM** (loaded at boot).
- **running-config** = current active config in **RAM**.
- IOS image and bootstrap program are different files/locations (Flash/ROM), not shown by `show startup-config`.

---

## Question 27
**Question:** Match each description with an appropriate IP address.

**Answer (matches):**
- **Public address → 198.133.219.2**
- **Loopback address → 127.0.0.1**
- **Link-local address → 169.254.1.5**
- **Experimental address → 240.2.6.255**

**Why it’s correct:**
- **127.0.0.0/8** is reserved for **loopback** testing (localhost).
- **169.254.0.0/16** is IPv4 **link-local/APIPA** (used when DHCP fails).
- **240.0.0.0/4** is **experimental (Class E)** and not used for normal host addressing.
- **198.133.219.2** is not in private ranges (10/8, 172.16/12, 192.168/16) → treated as **public**.

---

## Question 28
**Question:** What is the consequence of configuring a router with the `ipv6 unicast-routing` global configuration command?

**Answer:** **The IPv6-enabled router interfaces begin sending ICMPv6 Router Advertisement messages.**

**Why it’s correct:**
- `ipv6 unicast-routing` enables the router to **forward IPv6** (act as an IPv6 router).
- When forwarding is enabled, IPv6 interfaces can send **ICMPv6 Router Advertisements (RAs)** used for **SLAAC**.
- It does not automatically “activate” all interfaces, and it does not create a global unicast address by itself.

---

## Question 29
**Question:** What mechanism is used by a router to prevent a received IPv4 packet from traveling endlessly on a network?

**Answer:** **It decrements the TTL value by 1 and if the result is 0, it discards the packet and sends a Time Exceeded message to the source host.**

**Why it’s correct:**
- Every router hop **decrements TTL** (Time To Live) by 1.
- If TTL reaches **0**, the router drops the packet and sends **ICMP Time Exceeded** back to the sender.
- This prevents routing loops from circulating packets forever (and is how `traceroute/tracert` works).

---

## Question 30
**Question:** Which range of link-local addresses can be assigned to an IPv6-enabled interface?

**Answer:** **FE80::/10**

**Why it’s correct:**
- **FE80::/10** is the IPv6 **link-local** prefix (used on the local link only).
- **FF00::/8** is multicast.
- **FEC0::/10** was an old “site-local” concept (deprecated).
- **FDEE::/7** is in the **unique local address (ULA)** space (commonly FC00::/7, with FD00::/8 used in practice).

---

# CCNA Practice Questions 31–40 (Answers + Explanations)

> Format: **Question → Answer → Why it’s correct (CCNA notes)**

---

## Question 31
**Question:** If PC1 is sending a packet to PC2 and routing has been configured between the two routers, what will R1 do with the Ethernet frame header attached by PC1?

**Answer:** **Remove the Ethernet header and configure a new Layer 2 header before sending it out S0/0/0.**

**Why it’s correct:**
- Routers make forwarding decisions using the **Layer 3 (IP) header**, not the incoming Ethernet header.
- When R1 receives an **Ethernet frame** from PC1, it **de-encapsulates** (removes) the Layer 2 header/trailer, examines the IP packet, chooses the outgoing interface (serial), then **re-encapsulates** the packet with a **new Layer 2 header** appropriate for the outgoing link (PPP/HDLC on serial).
- Key idea: **L2 changes hop-by-hop; L3 stays end-to-end (without NAT).**

---

## Question 32
**Question:** What are two characteristics shared by TCP and UDP? (Choose two.)

**Answer (choose two):**
- ✅ **port numbering**
- ✅ **use of checksum**

**Why it’s correct:**
- **Both TCP and UDP** use **port numbers** to identify source/destination applications (multiplexing/demultiplexing).
- **Both include a checksum** for error detection of the segment/datagram.
- Not shared:
  - **3-way handshake** and **window size** are TCP-only.
  - **Connectionless communication** describes UDP (TCP is connection-oriented).

---

## Question 33
**Question:** What are two characteristics of IP? (Choose two.)

**Answer (choose two):**
- ✅ **does not require a dedicated end-to-end connection**
- ✅ **operates independently of the network media**

**Why it’s correct:**
- IP is **connectionless** (no dedicated circuit; it’s packet-switched).
- IP is **media independent** (works over Ethernet, Wi-Fi, fiber, etc.).
- IP does **not** guarantee delivery, retransmit, or reorder packets—those are transport-layer responsibilities (TCP).

---

## Question 34
**Question:** A remote employee logs in with username/password, attends an important video conference, the primary ISP fails, and a secondary connection activates within seconds with no noticeable disruption. Which three network characteristics are described? (Choose three.)

**Answer (choose three):**
- ✅ **security**
- ✅ **fault tolerance**
- ✅ **quality of service**

**Why it’s correct:**
- Username/password login points to **security** (controlled access).
- Automatic secondary link takeover is **fault tolerance** (redundancy/availability).
- Ensuring excellent video quality is **QoS** (prioritizing voice/video, reducing delay/jitter/loss).

---

## Question 35
**Question:** Which two traffic types use the Real-Time Transport Protocol (RTP)? (Choose two.)

**Answer (choose two):**
- ✅ **voice**
- ✅ **video**

**Why it’s correct:**
- **RTP** is designed for **real-time** media delivery where timing matters (VoIP, video conferencing/streaming).
- Web browsing and file transfers typically rely on TCP-based application protocols instead.

---

## Question 36
**Question:** Which two statements describe how to assess traffic flow patterns and network traffic types using a protocol analyzer? (Choose two.)

**Answer (choose two):**
- ✅ **Capture traffic during peak utilization times to get a good representation of the different traffic types.**
- ✅ **Perform the capture on different network segments.**

**Why it’s correct:**
- Capturing at **peak times** shows what the network really looks like under load (real mix of apps and bottlenecks).
- Capturing on **different segments** (access, distribution, server VLANs, WAN edge, etc.) shows different flows and helps locate where traffic originates/accumulates.
- “Only capture WAN” / “only the data center” is too narrow; weekends may not represent normal usage.

---

## Question 37
**Question:** Refer to the exhibit. What is wrong with the displayed termination?

**Answer:** **The untwisted length of each wire is too long.**

**Why it’s correct:**
- For UTP/STP Ethernet, you should keep the pairs **twisted as close as possible** to the connector.
- Excessive untwist increases **crosstalk/EMI** and can cause errors—especially at higher speeds.

---

## Question 38
**Question:** A small site wants the same mask for all networks. Needs: IP phones (22), PCs (20), printers (2), scanners (2). Given 192.168.10.0/24, which single subnet mask is most efficient for four subnets?

**Answer:** **255.255.255.224** (/**27**)

**Why it’s correct:**
- With one fixed mask (FLSM), you size for the **largest subnet**.
- Largest requirement is **22 hosts** → needs at least **22 usable**.
- **/27** gives 32 total addresses → **30 usable**, enough for 22 (and 20).
- **/28** (14 usable) is too small; **/26** (62 usable) works but wastes more addresses than /27.

---

## Question 39
**Question:** Network is 192.168.10.0 subnetted with **/29**. Use the **5th subnet** (subnet zero is first). Router interface uses **first usable**, server uses **last usable**. What server IP/mask/gateway allows Internet connectivity?

**Answer:** **IP 192.168.10.38, subnet mask 255.255.255.248, default gateway 192.168.10.33**

**Why it’s correct:**
- /29 block size = **8** (…0, 8, 16, 24, **32**, 40…).
- 5th subnet (counting subnet zero as 1st) is **192.168.10.32/29**:
  - Network: .32
  - Usable hosts: **.33 – .38**
  - Broadcast: .39
- Router (first usable) = **.33**, server (last usable) = **.38**, mask = **255.255.255.248**.

---

## Question 40
**Question:** What three requirements are defined by the protocols used in network communications to allow message transmission across a network? (Choose three.)

**Answer (choose three):**
- ✅ **message encoding**
- ✅ **delivery options**
- ✅ **message size**

**Why it’s correct:**
- Network protocols define rules such as:
  - **How data is represented/encoded** (so both sides interpret bits correctly)
  - **How messages are delivered** (unicast/multicast/broadcast, reliability expectations, etc.)
  - **How large messages can be / how they’re segmented** (message size constraints)
- Items like “end-device installation” and “connector specifications” are not protocol requirements for message transmission.

---
