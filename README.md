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
