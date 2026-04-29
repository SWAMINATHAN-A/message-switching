# 📡 Message Switching System

A lightweight **in-memory message broker** that enables communication between distributed clients using queues and RPC-style messaging.

---

## 🚀 Overview

This project implements a **store-and-forward messaging system** where a central server (message switch) routes messages between clients.

It demonstrates key distributed systems concepts like:
- Message Queues  
- Producer–Consumer Model  
- Remote Procedure Calls (RPC)  
- Client–Server Architecture  

---

## 🧠 Features

- 🔁 Named message queues  
- 📬 Store-and-forward delivery  
- 🔗 Correlation IDs for tracking messages  
- 🔄 RPC-style request/response support  
- ⚡ Lightweight in-memory design  
- 🧩 Easily extensible  


- **Server** → Maintains queues and routes messages  
- **Clients** → Act as producers, consumers, or RPC servers  

---

## 📦 Message Format

Each message includes:

- `correlation_id` → Unique ID for tracking  
- `reply_to` → Queue for responses (used in RPC)  
- `payload` → Actual data  

---

## ⚙️ How It Works

### Client Flow

1. Connect to server  
2. Create or subscribe to a queue  
3. Send messages  
4. Receive messages  
5. Acknowledge after processing  

---

### RPC Flow

**Client:**
- Creates a temporary reply queue  
- Sends request  
- Waits for response  

**Server:**
- Listens on queue  
- Processes request  
- Sends response back  
- Acknowledges message  

---



**CONTRIBUTORS**
-Asini31
-chan-dra-k
-Saumya-01git

