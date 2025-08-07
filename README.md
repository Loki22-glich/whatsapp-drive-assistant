# 📱 WhatsApp Drive Assistant – Internship Task (Q2)

This project is a WhatsApp-based Drive Assistant built using **n8n.io**, **Twilio**, and **low-code automation**.

It is part of my internship task submission – **Question 2**, where I had to build an automated assistant that can receive WhatsApp commands like `LIST`, `DELETE`, `MOVE`, etc., and send proper responses.

---

## 🛠 Tech Stack

- [n8n.io](https://n8n.io) – Automation platform (free cloud)
- Twilio WhatsApp Sandbox – For sending & receiving messages
- JavaScript – Used inside the n8n Function node

---

## 💬 How it Works

1. A **Webhook** receives the message sent via WhatsApp.
2. A **Function node** parses the message into:
   - `command` (LIST / DELETE / MOVE / SUMMARY)
   - `target` (like a file name or folder)
3. A **Switch node** routes the command
4. A **Set node** builds the reply message
5. A **Twilio node** sends the response to WhatsApp

---

## ✅ Sample Commands

LIST /ProjectX
DELETE /file.txt
MOVE /file.txt /Archive
SUMMARY /Budget2024

---

## 📸 Screenshots

| Screenshot | Description |
|------------|-------------|
| `workflow.png` | Full n8n workflow |
| `function_output.png` | Shows parsed command and target |
| `execution.png` | Confirms that the flow ran successfully |
| `set_node.png` | (Optional) Set node that generates reply |
| `switch_node.png` | (Optional) Rules for each command |

---

## ⚠️ Notes

- Twilio sandbox was used for this demo
- File actions are simulated (no real Drive API used)
- Fully modular and extendable to real cloud storage

---

## 👤 Built by

**Banoth Lokesh**  
B.Tech, IIT Madras  
Internship project submission
