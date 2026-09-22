# Networking From First Principles

> **Don't memorize networking. Derive it.**

Most networking resources teach you *what* to memorize.
This one teaches you *why* anything exists to memorize.

This repository derives computer networking from a single
fundamental problem:

> **Independent systems need to communicate.**

Every concept — from IP addresses to cloud VPCs — is introduced
by first presenting the problem it solves, not the definition
to memorize.

---

## The Reasoning Pattern

Every technology in this repo is explained using the same
first-principles chain:

    What problem existed?
         ↓
    Why was the existing system insufficient?
         ↓
    What solution was introduced?
         ↓
    What information does it require?
         ↓
    What decision does it make?
         ↓
    What happens next?

---

## Why This Exists

Networking is usually taught as a collection of facts:

- "A router is a Layer 3 device."
- "TCP is reliable, UDP is not."
- "DNS translates names to IPs."

But facts without reasoning are fragile. They break the moment
you encounter something new.

This repo takes the opposite approach:

**Start with the problem. Derive the solution. Then name it.**

---

## Who This Is For

- **Cloud engineers** who want to understand *why* VPCs, subnets,
  and route tables exist — not just how to configure them
- **DevOps / SREs** who troubleshoot networks daily and want
  deeper intuition
- **Interview candidates** who want to *defend* their answers,
  not recite them
- **Self-taught engineers** who learned tools before foundations
- **Anyone** who has ever asked: *"But why does this exist?"*

---

## Table of Contents

| # | Document | Problem It Solves |
|---|---|---|
| 00 | [Why Networking Exists](00-why-networking-exists.md) | Communication between systems |
| 01 | [The Communication Medium](01-the-medium.md) | How does data physically move? |
| 02 | [Representing Information](02-representation.md) | How is data encoded as signals? |
| 03 | [Addressing](03-addressing.md) | Who is the data for? |
| 04 | [Local Delivery](04-local-delivery.md) | How does data reach nearby devices? |
| 05 | [Scalable Connectivity](05-scalable-connectivity.md) | How do we connect thousands of devices? |
| 06 | [Routing](06-routing.md) | How does data cross between networks? |
| 07 | [Process Identification](07-process-identification.md) | Which app should receive the data? |
| 08 | [Transport Protocols](08-transport.md) | How do we handle loss, order, congestion? |
| 09 | [Naming (DNS)](09-naming.md) | How do humans use meaningful names? |
| 10 | [Automatic Configuration (DHCP)](10-configuration.md) | How do devices join networks easily? |
| 11 | [Security](11-security.md) | How do we control who can communicate? |
| 12 | [Observability](12-observability.md) | How do we know what's happening? |
| 13 | [Troubleshooting](13-troubleshooting.md) | What happens when it fails? |

---

## The Mental Model

                NETWORKING
                     │
                     ▼
          Communication Between Systems
                     │
        ┌────────────┼────────────┐
        ▼            ▼            ▼
    Identify      Deliver       Control
        │            │            │
        ▼            ▼            ▼
    Addresses     Routing       Security
        │            │
        ▼            ▼
     Local       Remote
    Delivery    Delivery
        │            │
        └──────┬─────┘
               ▼
          Applications
               │
               ▼
       Reliable / Suitable
          Communication

---

## Cloud Mapping

Traditional networking concepts map directly to cloud services:

| Concept | AWS | Azure | GCP |
|---|---|---|---|
| Network | VPC | VNet | VPC |
| Subnet | Subnet | Subnet | Subnet |
| Routing | Route Table | Route Table | Route Table |
| Firewall | Security Group / NACL | NSG | Firewall Rules |
| NAT | NAT Gateway | NAT Gateway | Cloud NAT |
| Load Balancing | ALB / NLB | Load Balancer | Cloud LB |
| VPN | Site-to-Site VPN | VPN Gateway | Cloud VPN |

Understanding networking first means understanding cloud
networking — not memorizing cloud services.

---

## How to Use This Repo

1. **Read in order.** Each document builds on the previous one.
2. **Ask the questions.** Every section ends with "Questions You
   Should Be Able to Defend."
3. **Don't memorize.** If you can't explain *why* something exists,
   go back and re-read the problem it solves.
4. **Map to your world.** See how each concept appears in AWS,
   Kubernetes, Linux, or your daily work.

---

## Contributing

Found a concept that could be explained more clearly?
Open an issue or submit a PR. The goal is reasoning, not volume.

---

## License

MIT — use it, share it, teach with it.

---

> *"The most important thing is not the definition.
> It is the way of thinking."*