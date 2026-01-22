# 🚚 Transport Layer (OSI Layer 4) – 
---

## 1️⃣ What is the Transport Layer?

The **Transport Layer** is the **4th layer of the OSI model**.

**Simple definition:**

> The Transport Layer is responsible for **end-to-end communication between applications**, ensuring data is delivered correctly.

It sits **between the Application/Session layers and the Network layer**.

---

## 2️⃣ What Does the Transport Layer Do?

The Transport Layer handles:

### ✅ Port Numbers

* Identifies **which application** should receive the data

Example:

```
IP address → Machine
Port number → Application
```

---

### ✅ Segmentation & Reassembly

* Breaks large data into **small segments**
* Reassembles them at the destination

---

### ✅ Flow Control

* Prevents sender from overwhelming receiver

---

### ✅ Error Control

* Detects lost or corrupted data
* Retransmits if needed (TCP)

---

## 3️⃣ TCP vs UDP (MOST IMPORTANT TOPIC)

### 🔹 TCP (Transmission Control Protocol)

* Reliable
* Connection-oriented
* Guarantees delivery
* Ordered data transfer

**Used for:**

* HTTP / HTTPS
* SSH
* FTP
* Databases

---

### 🔹 UDP (User Datagram Protocol)

* Fast
* Connectionless
* No delivery guarantee
* No ordering

**Used for:**

* Streaming
* DNS queries
* Monitoring & metrics

---

### 🔍 TCP vs UDP Comparison

| Feature     | TCP       | UDP            |
| ----------- | --------- | -------------- |
| Reliability | Yes       | No             |
| Speed       | Slower    | Faster         |
| Connection  | Required  | Not required   |
| Use cases   | Web, APIs | Streaming, DNS |

---

## 4️⃣ Common Port Numbers (INTERVIEW MUST-KNOW)

| Service    | Port |
| ---------- | ---- |
| HTTP       | 80   |
| HTTPS      | 443  |
| SSH        | 22   |
| FTP        | 21   |
| SMTP       | 25   |
| MySQL      | 3306 |
| PostgreSQL | 5432 |
| Jenkins    | 8080 |

---

## 5️⃣ Real-World Example (Very Important)

### Accessing a Website

```
Browser → TCP Connection → Server IP:443 → HTTPS Response
```

Here:

* TCP ensures reliable delivery
* Port 443 identifies HTTPS

---

## 6️⃣ Transport Layer in DevOps (REAL USE CASES)

### 🔹 Web Applications

* HTTP/HTTPS traffic (TCP)

### 🔹 APIs & Microservices

* Service-to-service communication

### 🔹 CI/CD Tools

* Jenkins (8080)
* Git (SSH on 22)

### 🔹 Monitoring

* Metrics via UDP

---

## 7️⃣ Linux Commands Related to Transport Layer

```bash
netstat -tuln
ss -tuln
lsof -i :8080
```

Used to:

* Check open ports
* Verify services
* Debug connectivity

---

## 8️⃣ Common Failure Scenarios (DevOps Thinking)

### Problem: Website not accessible

Possible Transport Layer issues:

* Wrong port
* Service not listening
* Firewall blocking port

---

ew-ready.**

