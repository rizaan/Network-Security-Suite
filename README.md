# Admin Server & Agent Setup Guide

## Prerequisites

- Windows OS
- Network access between server and agent devices

---

## 1. Start the Admin Server

1. Navigate to the `admin_server` folder.
2. Run `main.exe`.

This will automatically:
- Install all required dependencies
- Start the FastAPI server
- Trigger a **Windows Security Prompt** — click **"Allow"** to permit network access

---

## 2. Set Up the Agent

1. Run `Agent.exe`.
2. When prompted, enter the **Server IP Address**:

   On the server device, open **Command Prompt** and run:
```
   ipconfig
```
   Look for:
```
   Wireless LAN adapter Wi-Fi:
      IPv4 Address. . . . . . . . . . . : 192.168.31.164
```
   Use that IP (e.g., `192.168.31.164`) in the Agent config.

3. Save the config and start the Agent.

---

## 3. Approve the Agent

1. Go to: [https://admin-soc-tool.vercel.app/system-monitoring](https://admin-soc-tool.vercel.app/system-monitoring)
2. In the **Agent Approval** section, find the pending agent.
3. Click **Approve**.

> ✅ Once approved, the agent will begin sending data every **3 seconds**.
