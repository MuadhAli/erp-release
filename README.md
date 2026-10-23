# Madina Store ERP — Official Releases

Official production release repository for **Madina Store ERP** desktop application.

## 📦 Latest Release: v1.0.0

- **Setup Installer:** [Madina-Store-ERP-Setup-1.0.0.exe](https://github.com/MuadhAli/erp-release/releases/latest)
- **Architecture:** Windows x64 (NSIS Installer)
- **Release Date:** October 2026

---

## 🚀 Installation & Setup Guide

### 1. Branch Server PC (Main PC in the shop)
1. Install MariaDB (or MySQL) on port 3306 or 3307 as a Windows Service.
2. Run Madina-Store-ERP-Setup-1.0.0.exe.
3. In Setup, select **Branch Server**, enter your Branch Code (e.g. MB), local DB credentials, and Cloud Hostinger sync details.
4. Open port 4000 on Windows Firewall (Inbound Rules) so cashier tills on the LAN can reach it.

### 2. Cashier Till PCs (Counters)
1. Run Madina-Store-ERP-Setup-1.0.0.exe.
2. In Setup, select **Till**, enter the Branch PC LAN address (e.g. http://192.168.1.50:4000) and Till Code (e.g. T2).
3. **No MariaDB or database needed** on cashier tills!

---

## 🔄 In-App Updates
Users can check for the latest updates directly in the app:
1. Click the **User Profile avatar** in the top navigation bar.
2. Select **Check for Updates**.
3. View the latest release notes and download the newest installer with one click!
