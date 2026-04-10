# WhatsApp Queue Sender (Client‑Side)

A **privacy‑first, client‑side web app** for sending WhatsApp messages to a list of contacts **one by one** using WhatsApp Desktop or WhatsApp Web.

✅ No server  
✅ No database  
✅ No third‑party services  
✅ No contact data stored  
✅ Works on GitHub Pages  

This tool is designed for **manual, compliant sending**, similar to tools like Privyr — but without uploading personal data to external platforms.

---

## ✨ Features

- 📄 Upload contacts via CSV (client‑side only)
- 👥 Queue‑style contact launcher
- 💬 WhatsApp‑style message formatting preview
- 🔗 Opens chats via official `wa.me` links
- ✅ Visual status tracking (Pending / Opened / Sent)
- 🔒 Strong privacy guarantees (no storage, no network calls)

---

## 🚫 What This Tool Does NOT Do

To stay safe and compliant with WhatsApp rules, this app **intentionally does not**:

- ❌ Auto‑send messages
- ❌ Send bulk messages automatically
- ❌ Attach files or images automatically
- ❌ Store contacts locally or online
- ❌ Use WhatsApp Business APIs

You **must manually click “Send”** in WhatsApp.

---

## 🖥️ How It Works

1. You upload a CSV file containing contacts
2. The file is parsed **entirely in your browser**
3. Contacts appear in a send queue
4. You click **Open in WhatsApp**
5. WhatsApp Desktop / Web opens with:
   - The correct contact
   - A pre‑filled message
6. You click **Send**
7. Back in the app, you mark the message as **Sent**

---

## 📁 CSV File Format

Your CSV file must use **exactly these headers** (case‑sensitive):

- `Name`
- `ContactNumber`

### ✅ Example CSV

```csv
Name,ContactNumber
Anthony Loh,6591234567
Jane Tan,6588123456
