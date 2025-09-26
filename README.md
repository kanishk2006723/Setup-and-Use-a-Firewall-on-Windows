# Setup-and-Use-a-Firewall-on-Windows
Here's a brief summary of how a firewall filters traffic, based on the provided document.

### Firewall Filtering Process

A firewall acts as a digital gatekeeper, inspecting all data packets that try to cross its boundary. The process begins with **Packet Arrival**, where the firewall intercepts a packet and extracts key details like its source IP, protocol, and port numbers.

Next, through **Stateful Inspection**, the firewall determines if the packet is part of an existing, approved connection. If it is, the packet is immediately allowed to pass.If not, the firewall proceeds to its list of rules.

In **Rule-Based Evaluation**, the packet is compared against the rules in a top-down order, and the first matching rule is executed. The rule's action can be **ALLOW** (the packet is forwarded), **DENY** (the packet is silently dropped), or **REJECT** (the packet is dropped with an error message sent back). Finally, if no rule matches, the firewall applies its **Default Deny** policy, blocking the traffic.
