# HTTP vs HTTPS Protocol

## 📌 Overview

This repository explains the difference between **HTTP (HyperText Transfer Protocol)** and **HTTPS (HyperText Transfer Protocol Secure)**.

HTTP and HTTPS are protocols used for communication between a **client (such as a web browser)** and a **web server**. HTTPS is the secure version of HTTP and protects data using encryption.

---

## 🌐 What is HTTP?

**HTTP (HyperText Transfer Protocol)** is a protocol used to transfer data between a client and a web server.

When you visit a website using HTTP, the information exchanged between your browser and the server is sent in **plain text**.

### Example

```text
http://example.com
```

### Features of HTTP

* Uses port **80**
* Data is transferred without encryption
* Faster than HTTPS in some situations because there is no encryption overhead
* Data can potentially be intercepted by attackers
* Does not provide strong data confidentiality

---

## 🔐 What is HTTPS?

**HTTPS (HyperText Transfer Protocol Secure)** is the secure version of HTTP.

HTTPS uses **TLS (Transport Layer Security)** to encrypt communication between the client and the server.

### Example

```text
https://example.com
```

### Features of HTTPS

* Uses port **443**
* Encrypts data using TLS
* Protects sensitive information
* Helps prevent data interception and tampering
* Uses a digital certificate to authenticate the website
* Provides better security for users

---

## ⚖️ HTTP vs HTTPS

| Feature                     | HTTP                        | HTTPS                              |
| --------------------------- | --------------------------- | ---------------------------------- |
| Full Form                   | HyperText Transfer Protocol | HyperText Transfer Protocol Secure |
| Security                    | Not secure                  | Secure                             |
| Encryption                  | ❌ No                        | ✅ Yes                              |
| Default Port                | 80                          | 443                                |
| TLS/SSL                     | ❌ No                        | ✅ Yes                              |
| Data Protection             | Low                         | High                               |
| Certificate                 | Not required                | Required                           |
| Suitable for Sensitive Data | ❌ No                        | ✅ Yes                              |
| URL                         | `http://`                   | `https://`                         |

---

## 🔄 How HTTP Works

The basic communication process is:

```text
Client/Browser
      |
      | HTTP Request
      ↓
Web Server
      |
      | HTTP Response
      ↓
Client/Browser
```

The data exchanged through HTTP is not encrypted.

---

## 🔒 How HTTPS Works

HTTPS adds a secure TLS layer between the client and server:

```text
Client/Browser
      |
      | Secure HTTPS Connection
      ↓
    TLS
      |
      ↓
Web Server
```

The communication is encrypted so that unauthorized users cannot easily read or modify the transmitted data.

---

## 🛡️ Why HTTPS is Important

HTTPS is especially important when handling sensitive information such as:

* 🔑 Passwords
* 💳 Credit/Debit card details
* 🏦 Banking information
* 📧 Email and personal information
* 🔐 Login credentials
* 🛒 Online payment information

---

## 📜 Simple Example

### HTTP

```text
Browser → HTTP → Server

"username=John&password=12345"
```

The information is transmitted without encryption.

### HTTPS

```text
Browser → HTTPS/TLS → Server

"Encrypted Data"
```

The information is encrypted during transmission.

---

## 🚀 Advantages of HTTPS

1. **Data Encryption**
   Protects information exchanged between the browser and server.

2. **Authentication**
   TLS certificates help verify that the user is communicating with the intended website.

3. **Data Integrity**
   Helps prevent data from being modified during transmission.

4. **Better Security**
   Provides protection for sensitive information.

5. **User Trust**
   Browsers indicate secure HTTPS connections, helping users recognize protected connections.

---

## ⚠️ Disadvantages of HTTP

* Data is not encrypted.
* Information can potentially be intercepted.
* Vulnerable to certain types of attacks.
* Not suitable for sensitive information.
* Users cannot rely on HTTP alone to verify the server's identity.

---

## 💡 Key Difference

The main difference is:

> **HTTP transfers data without encryption, while HTTPS uses TLS to encrypt and secure the communication between the client and server.**

---

## 🧑‍💻 Technologies Used

* HTTP
* HTTPS
* TLS
* Web Browser
* Web Server
* Digital Certificates

---

## 📚 Conclusion

HTTP and HTTPS are communication protocols used on the web. HTTP is the basic protocol, while HTTPS provides an additional security layer using TLS.

For modern websites, **HTTPS should be used whenever secure communication is required**, especially when users submit personal or sensitive information.

---

## ⭐ HTTP vs HTTPS at a Glance

```text
HTTP
 ↓
No Encryption
 ↓
Port 80
 ↓
Less Secure


HTTPS
 ↓
TLS Encryption
 ↓
Port 443
 ↓
More Secure
```

---

## 👨‍💻 Author

**Balsingh H**

This repository is created for learning and understanding the fundamentals of **HTTP and HTTPS protocols**.
