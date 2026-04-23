# WhatsApp Queue Sender (Client‑Side)

A **privacy‑first, client‑side web app** for sending WhatsApp messages to a list of contacts **one by one** using WhatsApp Desktop or WhatsApp Web.

✅ No server
✅ No database
✅ No third‑party services
✅ No contact data stored
✅ Works on GitHub Pages

---

## ✨ Features

- 📄 **CSV Upload:** Load contacts locally in your browser.
- 👥 **Queue Launcher:** Manage outreach one-by-one.
- 🏷️ **Custom Fields:** Use `{{Name}}`, `{{Field1}}`, `{{Field2}}`, and `{{Field3}}` in templates.
- 💬 **Live Preview:** See WhatsApp-style formatting (bold, italics) as you type.
- 🔍 **Selective Filtering:** Show or hide contacts based on status (Pending, Opened, Sent, Invalid).
- 🚫 **Invalid Detection:** Mark and filter out numbers that are not on WhatsApp.
- 📊 **Status Counters:** Real-time counts for each contact category.

---

## 🖥️ How It Works

1. **Upload CSV:** Load your list with names, numbers, and up to three custom fields.
2. **Set Template:** Draft your message using placeholders like `Hi {{Name}}, your workshop is at {{Field1}}`.
3. **Filter View:** Use the checkboxes to focus on specific groups (e.g., hide "Sent" to see remaining tasks).
4. **Launch Chat:** Click **Open in WhatsApp** to open the official `wa.me` link.
5. **Update Status:** Mark contacts as **Sent** or **Invalid** to automatically move to the next person.

---

## 📁 CSV File Format

Your CSV file must include these headers (case-sensitive):

- `Name`
- `ContactNumber` (Include country code, e.g., 65...)
- `Field1`, `Field2`, `Field3` (Optional custom data)

### ✅ Example CSV

```csv
Name,ContactNumber,Field1,Field2,Field3
Anthony Loh,6591234567,Zumba,10am,Sheng Hong AAC
Jane Tan,6588123456,Art Class,2pm,Neighbour Ring
