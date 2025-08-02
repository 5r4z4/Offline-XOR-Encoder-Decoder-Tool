# 🔐 XOR Encode & Decode Tool

A simple web-based tool to **XOR encode and decode text**, using a custom key and Base64 encoding.  
Useful for **CTFs**, reverse engineering, or lightweight obfuscation.

---

## ✨ Features

- 🔢 Custom XOR key (0–255)
- 🔁 Encode (XOR + Base64)
- 🔓 Decode (Base64 + XOR)
- ⚡ Instant result display
- 💡 Great for CTF token decoding (like: `e3o=` → `10`)

---
##🖥️ Usage
Open locally
Clone this repo

Open index.html in your browser

Or host it via GitHub Pages, Netlify, or your own server.


## 🧪 Example

**Input:**

- **Text:** `10`  
- **Key:** `74`

**Encoded Output:**
`e3o=`


---

## 🧰 How It Works

### 🔐 Encoding
1. XOR each character’s charCode with the provided key
2. Convert to a byte array
3. Base64-encode the byte stream

### 🔓 Decoding
1. Base64-decode the input string
2. XOR each byte with the same key
3. Convert the bytes back to a readable string

---

## 🚩 CTF Tip

Use this tool to decode session tokens or profile IDs:
eHt6fw== → XOR + Base64 decode → {"role":"user"}
{"role":"admin"} → XOR encode + base64 → Inject in URL

thank you
