# WhatsApp Queue Sender (Client‑Side)

A **privacy‑first, client‑side web app** for sending WhatsApp messages to a list of contacts **one by one** using WhatsApp Desktop or WhatsApp Web.

✅ No server
✅ No database
✅ No third‑party services
✅ No contact data stored on any server
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
- 💾 **Session Persistence:** Progress is automatically saved to your browser's local storage — reopen the tab and pick up exactly where you left off.
- ↺ **Reset Button:** Clear all saved data and start fresh with a single click.

---

## 🖥️ How It Works

1. **Upload CSV:** Load your list with names, numbers, and up to three custom fields.
2. **Set Template:** Draft your message using placeholders like `Hi {{Name}}, your workshop is at {{Field1}}`.
3. **Filter View:** Use the status chips to focus on specific groups (e.g., hide "Sent" to see remaining tasks).
4. **Launch Chat:** Click **Open in WhatsApp** to open the official `wa.me` link.
5. **Update Status:** Mark contacts as **Sent** or **Invalid** to automatically move to the next person.
6. **Resume Anytime:** If you close or refresh the tab, reopen the app and click **Restore Session** to continue from where you stopped.

---

## 💾 Session Persistence

Progress is saved automatically to your browser's **local storage** after every action — no manual saving needed.

### What is saved
- All contact data (loaded from your CSV)
- The status of every contact (Pending, Opened, Sent, Invalid)
- Your message template
- The currently selected contact

### Restoring a session
When you reopen the app and a previous session is detected, a **yellow banner** appears at the top showing:
- How many contacts were in the session
- How many were completed
- When the session was last saved

Click **Restore Session** to reload everything instantly — no need to re-upload the CSV.  
Click **Start Fresh** to discard the saved session and begin again.

### Resetting manually
Click the **↺ Reset & Clear** button in the top-right corner at any time. A confirmation dialog will appear before anything is deleted. Confirming clears all saved data from local storage and reloads the page.

> **Note:** Local storage is browser- and device-specific. Sessions do not transfer between different browsers or devices.

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
```

---

## 🔒 Privacy

All data stays in your browser. Nothing is uploaded to any server. The only external calls made are:

- Opening `api.whatsapp.com` links to start chats
- Loading the IBM Plex Sans and IBM Plex Mono fonts from Google Fonts (on first load)
