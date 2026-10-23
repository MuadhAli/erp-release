# Madina Store ERP — Official Releases

Official release repository for **Madina Store ERP** desktop application.

## 📦 Latest Release: v1.0.0

- **Setup Installer:** [Madina-Store-ERP-Setup-1.0.0.exe](https://github.com/MuadhAli/erp-release/releases/latest)
- **Architecture:** Standalone Autonomous Stations (Every PC runs its own local DB + direct Cloud Sync)
- **Installer Type:** Windows x64 (NSIS Installer)

---

## 🚀 Standalone Installation Guide (Run on Every PC)

Every billing counter / computer in the shop runs **100% independently**. There is **no branch master PC** and **no dependency between computers**. If any computer is turned off or restarted, other computers continue billing with zero interruption.

### Setup Instructions for Each PC:
1. Ensure MariaDB (or MySQL) is installed locally on the computer (127.0.0.1:3306).
2. Run Madina-Store-ERP-Setup-1.0.0.exe.
3. Fill in:
   - **Branch Code:** e.g. MB or MA (identifies the store)
   - **Counter / Till Code:** e.g. T1 on PC 1, T2 on PC 2, T3 on PC 3.
     *(This makes every invoice number permanently unique: MB-T1-00001, MB-T2-00001, with zero collision!)*
   - **Local DB:** Host 127.0.0.1, Port 3306, Database name, User, Password.
   - **Cloud Sync:** Hostinger Cloud credentials (srv2214.hstgr.io).
4. Click **Test connection** and **Save and start**.

---

## ⚡ Direct Cloud Sync & Unique Invoice IDs
- **Instant local billing:** Every bill generates its final, official invoice number immediately upon completion. No temporary IDs, no provisional bills.
- **Direct Cloud Sync:** Every PC connects directly to the Hostinger Cloud DB to pull master prices/products and push sales whenever internet is available.

---

## 🔄 Check for Updates
Users can update the software directly inside the app:
1. Click the **Profile avatar** in the top navigation bar.
2. Click **Check for Updates**.
3. View changelog and download new .exe updates with one click.
