# CCNA Practice Questions 1–60 — Study Notes (Answers + Deep Explanations)

Click any question in the navigation to jump. Each question shows the **correct answer**, a detailed **why**, and **where to study it in NetAcad**.

- Jump to: [Answer Key](#answer-key) • [NetAcad Study Map](#netacad-study-map)


## Quick navigation

- [Q01 — Twisted-pair connector in an Ethernet LAN](#q1) — **Answer:** *RJ‑45 (8P8C)**
- [Q02 — L2 vs L3 addresses (Host → Router first hop)](#q2) — **Answer:** L2 destination MAC: Router interface MAC (default gateway on Teache...
- [Q03 — QoS priority order](#q3) — **Answer:** *Live audio conference → Financial transactions → Web browsing**
- [Q04 — Incorrect default gateway impact](#q4) — **Answer:** *The host cannot communicate with hosts in other networks (off‑subn...
- [Q05 — Transport layer function (ports)](#q5) — **Answer:** *Two browser windows; transport layer ensures the right data goes t...
- [Q06 — IPv4 routing table features (choose two)](#q6) — **Answer:** 1) It stores information about routes derived from active router in...
- [Q07 — NIC attribute at OSI Layer 2](#q7) — **Answer:** *MAC address**
- [Q08 — NAT advantages/disadvantages (choose two)](#q8) — **Answer:** NAT slows IPv4 address depletion (conserves public IPv4 addresses).
- [Q09 — Header fields to OSI layers (match)](#q9) — **Answer:** FCS → L2 Data Link
- [Q10 — Subnet that contains 192.168.1.96 as usable host](#q10) — **Answer:** *192.168.1.64/26**
- [Q11 — VLSM by host requirements (match)](#q11) — **Answer:** A → 192.168.0.0/25 (126 usable)
- [Q12 — Message sizing/encoding/encapsulation (match)](#q12) — **Answer:** Message sizing → breaking a long message into smaller pieces before...
- [Q13 — AAA component (permissions)](#q13) — **Answer:** *Authorization**
- [Q14 — `config t` invalid from `Switch1>`](#q14) — **Answer:** Must enter privileged EXEC mode first.
- [Q15 — Windows command for IP configuration](#q15) — **Answer:** *`ipconfig`** (or `ipconfig /all` for full details)
- [Q16 — Windows commands to display routing table (choose two)](#q16) — **Answer:** *`route print` and `netstat -r`**
- [Q17 — IPv6 address components (match)](#q17) — **Answer:** Global routing prefix → network portion assigned by provider/ISP
- [Q18 — What happens after an ARP request?](#q18) — **Answer:** *PC2 sends an ARP reply with its MAC address.**
- [Q19 — MAC vs IP behavior without NAT (choose two)](#q19) — **Answer:** Source/destination MAC addresses are local and change at every rout...
- [Q20 — Two features of ARP (choose two)](#q20) — **Answer:** If the sender knows the destination IP but not MAC for a local dest...
- [Q21 — Switching method that drops frames failing FCS](#q21) — **Answer:** *Store‑and‑forward switching**
- [Q22 — Checking if periodic slowness is “normal”](#q22) — **Answer:** *Network performance baseline**
- [Q23 — Fastest way to test a banner](#q23) — **Answer:** *Exit privileged EXEC mode and press Enter** (to trigger a fresh se...
- [Q24 — Application protocols ↔ Transport protocols (match)](#q24) — **Answer:** FTP → TCP
- [Q25 — Configure router to accept only SSH (choose three)](#q25) — **Answer:** Configure the IP domain name
- [Q26 — `show startup-config` displays what?](#q26) — **Answer:** *Saved configuration in NVRAM**
- [Q27 — Identify public/loopback/link-local/experimental (match)](#q27) — **Answer:** Public → 198.133.219.2
- [Q28 — `ipv6 unicast-routing` effect](#q28) — **Answer:** *IPv6-enabled interfaces begin sending ICMPv6 Router Advertisements...
- [Q29 — Prevent endless IPv4 looping](#q29) — **Answer:** *Router decrements TTL by 1; if it reaches 0, drops packet and send...
- [Q30 — IPv6 link-local range](#q30) — **Answer:** *FE80::/10**
- [Q31 — What R1 does with incoming Ethernet header](#q31) — **Answer:** *Remove Ethernet header; add a new Layer 2 header for the outgoing ...
- [Q32 — Shared characteristics of TCP and UDP (choose two)](#q32) — **Answer:** *Port numbering and checksum**
- [Q33 — Characteristics of IP (choose two)](#q33) — **Answer:** does not require a dedicated end‑to‑end connection (connectionless)
- [Q34 — Network characteristics in the scenario (choose three)](#q34) — **Answer:** *Security, Fault tolerance, Quality of service**
- [Q35 — RTP traffic types (choose two)](#q35) — **Answer:** *Voice and Video**
- [Q36 — Protocol analyzer best capture strategy (choose two)](#q36) — **Answer:** Capture during peak utilization times.
- [Q37 — What’s wrong with the cable termination?](#q37) — **Answer:** *Untwisted wire length is too long.**
- [Q38 — Best single mask for 4 subnets (FLSM)](#q38) — **Answer:** *255.255.255.224 (/27)**
- [Q39 — /29: 5th subnet, router first usable, server last usable](#q39) — **Answer:** *IP 192.168.10.38 /29 (255.255.255.248), gateway 192.168.10.33**
- [Q40 — What protocols define for communication (choose three)](#q40) — **Answer:** *Message encoding, Delivery options, Message size**
- [Q41 — TCP/IP layers used for file transfer](#q41) — **Answer:** *Application, Transport, Internet, Network Access**
- [Q42 — IMAP advantage over POP](#q42) — **Answer:** *Messages stay on the mail server until manually deleted (server‑ba...
- [Q43 — Interpreting `tracert` output (choose two)](#q43) — **Answer:** There is connectivity between this device and 192.168.100.1.
- [Q44 — CSMA/CD characteristics (choose three)](#q44) — **Answer:** All devices on a segment see data that passes on the medium.
- [Q45 — OSI layers that map to TCP/IP Application (choose three)](#q45) — **Answer:** *Session, Presentation, Application**
- [Q46 — Malware that can slow network by spreading](#q46) — **Answer:** *Worm**
- [Q47 — Two most effective defenses against malware (choose two)](#q47) — **Answer:** Update OS and application software
- [Q48 — Low‑power wireless for home automation](#q48) — **Answer:** *ZigBee**
- [Q49 — Server type that relies on A/AAAA/NS/MX records](#q49) — **Answer:** *DNS**
- [Q50 — EUI‑64 interface ID from MAC](#q50) — **Answer:** *1E6F:65FF:FEC2:BDF8**
- [Q51 — Protocols at top layer of TCP/IP (choose two)](#q51) — **Answer:** *DNS and POP**
- [Q52 — Effect of `ip default-gateway` on a switch](#q52) — **Answer:** *The switch can be remotely managed from a host on another network.**
- [Q53 — Signal degradation causes in UTP (choose two)](#q53) — **Answer:** *Low‑quality cable/connectors and Improper termination**
- [Q54 — Frame field ensuring integrity against interference](#q54) — **Answer:** *FCS (Frame Check Sequence)**
- [Q55 — MAC sublayer functions (choose two)](#q55) — **Answer:** Implements trailer with frame check sequence (FCS) for error detection
- [Q56 — Smallest mask for 200 devices](#q56) — **Answer:** *255.255.255.0 (/24)**
- [Q57 — Destination port 22](#q57) — **Answer:** *SSH**
- [Q58 — SMTP provides what service?](#q58) — **Answer:** *Sending/relaying email (client → server and server → server).**
- [Q59 — DoS characteristic](#q59) — **Answer:** *An attack that slows or crashes a device or network service.**
- [Q60 — Attenuation meaning](#q60) — **Answer:** *Loss of signal strength as distance increases.**

---

## Questions

<a id="q1"></a>

## Q1 — Twisted-pair connector in an Ethernet LAN
**Question:** Which connector is used with twisted-pair cabling in an Ethernet LAN?  
**Correct answer:** **RJ‑45 (8P8C)**


**Where to study (NetAcad ITN):**
- Module 4.4.2 — UTP Cabling Standards and Connectors
- Module 4.4.4 — Activity: Cable Pinouts

**Why this is correct (deep dive):**
- **Copper twisted‑pair Ethernet** (UTP/STP) terminates in an **8‑position 8‑contact modular connector**, commonly called **RJ‑45**.
- CCNA often contrasts:
  - **Fiber connectors** (LC, SC, ST) → *not* for twisted pair.
  - **Coax connectors** (BNC/F-type) → *not* for twisted pair.
- “RJ‑45” is the exam word; “8P8C” is the precise hardware term.

**Exam trap:** Don’t confuse *connector type* (RJ‑45/LC/SC) with *cable type* (UTP/STP/fiber).


**Confidence:** High

---


<a id="q2"></a>

## Q2 — L2 vs L3 addresses (Host → Router first hop)
**Question:** Host B (Teachers subnet) sends a packet to Host D (Students subnet). Which Layer 2 and Layer 3 addresses are in the PDUs sent from Host B to the router?  
**Correct answer (Host B → Router, first hop):**
- **L2 destination MAC:** **Router interface MAC** (default gateway on Teachers LAN)  
- **L2 source MAC:** **Host B MAC**  
- **L3 destination IP:** **Host D IP**  
- **L3 source IP:** **Host B IP**

(Your draft included specific MAC/IP values from the exhibit; the logic above is the CCNA rule.)


**Where to study (NetAcad ITN):**
- Module 3.7.7 — Role of the Data Link Layer Addresses (Different IP Networks)
- Module 8.4.2 — Default Gateway

**Why this is correct (deep dive):**
- **Routers break broadcast domains.** Host B cannot send an Ethernet frame directly to Host D’s MAC because Host D is on a **different subnet**.
- The host uses **ARP** to learn the **default gateway’s MAC** (router interface on its LAN).
- **Layer 2 is hop‑by‑hop:**
  - On the Teachers LAN: destination MAC = router interface MAC.
  - After routing, on the Students LAN: destination MAC will become Host D’s MAC.
- **Layer 3 is end‑to‑end (without NAT):**
  - Source IP remains Host B, destination IP remains Host D the entire trip.
- **What changes at Layer 3 each hop?** Not the destination IP—**the TTL** changes (decrements).

**Exam trap:** Many people answer “destination MAC = Host D” — that’s only true if Host D is **in the same subnet**.


**Confidence:** High

---


<a id="q3"></a>

## Q3 — QoS priority order
**Question:** With QoS implemented, what are the priorities (highest → lowest) for: web page browsing, financial transactions, and live audio conference?  
**Correct answer:** **Live audio conference → Financial transactions → Web browsing**


**Where to study (NetAcad ITN):**
- Module 1.6.4 — Quality of Service

**Why this is correct (deep dive):**
- **Voice/audio** is extremely sensitive to:
  - **Latency** (delay)
  - **Jitter** (variation in delay)
  - **Loss**
  Even small delays make the conversation “feel” broken.
- **Financial transactions** are usually sensitive to:
  - **Reliability/integrity** (must arrive correctly)
  - Moderate delay may be tolerable compared to voice, but it’s still more important than web browsing.
- **Web browsing** is usually **best effort**. It can tolerate delay (pages load slower) and is frequently deprioritized versus real‑time media.

**CCNA rule of thumb:** Real‑time (voice/video) gets priority; best effort (web) is lowest.


**Confidence:** High

---


<a id="q4"></a>

## Q4 — Incorrect default gateway impact
**Question:** What will happen if the default gateway address is incorrectly configured on a host?  
**Correct answer:** **The host cannot communicate with hosts in other networks (off‑subnet).**


**Where to study (NetAcad ITN):**
- Module 8.4.2 — Default Gateway
- Module 10.3.1 — Default Gateway on a Host

**Why this is correct (deep dive):**
- When a host sends to:
  - **Same subnet** → it ARPs for the destination host’s MAC and sends directly (gateway not needed).
  - **Different subnet** → it must send the frame to the **default gateway**.
- With the wrong gateway, the host still has:
  - Correct IP/mask → it can still identify local vs remote.
  - Working local L2 → it can still reach local peers.
- But it cannot correctly forward remote traffic because the next hop is wrong/unreachable.

**Quick test in real life:** Local ping works, remote ping fails (unless there’s some weird proxy/alternate route).


**Confidence:** High

---


<a id="q5"></a>

## Q5 — Transport layer function (ports)
**Question:** Which scenario describes a function provided by the transport layer?  
**Correct answer:** **Two browser windows; transport layer ensures the right data goes to the right window (process).**


**Where to study (NetAcad ITN):**
- Module 14.4 — Port Numbers (Socket Pairs)

**Why this is correct (deep dive):**
- Transport (TCP/UDP) provides **multiplexing/demultiplexing**:
  - Multiple applications talk over the network at the same time.
  - The host uses **port numbers** to deliver incoming data to the correct process/socket.
- Example:
  - Browser tab A might use local ephemeral port 51500.
  - Browser tab B might use local ephemeral port 51501.
  TCP keeps the streams separate even if both talk to port 443 on the server.

**Exam trap:** “Unique identifier burned into the phone” is MAC (Layer 2). Transport does *ports*, not MACs.


**Confidence:** High

---


<a id="q6"></a>

## Q6 — IPv4 routing table features (choose two)
**Question:** Which two statements describe features of an IPv4 routing table on a router?  
**Correct answer (choose two):**
1) **It stores information about routes derived from active router interfaces** (connected routes).  
2) **If a default static route is configured, it appears with source code `S`** (often `S*` for the candidate default).


**Where to study (NetAcad ITN):**
- Module 8.5.2 — IP Router Routing Table
- Module 8.5.6 — Introduction to an IPv4 Routing Table

**Why this is correct (deep dive):**
- A router installs routes into the routing table from multiple sources:
  - **Directly connected networks** (from interfaces that are up/up) → code `C`
  - **Local interface addresses** → code `L`
  - **Static routes** → code `S` (default static often shown `S*`)
  - **Dynamic protocols** like OSPF/EIGRP/RIP → `O`, `D`, `R`, etc.
- The routing table contains **network prefixes and next hops**, not MAC addresses.
- Route selection logic is: **Longest Prefix Match** first, then (for equal prefix length) typically **Administrative Distance**, then **metric**.

**Exam traps:**
- `netstat -r` is a **PC OS** command, not a Cisco router command.
- “Higher metric is preferred” is false: **lower metric** is preferred *within a routing protocol*.


**Confidence:** High

---


<a id="q7"></a>

## Q7 — NIC attribute at OSI Layer 2
**Question:** What attribute of a NIC would place it at the data link layer of the OSI model?  
**Correct answer:** **MAC address**


**Where to study (NetAcad ITN):**
- Module 7.2.2 — Ethernet MAC Address
- Module 6.3.3 — Layer 2 Addresses

**Why this is correct (deep dive):**
- Ethernet frames use **MAC addresses** (48-bit) as Layer 2 identifiers.
- Switches learn MACs in their MAC address table and forward frames based on MAC destinations.
- IP addressing belongs to Layer 3 and is configured on hosts/interfaces, not “burned into” a NIC.


**Confidence:** High

---


<a id="q8"></a>

## Q8 — NAT advantages/disadvantages (choose two)
**Question:** Which two statements accurately describe an advantage or a disadvantage of deploying NAT for IPv4?  
**Correct answer (choose two):**
- ✅ **NAT slows IPv4 address depletion** (conserves public IPv4 addresses).  
- ✅ **NAT can break/complicate some applications requiring end‑to‑end connectivity.**


**Where to study (NetAcad ITN):**
- Module 11.3.2 — Routing to the Internet (NAT concept)
- Module 8.5 — Introduction to Routing

**Why this is correct (deep dive):**
- **IPv4 conservation:** Many private hosts (RFC1918) share one/few public IPs (PAT/overload).
- **Breaks end-to-end:** Anything that expects real end‑to‑end addressing can struggle:
  - Some VoIP and peer‑to‑peer apps
  - Some IPsec modes
  - Inbound server hosting without port‑forwarding/NAT rules
- NAT is not “authentication” or “encryption” — it’s address translation.

**Exam trap:** NAT is not a security feature by itself, though it can hide internal addressing.


**Confidence:** High

---


<a id="q9"></a>

## Q9 — Header fields to OSI layers (match)
**Question:** Match the header field with the appropriate OSI layer.  
**Correct answer (field → layer):**
- **FCS** → **L2 Data Link**  
- **802.2 header (LLC)** → **L2 Data Link**  
- **Destination MAC** → **L2 Data Link**  
- **Source IP** → **L3 Network**  
- **TTL** → **L3 Network**  
- **Destination port** → **L4 Transport**  
- **Acknowledgement number** → **L4 Transport**


**Where to study (NetAcad ITN):**
- Module 3.6.3 — Protocol Data Units
- Module 6.3.2 — Frame Fields
- Module 8.2.2 — IPv4 Packet Header Fields
- Module 14.2.3 — TCP Header Fields

**Why this is correct (deep dive):**
- **L2** cares about framing, MAC addressing, and error detection (FCS).
- **L3** is routing and logical addressing (IP), including **TTL/hop limit** control.
- **L4** is process‑to‑process delivery (ports) and reliability features like **ACKs** (TCP).

**Memory hook:** “MAC = L2, IP = L3, Ports = L4.”


**Confidence:** High

---


<a id="q10"></a>

## Q10 — Subnet that contains 192.168.1.96 as usable host
**Question:** Which subnet would include the address **192.168.1.96** as a usable host address?  
**Correct answer:** **192.168.1.64/26**


**Where to study (NetAcad ITN):**
- Module 11.5.1–11.5.2 — Subnet an IPv4 Network

**Why this is correct (deep dive):**
- /26 means:
  - Host bits = 6 → total addresses = 2^6 = 64
  - Subnet “block size” in last octet = 64
- Ranges:
  - 192.168.1.0–63
  - **192.168.1.64–127**
  - 192.168.1.128–191
  - 192.168.1.192–255
- 192.168.1.96 falls within **64–127** and is not network (.64) or broadcast (.127), so it is usable.


**Confidence:** High

---


<a id="q11"></a>

## Q11 — VLSM by host requirements (match)
**Question:** Match the network with the correct IP address and prefix to satisfy usable hosts:
- A: 100 hosts, B: 50 hosts, C: 25 hosts, D: 2 hosts  
**Correct answer:**
- **A → 192.168.0.0/25** (126 usable)  
- **B → 192.168.0.128/26** (62 usable)  
- **C → 192.168.0.192/27** (30 usable)  
- **D → 192.168.0.224/30** (2 usable)


**Where to study (NetAcad ITN):**
- Module 11.8 — VLSM

**Why this is correct (deep dive):**
- Usable hosts formula: **2^(host bits) − 2**.
- /25 → 7 host bits → 2^7 − 2 = 126.
- /26 → 6 host bits → 62.
- /27 → 5 host bits → 30.
- /30 → 2 host bits → 2 (perfect for point‑to‑point).
- The addressing is contiguous and non‑overlapping inside 192.168.0.0/24.

**Exam trap:** Don’t use /29 for “2 hosts” (it wastes addresses). CCNA loves /30 for 2-host links.


**Confidence:** High

---


<a id="q12"></a>

## Q12 — Message sizing/encoding/encapsulation (match)
**Question:** Match each description to its term.  
**Correct answer:**
- **Message sizing** → breaking a long message into smaller pieces before sending  
- **Message encoding** → converting information into a format acceptable for transmission  
- **Message encapsulation** → placing one message format inside another (adding headers/trailers)


**Where to study (NetAcad ITN):**
- Module 3.1.6 — Message Encoding
- Module 3.1.8 — Message Size

**Why this is correct (deep dive):**
- **Sizing** is the idea behind **segmentation** (L4) and **fragmentation** (L3, IPv4) when necessary.
- **Encoding** is how information becomes signals/bits (examples: ASCII/UTF‑8, line coding, modulation).
- **Encapsulation** is the “envelope” concept as data goes down the stack:
  - Data → Segment → Packet → Frame → Bits.


**Confidence:** High

---


<a id="q13"></a>

## Q13 — AAA component (permissions)
**Question:** Public folder is read‑only for anyone who can log in, but edit only for network admins. Which AAA component is addressed?  
**Correct answer:** **Authorization**


**Where to study (NetAcad ITN):**
- Module 16.3.4 — Authentication, Authorization, and Accounting (AAA)

**Why this is correct (deep dive):**
- **Authentication:** prove identity (username/password, MFA, certs).
- **Authorization:** what you’re allowed to do after you’re authenticated (read vs write).
- **Accounting:** logs what you did (auditing: who changed what and when).
- Here the user can log in (authentication succeeded), but permissions differ → **authorization**.


**Confidence:** High

---


<a id="q14"></a>

## Q14 — `config t` invalid from `Switch1>`
**Question:** Admin types `config t` and gets “% Invalid input…” while prompt is `Switch1>`. What’s the problem?  
**Correct answer:** Must enter **privileged EXEC mode** first.


**Where to study (NetAcad ITN):**
- Module 2.2.1–2.2.4 — Primary Command Modes / Navigate Between IOS Modes

**Why this is correct (deep dive):**
- `Switch1>` = **user EXEC** (limited commands).
- `Switch1#` = **privileged EXEC** (enable mode).
- Global configuration requires privileged EXEC:
  1. `Switch1> enable`
  2. `Switch1# configure terminal`

**Exam trap:** Prompts matter. Many questions are really about reading `>` vs `#`.


**Confidence:** High

---


<a id="q15"></a>

## Q15 — Windows command for IP configuration
**Question:** What command can be used on a Windows PC to see the IP configuration?  
**Correct answer:** **`ipconfig`** (or `ipconfig /all` for full details)


**Where to study (NetAcad ITN):**
- Module 2.7.3 — Verify Windows PC IP Configuration (ipconfig)

**Why this is correct (deep dive):**
- `ipconfig` shows IP, mask, gateway (basic).
- `ipconfig /all` adds DNS servers, DHCP status, lease times, and MAC.


**Confidence:** High

---


<a id="q16"></a>

## Q16 — Windows commands to display routing table (choose two)
**Question:** Which two commands can be used on a Windows host to display the routing table?  
**Correct answer:** **`route print`** and **`netstat -r`**


**Where to study (NetAcad ITN):**
- Module 8.4.4 — Host Routing Tables
- Module 14.4.4 — The netstat Command

**Why this is correct (deep dive):**
- Both commands show the IPv4/IPv6 route table on Windows.
- Contrast:
  - `tracert` shows hop path (not the routing table).
  - `show ip route` is Cisco IOS, not Windows.


**Confidence:** High

---


<a id="q17"></a>

## Q17 — IPv6 address components (match)
**Question:** Match the description to the IPv6 addressing component.  
**Correct answer:**
- **Global routing prefix** → network portion assigned by provider/ISP  
- **Subnet ID** → used by the organization to identify internal subnets  
- **Interface ID** → host/interface portion (like IPv4 host part)


**Where to study (NetAcad ITN):**
- Module 12.2 — IPv6 Address Representation
- Module 12.3.6 — IPv6 GUA Structure

**Why this is correct (deep dive):**
- Typical global unicast structure (often /64 per subnet):
  - Global routing prefix (e.g., /48)
  - Subnet ID (to reach /64)
  - Interface ID (last 64 bits)


**Confidence:** High

---


<a id="q18"></a>

## Q18 — What happens after an ARP request?
**Question:** PC1 sends an ARP request because it needs to send a packet to PC2. What happens next?  
**Correct answer:** **PC2 sends an ARP reply with its MAC address.**


**Where to study (NetAcad ITN):**
- Module 9.2.3–9.2.4 — ARP Request / ARP Reply

**Why this is correct (deep dive):**
- ARP resolves **IPv4 address → MAC address** on the local link.
- Steps:
  1. PC1 checks ARP cache; if missing → broadcasts ARP request (FF:FF:FF:FF:FF:FF).
  2. PC2 (owner of the target IP) replies unicast with its MAC.
  3. PC1 updates ARP cache and sends the actual frame.

**Possible ambiguity check:** This assumes PC2 is in the **same subnet**. If PC2 were remote, PC1 would ARP for the **default gateway** instead.


**Confidence:** High

---


<a id="q19"></a>

## Q19 — MAC vs IP behavior without NAT (choose two)
**Question:** Which two statements are correct about MAC and IP addresses during transmission if NAT is not involved?  
**Correct answer (choose two):**
- ✅ Source/destination **MAC addresses are local** and change at every routed hop.  
- ✅ Destination **IP address stays constant** end‑to‑end.


**Where to study (NetAcad ITN):**
- Module 3.6 — Encapsulation
- Module 8.1.2 — IP Encapsulation
- Module 7.1 — Ethernet Encapsulation

**Why this is correct (deep dive):**
- At each router:
  - Router strips the incoming L2 header/trailer.
  - Router forwards the L3 packet (same source/dest IP).
  - Router builds a new L2 frame for the next link (new source/dest MAC).
- L3 also changes TTL (and header checksum in IPv4), but not the destination IP.


**Confidence:** High

---


<a id="q20"></a>

## Q20 — Two features of ARP (choose two)
**Question:** What are two features of ARP?  
**Correct answer (choose two):**
- ✅ If the sender knows the destination IP but not MAC for a local destination, it generates an **ARP broadcast**.  
- ✅ The device that owns the target IPv4 address responds with an **ARP reply**.


**Where to study (NetAcad ITN):**
- Module 9.2.1–9.2.2 — ARP Overview / ARP Functions

**Why this is correct (deep dive):**
- ARP request = broadcast; ARP reply = typically unicast.
- ARP tables/cache reduce repeated broadcasts.
- ARP is only for **IPv4**; IPv6 uses **NDP** (Neighbor Discovery).


**Confidence:** High

---


<a id="q21"></a>

## Q21 — Switching method that drops frames failing FCS
**Question:** Which switching method drops frames that fail the FCS check?  
**Correct answer:** **Store‑and‑forward switching**


**Where to study (NetAcad ITN):**
- Module 7.4.1 — Frame Forwarding Methods on Cisco Switches

**Why this is correct (deep dive):**
- **Store‑and‑forward**:
  - Receives the **entire frame**.
  - Computes/validates **FCS (CRC)**.
  - Drops corrupted frames.
- **Cut‑through**:
  - Begins forwarding after reading destination MAC.
  - Low latency, but can forward bad frames (FCS not yet checked).

**Exam trap:** “Cut‑through” sounds advanced, but it’s *less* checking.


**Confidence:** High

---


<a id="q22"></a>

## Q22 — Checking if periodic slowness is “normal”
**Question:** Users report delays at certain times of the week. What should engineers check to see if this is normal behavior?  
**Correct answer:** **Network performance baseline**


**Where to study (NetAcad ITN):**
- Module 17.4.5 — Network Baseline

**Why this is correct (deep dive):**
- A baseline is what “normal” looks like historically:
  - utilization, latency, auth response time, CPU, error rates.
- If the baseline shows “every Monday 09:00 is slow,” that’s expected peak load—not necessarily a fault.
- Packet captures/debug/syslog help diagnose *why*, but baseline answers *whether it’s normal*.


**Confidence:** High

---


<a id="q23"></a>

## Q23 — Fastest way to test a banner
**Question:** After configuring a banner on a Cisco device, what is the fastest way to test that the banner is properly configured?  
**Correct answer:** **Exit privileged EXEC mode and press Enter** (to trigger a fresh session prompt).

> **Extra clarity:** A Cisco banner (MOTD/login) is shown when a session starts (console/SSH/Telnet). The fastest test is to **trigger a fresh login prompt** (end the current session / back out to the login) so the banner displays again. Exam wording often phrases this as “exit and press Enter”.


**Where to study (NetAcad ITN):**
- Module 2.4.5 — Banner Messages

**Why this is correct (deep dive):**
- **MOTD/login banners** are displayed at the start of a session (console/VTY).
- The quickest verification is to **end the current session context** and re-trigger the login/banner display.
- Reboot/power cycle would also show it, but is slow and disruptive.

**Small ambiguity note:** On a live device, the *clearest* test is opening a **new console/SSH session**, but your quiz option that best matches this idea is “Exit privileged EXEC mode and press Enter.”


**Confidence:** Medium

---


<a id="q24"></a>

## Q24 — Application protocols ↔ Transport protocols (match)
**Question:** Match the application protocols to the correct transport protocols.  
**Correct answer:**
- **FTP → TCP**  
- **HTTP → TCP**  
- **SMTP → TCP**  
- **DHCP → UDP**  
- **TFTP → UDP**


**Where to study (NetAcad ITN):**
- Module 14.2.5 — Applications that use TCP
- Module 14.3.4 — Applications that use UDP
- Module 15.3.4 — SMTP, POP, and IMAP
- Module 15.5.1 — File Transfer Protocol
- Module 15.5.1 — TFTP

**Why this is correct (deep dive):**
- TCP: reliable, ordered delivery (web, email transfer, file transfer control).
- UDP: lightweight, low overhead for simple request/response or simple transfers.
- Extra CCNA details:
  - DHCP uses UDP **67/68**.
  - TFTP uses UDP **69**.
  - HTTP uses TCP **80** (HTTPS TCP **443**).
  - SMTP uses TCP **25** (submission often **587**, SMTPS **465**).


**Confidence:** High

---


<a id="q25"></a>

## Q25 — Configure router to accept only SSH (choose three)
**Question:** Local user account exists on R1 for SSH. Which three additional steps are required to accept only encrypted SSH connections?  
**Correct answer (choose three):**
- ✅ Configure the **IP domain name**  
- ✅ **Generate SSH keys** (RSA)  
- ✅ Enable inbound **VTY SSH** sessions (`transport input ssh`)


**Where to study (NetAcad ITN):**
- Module 16.4.4 — Enable SSH

**Why this is correct (deep dive):**
- SSH on IOS requires RSA keys; key generation requires a domain name:
  - `ip domain-name example.com`
  - `crypto key generate rsa`
- VTY lines must accept SSH and reject Telnet:
  - `line vty 0 4`
  - `transport input ssh`
- To actually use the local username/password for login, you typically also configure:
  - `login local`
  (Not offered in your option list, but it’s part of a complete config in real life.)

**Exam trap:** “Enable inbound vty Telnet sessions” is the opposite of “SSH only.”


**Confidence:** High

---


<a id="q26"></a>

## Q26 — `show startup-config` displays what?
**Question:** Which information does the `show startup-config` command display?  
**Correct answer:** **Saved configuration in NVRAM**


**Where to study (NetAcad ITN):**
- Module 2.5.1 — Configuration Files

**Why this is correct (deep dive):**
- **running-config** = current config in RAM (active).
- **startup-config** = saved config stored in NVRAM (loaded on boot).
- IOS image = usually in flash; bootstrap = ROM; not shown by `show startup-config`.


**Confidence:** High

---


<a id="q27"></a>

## Q27 — Identify public/loopback/link-local/experimental (match)
**Question:** Match each description with an appropriate IPv4 address.  
**Correct answer:**
- **Public** → 198.133.219.2  
- **Loopback** → 127.0.0.1  
- **Link‑local (APIPA)** → 169.254.1.5  
- **Experimental (Class E)** → 240.2.6.255


**Where to study (NetAcad ITN):**
- Module 11.3.4 — Special Use IPv4 Addresses

**Why this is correct (deep dive):**
- Loopback: **127.0.0.0/8**
- Link-local: **169.254.0.0/16** (DHCP failure self-assigned)
- Experimental: **240.0.0.0/4**
- Public: not in private ranges (10/8, 172.16/12, 192.168/16)


**Confidence:** High

---


<a id="q28"></a>

## Q28 — `ipv6 unicast-routing` effect
**Question:** What is the consequence of configuring a router with `ipv6 unicast-routing`?  
**Correct answer:** **IPv6-enabled interfaces begin sending ICMPv6 Router Advertisements (RAs).**


**Where to study (NetAcad ITN):**
- Module 12.4.1 — Static GUA Configuration on a Router

**Why this is correct (deep dive):**
- `ipv6 unicast-routing` enables the router to **forward IPv6** (act as a router, not just a host).
- Once forwarding is enabled, interfaces with IPv6 enabled typically send **RAs**, allowing hosts to:
  - Learn prefix information
  - Autoconfigure addresses via **SLAAC**
  - Learn default gateway (the router’s link-local)
- It does not automatically activate interfaces or create a global unicast address.

**Note:** RAs can be controlled/suppressed, but the CCNA default behavior is RA generation when IPv6 routing is enabled.


**Confidence:** High

---


<a id="q29"></a>

## Q29 — Prevent endless IPv4 looping
**Question:** What mechanism prevents an IPv4 packet from traveling endlessly?  
**Correct answer:** **Router decrements TTL by 1; if it reaches 0, drops packet and sends ICMP Time Exceeded.**


**Where to study (NetAcad ITN):**
- Module 8.2.2 — IPv4 Header Fields (TTL)
- Module 13.1.4 — Time Exceeded

**Why this is correct (deep dive):**
- TTL enforces a maximum hop count.
- When TTL hits 0, router discards and sends **ICMP Time Exceeded**.
- `tracert/traceroute` works by intentionally causing TTL to expire at each hop.


**Confidence:** High

---


<a id="q30"></a>

## Q30 — IPv6 link-local range
**Question:** Which range of link-local addresses can be assigned to an IPv6-enabled interface?  
**Correct answer:** **FE80::/10**


**Where to study (NetAcad ITN):**
- Module 12.3.7 — IPv6 LLA

**Why this is correct (deep dive):**
- Link-local addresses are used on the local link only and are required for:
  - Neighbor Discovery
  - Router Advertisements
  - Next-hop routing on local segment
- Common distractors:
  - FF00::/8 = multicast
  - FEC0::/10 = deprecated site-local
  - FC00::/7 (often FD00::/8 in practice) = unique local addresses (ULA)


**Confidence:** High

---


<a id="q31"></a>

## Q31 — What R1 does with incoming Ethernet header
**Question:** PC1 sends to PC2 and routing is configured. What will R1 do with the Ethernet frame header attached by PC1?  
**Correct answer:** **Remove Ethernet header; add a new Layer 2 header for the outgoing interface (S0/0/0).**


**Where to study (NetAcad ITN):**
- Module 8.5.1 — Router Packet Forwarding Decision
- Module 3.6.5 — De-encapsulation Example

**Why this is correct (deep dive):**
- Routers operate primarily at **Layer 3**:
  - They decapsulate the incoming L2 frame.
  - Make a forwarding decision based on destination IP (routing table).
  - Re-encapsulate with the appropriate L2 framing for the next link.
- Ethernet L2 header is not valid on a serial link (PPP/HDLC).


**Confidence:** High

---


<a id="q32"></a>

## Q32 — Shared characteristics of TCP and UDP (choose two)
**Question:** What are two characteristics shared by TCP and UDP?  
**Correct answer (choose two):** **Port numbering** and **checksum**


**Where to study (NetAcad ITN):**
- Module 14.1.3–14.1.5 — Transport Layer Protocols (TCP/UDP)

**Why this is correct (deep dive):**
- Both use ports to identify applications.
- Both provide an error-detection checksum (UDP checksum required in IPv6; in IPv4 it exists and is commonly used).
- Only TCP has:
  - 3‑way handshake
  - sequence/ack for reliability
  - windowing/flow control


**Confidence:** High

---


<a id="q33"></a>

## Q33 — Characteristics of IP (choose two)
**Question:** What are two characteristics of IP?  
**Correct answer (choose two):**
- ✅ **does not require a dedicated end‑to‑end connection** (connectionless)  
- ✅ **operates independently of network media** (media independent)


**Where to study (NetAcad ITN):**
- Module 8.1.3 — Characteristics of IP

**Why this is correct (deep dive):**
- IP is best effort; it does not guarantee delivery, ordering, or retransmission.
- Those reliability features are handled by transport protocols (e.g., TCP).


**Confidence:** High

---


<a id="q34"></a>

## Q34 — Network characteristics in the scenario (choose three)
**Question:** Login + video conference + ISP failover with no disruption. Which three characteristics?  
**Correct answer (choose three):** **Security**, **Fault tolerance**, **Quality of service**


**Where to study (NetAcad ITN):**
- Module 1.6.1–1.6.3 — Reliable Networks (Architecture, Fault Tolerance, Scalability)
- Module 1.6.4 — QoS
- Module 1.6.5 — Network Security

**Why this is correct (deep dive):**
- Security: user authentication (username/password).
- Fault tolerance: redundancy/failover to secondary ISP.
- QoS: video quality relies on prioritization and controlling delay/jitter/loss.


**Confidence:** High

---


<a id="q35"></a>

## Q35 — RTP traffic types (choose two)
**Question:** Which two traffic types use RTP?  
**Correct answer (choose two):** **Voice** and **Video**


**Where to study (NetAcad ITN):**
- Module 17.2.3 — Voice and Video Applications
- Module 14.3 — UDP Overview

**Why this is correct (deep dive):**
- RTP carries real‑time media streams.
- It’s commonly paired with control signaling/protocols (SIP, H.323) and RTCP for stats/feedback.


**Confidence:** High

---


<a id="q36"></a>

## Q36 — Protocol analyzer best capture strategy (choose two)
**Question:** Which two statements describe how to assess traffic patterns using a protocol analyzer?  
**Correct answer (choose two):**
- ✅ Capture during **peak utilization** times.  
- ✅ Capture on **different network segments**.


**Where to study (NetAcad ITN):**
- Module 17.3.2 — Protocol Analysis
- Module 3.7.10 — Lab: Use Wireshark to View Network Traffic

**Why this is correct (deep dive):**
- Peak captures show the true mix under load (what causes complaints).
- Different segments show different flows (access VLAN vs server VLAN vs WAN edge).


**Confidence:** High

---


<a id="q37"></a>

## Q37 — What’s wrong with the cable termination?
**Question:** What is wrong with the displayed termination?  
**Correct answer:** **Untwisted wire length is too long.**


**Where to study (NetAcad ITN):**
- Module 4.4.1–4.4.2 — Properties/Standards of UTP Cabling

**Why this is correct (deep dive):**
- UTP relies on twisting to reduce crosstalk and EMI.
- Untwisting too far near the connector increases interference and errors.
- Best practice is to keep twist as close to the plug as possible (a few millimeters).


**Confidence:** High

---


<a id="q38"></a>

## Q38 — Best single mask for 4 subnets (FLSM)
**Question:** Same mask for all networks. Needs: 22, 20, 2, 2 hosts. Network is 192.168.10.0/24. Which single mask is most efficient?  
**Correct answer:** **255.255.255.224 (/27)**


**Where to study (NetAcad ITN):**
- Module 11.7.2 — Minimize Unused Host IPv4 Addresses and Maximize Subnets

**Why this is correct (deep dive):**
- With one mask, you size for the largest subnet requirement: **22 hosts**.
- /27:
  - 5 host bits → 2^5 − 2 = **30 usable**
  - Enough for 22 and 20.
- /28 provides 14 usable → too small.
- /26 provides 62 usable → works but wastes more addresses.


**Confidence:** High

---


<a id="q39"></a>

## Q39 — /29: 5th subnet, router first usable, server last usable
**Question:** 192.168.10.0 subnetted /29. Use 5th subnet (subnet zero is first). Router gets first usable, server gets last usable. What server config?  
**Correct answer:** **IP 192.168.10.38 /29 (255.255.255.248), gateway 192.168.10.33**


**Where to study (NetAcad ITN):**
- Module 11.5 — Subnet an IPv4 Network

**Why this is correct (deep dive):**
- /29 block size = 8:
  - 0, 8, 16, 24, **32**, 40, ...
- Count subnets (subnet zero is first):
  1) .0/29  
  2) .8/29  
  3) .16/29  
  4) .24/29  
  5) **.32/29**
- For 192.168.10.32/29:
  - Network = .32
  - Usable = **.33–.38**
  - Broadcast = .39
- Router first usable = .33; server last usable = .38.


**Confidence:** High

---


<a id="q40"></a>

## Q40 — What protocols define for communication (choose three)
**Question:** What three requirements are defined by protocols to allow message transmission across a network?  
**Correct answer (choose three):** **Message encoding**, **Delivery options**, **Message size**


**Where to study (NetAcad ITN):**
- Module 3.1.5–3.1.10 — Network Protocol Requirements (encoding/size/timing/delivery)

**Why this is correct (deep dive):**
- Protocols must define:
  - **Encoding**: how bits represent data so both ends interpret identically.
  - **Delivery options**: unicast/multicast/broadcast; connection expectations; acknowledgments at higher layers, etc.
  - **Message size**: segmentation rules, maximum sizes, how large a PDU can be.
- “Connector specifications” and “end-device installation” are physical/implementation topics, not protocol definitions.


**Confidence:** High

---


<a id="q41"></a>

## Q41 — TCP/IP layers used for file transfer
**Question:** If Host1 transfers a file to the server, what layers of TCP/IP model are used?  
**Correct answer:** **Application, Transport, Internet, Network Access**


**Where to study (NetAcad ITN):**
- Module 3.5.3 — TCP/IP Protocol Model

**Why this is correct (deep dive):**
- Any real communication uses the full stack:
  - Application: the file-transfer protocol (FTP/SMB/HTTP/etc.)
  - Transport: TCP (reliability) or UDP (depends, but most file transfer uses TCP)
  - Internet: IP routing
  - Network access: Ethernet/Wi‑Fi and physical signaling


**Confidence:** High

---


<a id="q42"></a>

## Q42 — IMAP advantage over POP
**Question:** Advantage for small orgs adopting IMAP instead of POP?  
**Correct answer:** **Messages stay on the mail server until manually deleted (server‑based mailbox).**


**Where to study (NetAcad ITN):**
- Module 15.3.4 — SMTP, POP, and IMAP

**Why this is correct (deep dive):**
- IMAP is designed for **synchronization** across multiple devices/clients:
  - Read/unread state, folders, server-side storage.
- POP typically downloads mail to a client and may delete from server (unless configured otherwise).
- This makes IMAP better when users have laptop + phone + webmail.


**Confidence:** High

---


<a id="q43"></a>

## Q43 — Interpreting `tracert` output (choose two)
**Question:** Based on tracert output, which two statements are correct?  
**Correct answer (choose two):**
- ✅ There is connectivity between this device and **192.168.100.1**.  
- ✅ There are **4 hops between** this device and **192.168.100.1**.


**Where to study (NetAcad ITN):**
- Module 13.2.5 — Traceroute - Test the Path

**Why this is correct (deep dive):**
- “Trace complete” after reaching the destination means the destination responded → connectivity exists.
- If destination is listed as hop 5, then hops 1–4 are intermediate routers → 4 hops “between”.

**Exam trap:** You cannot prove “videoconferencing quality” from tracert alone.


**Confidence:** High

---


<a id="q44"></a>

## Q44 — CSMA/CD characteristics (choose three)
**Question:** What are three characteristics of CSMA/CD?  
**Correct answer (choose three):**
- ✅ All devices on a segment see data that passes on the medium.  
- ✅ A device listens and waits until the media is not busy before transmitting.  
- ✅ After detecting a collision, hosts retry after a random backoff delay.


**Where to study (NetAcad ITN):**
- Module 6.2.7 — Contention-Based Access - CSMA/CD

**Why this is correct (deep dive):**
- CSMA/CD is for **shared, half‑duplex Ethernet**:
  - Carrier Sense = listen first
  - Multiple Access = many devices share medium
  - Collision Detection = detect and stop; then random backoff

**Not correct options explained:**
- “Electronic token” = Token Ring concept.
- “Priority transmit” is not CSMA/CD behavior.
- Jam signal exists, but it doesn’t mean the medium is clear; it helps ensure collision detection.


**Confidence:** High

---


<a id="q45"></a>

## Q45 — OSI layers that map to TCP/IP Application (choose three)
**Question:** Which three OSI layers map to TCP/IP Application layer?  
**Correct answer:** **Session**, **Presentation**, **Application**


**Where to study (NetAcad ITN):**
- Module 3.5.4 — OSI and TCP/IP Model Comparison

**Why this is correct (deep dive):**
- TCP/IP combines OSI layers 5–7 into one Application layer.
- Transport stays Transport; Network stays Internet; Data Link + Physical map to Network Access.


**Confidence:** High

---


<a id="q46"></a>

## Q46 — Malware that can slow network by spreading
**Question:** Slow network after user installed third‑party software. Which malware might cause slow performance?  
**Correct answer:** **Worm**


**Where to study (NetAcad ITN):**
- Module 16.2.1 — Types of Malware

**Why this is correct (deep dive):**
- Worms self‑replicate and spread across networks → heavy traffic and resource use.
- Viruses typically require a host file and user action; can cause issues, but the classic “network slowdown from spreading” is a worm symptom.
- Phishing/spam are not malware types that directly cause LAN-wide traffic saturation.


**Confidence:** High

---


<a id="q47"></a>

## Q47 — Two most effective defenses against malware (choose two)
**Question:** Two most effective defenses against malware?  
**Correct answer (choose two):**
- ✅ **Update OS and application software**  
- ✅ **Install and update antivirus/endpoint protection**


**Where to study (NetAcad ITN):**
- Module 16.3.3 — Upgrade, Update, and Patch
- Module 16.3.7 — Endpoint Security

**Why this is correct (deep dive):**
- Updates close known vulnerabilities exploited by malware.
- Endpoint protection improves prevention/detection/removal (signatures + behavioral detection).
- Firewalls/passwords help overall security posture but are not as direct as patching + endpoint protection for malware defense.


**Confidence:** High

---


<a id="q48"></a>

## Q48 — Low‑power wireless for home automation
**Question:** Which wireless technology has low-power and low data rate requirements and is popular in home automation?  
**Correct answer:** **ZigBee**


**Where to study (NetAcad ITN):**
- Module 4.6.2 — Types of Wireless Media
- Module 1.7.7 — Technology Trends in the Home

**Why this is correct (deep dive):**
- ZigBee is designed for:
  - low power sensors
  - low throughput
  - mesh networking (good coverage in a home)
- Wi‑Fi/5G are higher power and higher bandwidth.
- LoRaWAN is low power too, but aimed at **wide-area, long-range IoT**, not typical in-home mesh control.


**Confidence:** High

---


<a id="q49"></a>

## Q49 — Server type that relies on A/AAAA/NS/MX records
**Question:** Which type of server relies on A, NS, AAAA, MX records to provide services?  
**Correct answer:** **DNS**


**Where to study (NetAcad ITN):**
- Module 15.4.1 — Domain Name System

**Why this is correct (deep dive):**
- Those are DNS resource record types:
  - A = IPv4 host record
  - AAAA = IPv6 host record
  - NS = authoritative name servers
  - MX = mail exchangers


**Confidence:** High

---


<a id="q50"></a>

## Q50 — EUI‑64 interface ID from MAC
**Question:** Interface ID for IPv6 using EUI‑64 from MAC **1C‑6F‑65‑C2‑BD‑F8**?  
**Correct answer:** **1E6F:65FF:FEC2:BDF8**


**Where to study (NetAcad ITN):**
- Module 12.5.6 — EUI-64 Process

**Why this is correct (deep dive):**
EUI‑64 steps:
1) Split MAC into two halves:  
   - 1C‑6F‑65 and C2‑BD‑F8  
2) Insert **FFFE** in the middle:  
   - 1C‑6F‑65‑FF‑FE‑C2‑BD‑F8  
3) Flip the **U/L bit** (XOR first byte with 0x02):  
   - 1C → 1E  
4) Group into hextets:  
   - **1E6F:65FF:FEC2:BDF8**

**Exam trap:** People forget the U/L bit flip step.


**Confidence:** High

---


<a id="q51"></a>

## Q51 — Protocols at top layer of TCP/IP (choose two)
**Question:** Which two protocols operate at the top layer of the TCP/IP suite?  
**Correct answer:** **DNS** and **POP**


**Where to study (NetAcad ITN):**
- Module 15.1.3 — TCP/IP Application Layer Protocols

**Why this is correct (deep dive):**
- TCP/IP top layer = **Application**.
- DNS and POP are application protocols.
- TCP/UDP = Transport, IP = Internet, Ethernet = Network access.


**Confidence:** High

---


<a id="q52"></a>

## Q52 — Effect of `ip default-gateway` on a switch
**Question:** `ip default-gateway 172.16.100.1` is configured on a switch. What is the effect?  
**Correct answer:** **The switch can be remotely managed from a host on another network.**


**Where to study (NetAcad ITN):**
- Module 10.3.2 — Default Gateway on a Switch

**Why this is correct (deep dive):**
- On a Layer 2 switch, management traffic (SSH/Telnet/SNMP/HTTP) originates from its **SVI management IP**.
- To reach off-subnet managers, it needs a default gateway.
- This does not create a management interface with that address; it sets the **next hop** for off-subnet traffic.


**Confidence:** High

---


<a id="q53"></a>

## Q53 — Signal degradation causes in UTP (choose two)
**Question:** Two common causes of signal degradation with UTP?  
**Correct answer (choose two):** **Low‑quality cable/connectors** and **Improper termination**


**Where to study (NetAcad ITN):**
- Module 4.3.1 — Characteristics of Copper Cabling
- Module 4.4.1 — Properties of UTP Cabling

**Why this is correct (deep dive):**
- Bad materials and bad terminations increase:
  - attenuation
  - crosstalk
  - reflections/impedance mismatch
- “Loss of light over long distances” is fiber optics.
- “Low-quality shielding” doesn’t apply to UTP (unshielded).


**Confidence:** High

---


<a id="q54"></a>

## Q54 — Frame field ensuring integrity against interference
**Question:** Which frame field is created by a source node and used by destination to ensure data wasn’t altered?  
**Correct answer:** **FCS (Frame Check Sequence)**


**Where to study (NetAcad ITN):**
- Module 6.3.2 — Frame Fields (FCS)
- Module 7.1.4 — Ethernet Frame Fields

**Why this is correct (deep dive):**
- Sender computes a CRC and stores it in the FCS trailer.
- Receiver recomputes and compares; mismatch = corrupted frame → drop.


**Confidence:** High

---


<a id="q55"></a>

## Q55 — MAC sublayer functions (choose two)
**Question:** Which two functions are performed at the **MAC sublayer** to facilitate Ethernet communication?  
**Correct answer (choose two):**

> **Extra clarity:** The **MAC sublayer** covers **framing + MAC addressing + error detection (FCS)** and **media access**. The choices about “which network layer protocol is encapsulated” and “interface between upper layers and NIC hardware” are **LLC sublayer** responsibilities.
- ✅ **Implements trailer with frame check sequence (FCS) for error detection**  
- ✅ **Implements a process to delimit fields within an Ethernet II frame** (framing)


**Where to study (NetAcad ITN):**
- Module 7.1.2–7.1.3 — Data Link Sublayers / MAC Sublayer

**Why this is correct (deep dive):**
- The Data Link layer is split into:
  - **LLC (Logical Link Control):** interface to upper layers, protocol multiplexing control (in the IEEE model).
  - **MAC (Media Access Control):** framing, MAC addressing, and error detection + media access rules.
- **FCS** is classic MAC responsibility (error detection).
- **Frame delimiting/framing** (identifying start/end of fields; building the MAC header/trailer format) is also MAC responsibility.

**Important nuance (possible ambiguity):**
- Another option in your list says: *“places information in the Ethernet frame that identifies which network layer protocol is being encapsulated.”*
  - In **Ethernet II**, that’s the **EtherType** field, which is part of the MAC header.
  - In **IEEE 802.3 + 802.2 LLC**, protocol identification is associated with **LLC/SNAP**.
- Because the question explicitly says **MAC sublayer** and also offers a pure framing option, the safest CCNA-style pair is **FCS + framing/delimiting**.  
If your course material treats EtherType as a MAC function, your instructor might accept that alternative—send the exact option list if the quiz marks it wrong and we’ll lock it down.


**Confidence:** Medium

---


<a id="q56"></a>

## Q56 — Smallest mask for 200 devices
**Question:** New LAN must support 200 connected devices. Smallest mask?  
**Correct answer:** **255.255.255.0 (/24)**


**Where to study (NetAcad ITN):**
- Module 11.5 — Subnet an IPv4 Network

**Why this is correct (deep dive):**
- Need ≥ 200 usable hosts.
- /24 provides 254 usable (256 − 2).
- /25 provides 126 usable → too small.
- Therefore /24 is the smallest in the options that satisfies the requirement.


**Confidence:** High

---


<a id="q57"></a>

## Q57 — Destination port 22
**Question:** Destination port number is 22. What service?  
**Correct answer:** **SSH**


**Where to study (NetAcad ITN):**
- Module 14.4 — Port Number Groups (Well-known ports)
- Module 16.4.4 — Enable SSH

**Why this is correct (deep dive):**
- TCP/22 is the well-known port for SSH remote management.


**Confidence:** High

---


<a id="q58"></a>

## Q58 — SMTP provides what service?
**Question:** What service is provided by SMTP?  
**Correct answer:** **Sending/relaying email (client → server and server → server).**


**Where to study (NetAcad ITN):**
- Module 15.3.4 — Email Protocols (SMTP)

**Why this is correct (deep dive):**
- SMTP is for **sending** mail.
- POP/IMAP are for **retrieving** mail.
- SSH/Telnet are for remote access, not mail.


**Confidence:** High

---


<a id="q59"></a>

## Q59 — DoS characteristic
**Question:** What characteristic describes a DoS attack?  
**Correct answer:** **An attack that slows or crashes a device or network service.**


**Where to study (NetAcad ITN):**
- Module 16.2.4 — Denial of Service Attacks

**Why this is correct (deep dive):**
- DoS targets **availability**.
- It overwhelms resources (bandwidth, CPU, sessions), making service unavailable.


**Confidence:** High

---


<a id="q60"></a>

## Q60 — Attenuation meaning
**Question:** What does “attenuation” mean in data communication?  
**Correct answer:** **Loss of signal strength as distance increases.**


**Where to study (NetAcad ITN):**
- Module 4.4.1 — Properties of UTP Cabling (Attenuation)

**Why this is correct (deep dive):**
- Attenuation is signal weakening along the medium (copper or fiber).
- Not the same as:
  - Crosstalk (leakage between pairs)
  - Latency (time delay)
  - Amplification (strengthening)


**Confidence:** High

---

---

## NetAcad study map for these 60 questions

> This section tells you *exactly where to review the concept* inside the Cisco NetAcad **CCNA: Introduction to Networks (ITN)** outline.

### Module 1 — Related questions: Q3, Q34, Q48
- Module 1.6.1–1.6.3 — Reliable Networks (Architecture, Fault Tolerance, Scalability)  
  ↳ *Used in:* Q34
- Module 1.6.4 — QoS  
  ↳ *Used in:* Q34
- Module 1.6.4 — Quality of Service  
  ↳ *Used in:* Q3
- Module 1.6.5 — Network Security  
  ↳ *Used in:* Q34
- Module 1.7.7 — Technology Trends in the Home  
  ↳ *Used in:* Q48

### Module 2 — Related questions: Q14, Q15, Q23, Q26
- Module 2.2.1–2.2.4 — Primary Command Modes / Navigate Between IOS Modes  
  ↳ *Used in:* Q14
- Module 2.4.5 — Banner Messages  
  ↳ *Used in:* Q23
- Module 2.5.1 — Configuration Files  
  ↳ *Used in:* Q26
- Module 2.7.3 — Verify Windows PC IP Configuration (ipconfig)  
  ↳ *Used in:* Q15

### Module 3 — Related questions: Q2, Q9, Q12, Q19, Q31, Q36, Q40, Q41, Q45
- Module 3.1.5–3.1.10 — Network Protocol Requirements (encoding/size/timing/delivery)  
  ↳ *Used in:* Q40
- Module 3.1.6 — Message Encoding  
  ↳ *Used in:* Q12
- Module 3.1.8 — Message Size  
  ↳ *Used in:* Q12
- Module 3.5.3 — TCP/IP Protocol Model  
  ↳ *Used in:* Q41
- Module 3.5.4 — OSI and TCP/IP Model Comparison  
  ↳ *Used in:* Q45
- Module 3.6 — Encapsulation  
  ↳ *Used in:* Q19
- Module 3.6.3 — Protocol Data Units  
  ↳ *Used in:* Q9
- Module 3.6.5 — De-encapsulation Example  
  ↳ *Used in:* Q31
- Module 3.7.10 — Lab: Use Wireshark to View Network Traffic  
  ↳ *Used in:* Q36
- Module 3.7.7 — Role of the Data Link Layer Addresses (Different IP Networks)  
  ↳ *Used in:* Q2

### Module 4 — Related questions: Q1, Q37, Q48, Q53, Q60
- Module 4.3.1 — Characteristics of Copper Cabling  
  ↳ *Used in:* Q53
- Module 4.4.1 — Properties of UTP Cabling  
  ↳ *Used in:* Q53
- Module 4.4.1 — Properties of UTP Cabling (Attenuation)  
  ↳ *Used in:* Q60
- Module 4.4.1–4.4.2 — Properties/Standards of UTP Cabling  
  ↳ *Used in:* Q37
- Module 4.4.2 — UTP Cabling Standards and Connectors  
  ↳ *Used in:* Q1
- Module 4.4.4 — Activity: Cable Pinouts  
  ↳ *Used in:* Q1
- Module 4.6.2 — Types of Wireless Media  
  ↳ *Used in:* Q48

### Module 6 — Related questions: Q7, Q9, Q44, Q54
- Module 6.2.7 — Contention-Based Access - CSMA/CD  
  ↳ *Used in:* Q44
- Module 6.3.2 — Frame Fields  
  ↳ *Used in:* Q9
- Module 6.3.2 — Frame Fields (FCS)  
  ↳ *Used in:* Q54
- Module 6.3.3 — Layer 2 Addresses  
  ↳ *Used in:* Q7

### Module 7 — Related questions: Q7, Q19, Q21, Q54, Q55
- Module 7.1 — Ethernet Encapsulation  
  ↳ *Used in:* Q19
- Module 7.1.2–7.1.3 — Data Link Sublayers / MAC Sublayer  
  ↳ *Used in:* Q55
- Module 7.1.4 — Ethernet Frame Fields  
  ↳ *Used in:* Q54
- Module 7.2.2 — Ethernet MAC Address  
  ↳ *Used in:* Q7
- Module 7.4.1 — Frame Forwarding Methods on Cisco Switches  
  ↳ *Used in:* Q21

### Module 8 — Related questions: Q2, Q4, Q6, Q8, Q9, Q16, Q19, Q29, Q31, Q33
- Module 8.1.2 — IP Encapsulation  
  ↳ *Used in:* Q19
- Module 8.1.3 — Characteristics of IP  
  ↳ *Used in:* Q33
- Module 8.2.2 — IPv4 Header Fields (TTL)  
  ↳ *Used in:* Q29
- Module 8.2.2 — IPv4 Packet Header Fields  
  ↳ *Used in:* Q9
- Module 8.4.2 — Default Gateway  
  ↳ *Used in:* Q2, Q4
- Module 8.4.4 — Host Routing Tables  
  ↳ *Used in:* Q16
- Module 8.5 — Introduction to Routing  
  ↳ *Used in:* Q8
- Module 8.5.1 — Router Packet Forwarding Decision  
  ↳ *Used in:* Q31
- Module 8.5.2 — IP Router Routing Table  
  ↳ *Used in:* Q6
- Module 8.5.6 — Introduction to an IPv4 Routing Table  
  ↳ *Used in:* Q6

### Module 9 — Related questions: Q18, Q20
- Module 9.2.1–9.2.2 — ARP Overview / ARP Functions  
  ↳ *Used in:* Q20
- Module 9.2.3–9.2.4 — ARP Request / ARP Reply  
  ↳ *Used in:* Q18

### Module 10 — Related questions: Q4, Q52
- Module 10.3.1 — Default Gateway on a Host  
  ↳ *Used in:* Q4
- Module 10.3.2 — Default Gateway on a Switch  
  ↳ *Used in:* Q52

### Module 11 — Related questions: Q8, Q10, Q11, Q27, Q38, Q39, Q56
- Module 11.3.2 — Routing to the Internet (NAT concept)  
  ↳ *Used in:* Q8
- Module 11.3.4 — Special Use IPv4 Addresses  
  ↳ *Used in:* Q27
- Module 11.5 — Subnet an IPv4 Network  
  ↳ *Used in:* Q39, Q56
- Module 11.5.1–11.5.2 — Subnet an IPv4 Network  
  ↳ *Used in:* Q10
- Module 11.7.2 — Minimize Unused Host IPv4 Addresses and Maximize Subnets  
  ↳ *Used in:* Q38
- Module 11.8 — VLSM  
  ↳ *Used in:* Q11

### Module 12 — Related questions: Q17, Q28, Q30, Q50
- Module 12.2 — IPv6 Address Representation  
  ↳ *Used in:* Q17
- Module 12.3.6 — IPv6 GUA Structure  
  ↳ *Used in:* Q17
- Module 12.3.7 — IPv6 LLA  
  ↳ *Used in:* Q30
- Module 12.4.1 — Static GUA Configuration on a Router  
  ↳ *Used in:* Q28
- Module 12.5.6 — EUI-64 Process  
  ↳ *Used in:* Q50

### Module 13 — Related questions: Q29, Q43
- Module 13.1.4 — Time Exceeded  
  ↳ *Used in:* Q29
- Module 13.2.5 — Traceroute - Test the Path  
  ↳ *Used in:* Q43

### Module 14 — Related questions: Q5, Q9, Q16, Q24, Q32, Q35, Q57
- Module 14.1.3–14.1.5 — Transport Layer Protocols (TCP/UDP)  
  ↳ *Used in:* Q32
- Module 14.2.3 — TCP Header Fields  
  ↳ *Used in:* Q9
- Module 14.2.5 — Applications that use TCP  
  ↳ *Used in:* Q24
- Module 14.3 — UDP Overview  
  ↳ *Used in:* Q35
- Module 14.3.4 — Applications that use UDP  
  ↳ *Used in:* Q24
- Module 14.4 — Port Number Groups (Well-known ports)  
  ↳ *Used in:* Q57
- Module 14.4 — Port Numbers (Socket Pairs)  
  ↳ *Used in:* Q5
- Module 14.4.4 — The netstat Command  
  ↳ *Used in:* Q16

### Module 15 — Related questions: Q24, Q42, Q49, Q51, Q58
- Module 15.1.3 — TCP/IP Application Layer Protocols  
  ↳ *Used in:* Q51
- Module 15.3.4 — Email Protocols (SMTP)  
  ↳ *Used in:* Q58
- Module 15.3.4 — SMTP, POP, and IMAP  
  ↳ *Used in:* Q24, Q42
- Module 15.4.1 — Domain Name System  
  ↳ *Used in:* Q49
- Module 15.5.1 — File Transfer Protocol  
  ↳ *Used in:* Q24
- Module 15.5.1 — TFTP  
  ↳ *Used in:* Q24

### Module 16 — Related questions: Q13, Q25, Q46, Q47, Q57, Q59
- Module 16.2.1 — Types of Malware  
  ↳ *Used in:* Q46
- Module 16.2.4 — Denial of Service Attacks  
  ↳ *Used in:* Q59
- Module 16.3.3 — Upgrade, Update, and Patch  
  ↳ *Used in:* Q47
- Module 16.3.4 — Authentication, Authorization, and Accounting (AAA)  
  ↳ *Used in:* Q13
- Module 16.3.7 — Endpoint Security  
  ↳ *Used in:* Q47
- Module 16.4.4 — Enable SSH  
  ↳ *Used in:* Q25, Q57

### Module 17 — Related questions: Q22, Q35, Q36
- Module 17.2.3 — Voice and Video Applications  
  ↳ *Used in:* Q35
- Module 17.3.2 — Protocol Analysis  
  ↳ *Used in:* Q36
- Module 17.4.5 — Network Baseline  
  ↳ *Used in:* Q22



---

<a id="answer-key"></a>
## Answer Key

| Q | Answer | Confidence |
|---:|---|---|
| 1 | *RJ‑45 (8P8C)** | High |
| 2 | L2 destination MAC: Router interface MAC (default gateway on Teachers LAN) | High |
| 3 | *Live audio conference → Financial transactions → Web browsing** | High |
| 4 | *The host cannot communicate with hosts in other networks (off‑subnet).** | High |
| 5 | *Two browser windows; transport layer ensures the right data goes to the right window (process).** | High |
| 6 | 1) It stores information about routes derived from active router interfaces (connected routes). | High |
| 7 | *MAC address** | High |
| 8 | NAT slows IPv4 address depletion (conserves public IPv4 addresses). | High |
| 9 | FCS → L2 Data Link | High |
| 10 | *192.168.1.64/26** | High |
| 11 | A → 192.168.0.0/25 (126 usable) | High |
| 12 | Message sizing → breaking a long message into smaller pieces before sending | High |
| 13 | *Authorization** | High |
| 14 | Must enter privileged EXEC mode first. | High |
| 15 | *`ipconfig`** (or `ipconfig /all` for full details) | High |
| 16 | *`route print` and `netstat -r`** | High |
| 17 | Global routing prefix → network portion assigned by provider/ISP | High |
| 18 | *PC2 sends an ARP reply with its MAC address.** | High |
| 19 | Source/destination MAC addresses are local and change at every routed hop. | High |
| 20 | If the sender knows the destination IP but not MAC for a local destination, it generates an ARP broadcast. | High |
| 21 | *Store‑and‑forward switching** | High |
| 22 | *Network performance baseline** | High |
| 23 | *Exit privileged EXEC mode and press Enter** (to trigger a fresh session prompt). | Medium |
| 24 | FTP → TCP | High |
| 25 | Configure the IP domain name | High |
| 26 | *Saved configuration in NVRAM** | High |
| 27 | Public → 198.133.219.2 | High |
| 28 | *IPv6-enabled interfaces begin sending ICMPv6 Router Advertisements (RAs).** | High |
| 29 | *Router decrements TTL by 1; if it reaches 0, drops packet and sends ICMP Time Exceeded.** | High |
| 30 | *FE80::/10** | High |
| 31 | *Remove Ethernet header; add a new Layer 2 header for the outgoing interface (S0/0/0).** | High |
| 32 | *Port numbering and checksum** | High |
| 33 | does not require a dedicated end‑to‑end connection (connectionless) | High |
| 34 | *Security, Fault tolerance, Quality of service** | High |
| 35 | *Voice and Video** | High |
| 36 | Capture during peak utilization times. | High |
| 37 | *Untwisted wire length is too long.** | High |
| 38 | *255.255.255.224 (/27)** | High |
| 39 | *IP 192.168.10.38 /29 (255.255.255.248), gateway 192.168.10.33** | High |
| 40 | *Message encoding, Delivery options, Message size** | High |
| 41 | *Application, Transport, Internet, Network Access** | High |
| 42 | *Messages stay on the mail server until manually deleted (server‑based mailbox).** | High |
| 43 | There is connectivity between this device and 192.168.100.1. | High |
| 44 | All devices on a segment see data that passes on the medium. | High |
| 45 | *Session, Presentation, Application** | High |
| 46 | *Worm** | High |
| 47 | Update OS and application software | High |
| 48 | *ZigBee** | High |
| 49 | *DNS** | High |
| 50 | *1E6F:65FF:FEC2:BDF8** | High |
| 51 | *DNS and POP** | High |
| 52 | *The switch can be remotely managed from a host on another network.** | High |
| 53 | *Low‑quality cable/connectors and Improper termination** | High |
| 54 | *FCS (Frame Check Sequence)** | High |
| 55 | Implements trailer with frame check sequence (FCS) for error detection | Medium |
| 56 | *255.255.255.0 (/24)** | High |
| 57 | *SSH** | High |
| 58 | *Sending/relaying email (client → server and server → server).** | High |
| 59 | *An attack that slows or crashes a device or network service.** | High |
| 60 | *Loss of signal strength as distance increases.** | High |


---

<a id="netacad-study-map"></a>
## NetAcad Study Map

### Module 1: Networking Today
**Related practice questions:** Q03, Q34, Q48, Q60

- **1.6.4 — Quality of Service** → Q03, Q60
- **1.6.4 — QoS** → Q34, Q60
- **1.6.5 — Network Security** → Q34, Q60
- **1.7.7 — Technology Trends in the Home** → Q48, Q60

### Module 2: Basic Switch and End Device Configuration
**Related practice questions:** Q15, Q23, Q26, Q60

- **2.4.5 — Banner Messages** → Q23, Q60
- **2.5.1 — Configuration Files** → Q26, Q60
- **2.7.3 — Verify Windows PC IP Configuration (ipconfig)** → Q15, Q60

### Module 3: Protocols and Models
**Related practice questions:** Q02, Q09, Q12, Q19, Q31, Q36, Q41, Q45, Q60

- **3.1.6 — Message Encoding** → Q12, Q60
- **3.1.8 — Message Size** → Q12, Q60
- **3.5.3 — TCP/IP Protocol Model** → Q41, Q60
- **3.5.4 — OSI and TCP/IP Model Comparison** → Q45, Q60
- **3.6 — Encapsulation** → Q19, Q60
- **3.6.3 — Protocol Data Units** → Q09, Q60
- **3.6.5 — De-encapsulation Example** → Q31, Q60
- **3.7.7 — Role of the Data Link Layer Addresses (Different IP Networks)** → Q02, Q60
- **3.7.10 — Lab: Use Wireshark to View Network Traffic** → Q36, Q60

### Module 4: Physical Layer
**Related practice questions:** Q01, Q48, Q53, Q60

- **4.3.1 — Characteristics of Copper Cabling** → Q53, Q60
- **4.4.1 — Properties of UTP Cabling** → Q53, Q60
- **4.4.1 — Properties of UTP Cabling (Attenuation)** → Q60, Q60
- **4.4.2 — UTP Cabling Standards and Connectors** → Q01, Q60
- **4.4.4 — Activity: Cable Pinouts** → Q01, Q60
- **4.6.2 — Types of Wireless Media** → Q48, Q60

### Module 6: Data Link Layer
**Related practice questions:** Q07, Q09, Q44, Q54, Q60

- **6.2.7 — Contention-Based Access - CSMA/CD** → Q44, Q60
- **6.3.2 — Frame Fields** → Q09, Q60
- **6.3.2 — Frame Fields (FCS)** → Q54, Q60
- **6.3.3 — Layer 2 Addresses** → Q07, Q60

### Module 7: Ethernet Switching
**Related practice questions:** Q07, Q19, Q21, Q54, Q60

- **7.1 — Ethernet Encapsulation** → Q19, Q60
- **7.1.4 — Ethernet Frame Fields** → Q54, Q60
- **7.2.2 — Ethernet MAC Address** → Q07, Q60
- **7.4.1 — Frame Forwarding Methods on Cisco Switches** → Q21, Q60

### Module 8: Network Layer
**Related practice questions:** Q02, Q04, Q06, Q08, Q09, Q16, Q19, Q29, Q31, Q33, Q60

- **8.1.2 — IP Encapsulation** → Q19, Q60
- **8.1.3 — Characteristics of IP** → Q33, Q60
- **8.2.2 — IPv4 Packet Header Fields** → Q09, Q60
- **8.2.2 — IPv4 Header Fields (TTL)** → Q29, Q60
- **8.4.2 — Default Gateway** → Q02, Q04, Q60
- **8.4.4 — Host Routing Tables** → Q16, Q60
- **8.5 — Introduction to Routing** → Q08, Q60
- **8.5.1 — Router Packet Forwarding Decision** → Q31, Q60
- **8.5.2 — IP Router Routing Table** → Q06, Q60
- **8.5.6 — Introduction to an IPv4 Routing Table** → Q06, Q60

### Module 10: Basic Router Configuration
**Related practice questions:** Q04, Q52, Q60

- **10.3.1 — Default Gateway on a Host** → Q04, Q60
- **10.3.2 — Default Gateway on a Switch** → Q52, Q60

### Module 11: IPv4 Addressing
**Related practice questions:** Q08, Q11, Q27, Q38, Q39, Q56, Q60

- **11.3.2 — Routing to the Internet (NAT concept)** → Q08, Q60
- **11.3.4 — Special Use IPv4 Addresses** → Q27, Q60
- **11.5 — Subnet an IPv4 Network** → Q39, Q56, Q60
- **11.7.2 — Minimize Unused Host IPv4 Addresses and Maximize Subnets** → Q38, Q60
- **11.8 — VLSM** → Q11, Q60

### Module 12: IPv6 Addressing
**Related practice questions:** Q17, Q28, Q30, Q50, Q60

- **12.2 — IPv6 Address Representation** → Q17, Q60
- **12.3.6 — IPv6 GUA Structure** → Q17, Q60
- **12.3.7 — IPv6 LLA** → Q30, Q60
- **12.4.1 — Static GUA Configuration on a Router** → Q28, Q60
- **12.5.6 — EUI-64 Process** → Q50, Q60

### Module 13: ICMP
**Related practice questions:** Q29, Q43, Q60

- **13.1.4 — Time Exceeded** → Q29, Q60
- **13.2.5 — Traceroute - Test the Path** → Q43, Q60

### Module 14: Transport Layer
**Related practice questions:** Q05, Q09, Q16, Q24, Q35, Q57, Q60

- **14.2.3 — TCP Header Fields** → Q09, Q60
- **14.2.5 — Applications that use TCP** → Q24, Q60
- **14.3 — UDP Overview** → Q35, Q60
- **14.3.4 — Applications that use UDP** → Q24, Q60
- **14.4 — Port Numbers (Socket Pairs)** → Q05, Q60
- **14.4 — Port Number Groups (Well-known ports)** → Q57, Q60
- **14.4.4 — The netstat Command** → Q16, Q60

### Module 15: Application Layer
**Related practice questions:** Q24, Q42, Q49, Q51, Q58, Q60

- **15.1.3 — TCP/IP Application Layer Protocols** → Q51, Q60
- **15.3.4 — SMTP, POP, and IMAP** → Q24, Q42, Q60
- **15.3.4 — Email Protocols (SMTP)** → Q58, Q60
- **15.4.1 — Domain Name System** → Q49, Q60
- **15.5.1 — File Transfer Protocol** → Q24, Q60
- **15.5.1 — TFTP** → Q24, Q60

### Module 16: Network Security Fundamentals
**Related practice questions:** Q13, Q25, Q46, Q47, Q57, Q59, Q60

- **16.2.1 — Types of Malware** → Q46, Q60
- **16.2.4 — Denial of Service Attacks** → Q59, Q60
- **16.3.3 — Upgrade, Update, and Patch** → Q47, Q60
- **16.3.4 — Authentication, Authorization, and Accounting (AAA)** → Q13, Q60
- **16.3.7 — Endpoint Security** → Q47, Q60
- **16.4.4 — Enable SSH** → Q25, Q57, Q60

### Module 17: Build a Small Network
**Related practice questions:** Q22, Q35, Q36, Q60

- **17.2.3 — Voice and Video Applications** → Q35, Q60
- **17.3.2 — Protocol Analysis** → Q36, Q60
- **17.4.5 — Network Baseline** → Q22, Q60


