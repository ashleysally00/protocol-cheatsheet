# Protocol Cheatsheet

> **Main idea:**  
> *What do I want this device or software to do, and what kind of connection or compatibility do I need to make that happen?*

This quick-reference guide explains protocols — what they are, how they differ from ports and cables, and how to choose the right ones for what you're trying to do.

A **protocol** is a set of rules that define how devices or software communicate — whether it's sending video to a monitor, transferring files between systems, or securing a login. Some protocols operate entirely in software, while others rely on specific hardware to function.
### Why Protocols Matter
---

When you're setting up an **external monitor**, you're really asking:  
**Can my laptop send video, and does this cable support video output?**  
→ You need a protocol like **DisplayPort Alt Mode** over **USB-C** or a classic **HDMI** connection.

When you're working with **machine learning systems** that use microservices (like a model served by an API), you may use **gRPC** — a high-performance protocol for remote procedure calls, especially common in **Google Cloud, TensorFlow Serving, or internal ML workflows**. Alternatively, **HTTP/HTTPS** or **SFTP** can handle large file downloads or remote jobs.

When you want to **secure a login or API call**, you're relying on protocols like **OAuth** or **TLS** — even though you might not see them.

All of these are powered by **protocols** — sets of rules that make devices and software talk to each other effectively.

---

### Protocols by Use Case

| Use Case | Protocols |
|----------|-----------|
| **Web browsing** | HTTP, HTTPS |
| **Secure login/API auth** | TLS, OAuth |
| **Video output** | HDMI, DisplayPort, USB-C (Alt Mode) |
| **File transfer** | FTP, SFTP, SCP, gRPC |
| **Remote ML workflows** | gRPC, HTTP, SFTP |
| **Smart devices** | Bluetooth, Zigbee, Z-Wave |
| **Device control & sync** | MIDI, CEC (for HDMI), USB protocols |

---

### Bonus: Lower-Layer Protocols (Behind the Scenes)

These protocols work below the surface — you don’t usually interact with them directly, but **every higher-level protocol depends on them**.

| Protocol | Layer | Role |
|----------|-------|------|
| **IP (Internet Protocol)** | Network | Routes packets between devices across networks |
| **TCP (Transmission Control Protocol)** | Transport | Ensures reliable, ordered data transfer |
| **UDP (User Datagram Protocol)** | Transport | Faster, less reliable alternative to TCP |

> For example: HTTP relies on TCP, and TLS secures TCP connections.  
> They're all stacked together — this is called the **network protocol stack**.

---

### AI/Model Interaction Protocols

These software-based protocols manage how AI systems (especially language models) interact with external tools, data, memory, and APIs in structured workflows.

| Protocol | Purpose |
|----------|---------|
| **MCP (Model Context Protocol)** | A standardized way for language models to access tools, files, memory, and APIs in structured, context-aware workflows. Used by systems like Claude to interact with real-world data. |
| **OpenAI Tool Calling Schema** | Defines message formats for GPT models to call tools and use the results. JSON-based and used in OpenAI’s assistant API. |
| **LangChain Agent Frameworks** | Organizes tool use, memory, and step-by-step reasoning loops for building agents. Works across many models and APIs. |

#### Comparison Table

| Name | Owner | Open Standard? | Use Case |
|------|-------|----------------|----------|
| **MCP** | Hugging Face | ✅ Yes | Cross-model tool/memory interaction |
| **OpenAI Tool Schema** | OpenAI | ❌ No | GPT-specific tool calling |
| **LangChain Agent Framework** | LangChain | ❌ No | Custom agent building with memory/tools |

> These protocols are key when building tool-using AI systems. MCP aims to standardize the space, while OpenAI and LangChain offer more framework-specific solutions.

### 🧭 Final Thoughts

Understanding protocols helps you choose the **right tools** for your workflow — whether you’re setting up a display, transferring files, building APIs, or securing user data.

Whenever you're confused about a cable, software, or service — try asking:
> “What do I want this to do, and which protocol supports that?”

This cheatsheet gives you a foundation for figuring it out quickly.
