Outelsys – Offline C# RFID Access Control & Messaging System
📌 Project Overview

Outelsys is an offline access control and internal messaging system built entirely in C#.
It manages RFID card-based entry/exit operations, keeps local logs, and allows offline messaging without any internet connection.
Ideal for factories, offices, schools, or any facility where security and independence from the internet are required.
🚀 Features

    Offline Operation – Works entirely without internet; all data is stored locally.

    RFID Access Control – Secure entry/exit via RFID cards connected to a local C# application.

    Local Database – Stores all users, logs, and messages in an offline SQL database (e.g., SQLite / LocalDB).

    Messaging System – Send and receive messages between workstations over a local network or single PC.

    Event Logging – Automatic tracking of every access attempt with date, time, and user ID.

    Admin Panel – Manage users, view logs, and control access permissions.

🛠 Technologies Used

Hardware:

    RFID Reader (Serial/USB)

    RFID Cards/Tags

    PC running Windows

Software:

    Language: C# (.NET Framework / .NET 8)

    Database: SQLite / SQL Server LocalDB (offline mode)

    UI Framework: WinForms or WPF

    Serial Communication: For reading RFID card data from the reader

🔧 How It Works

    RFID Card Scan → The card is read by the RFID reader connected to the PC.

    Authentication → The C# application checks the card ID in the local database.

    Access Decision →

        If authorized → Display access granted message, log the event.

        If not authorized → Deny access, log the attempt.

    Messaging → Staff can send and read messages within the same application.

    Reports → Admin can filter logs by user/date and export them.

📂 Project Structure

/Outelsys
   /Hardware         → RFID reader connection code
   /UI               → Forms/WPF interface
   /Database         → Local SQLite database files
   /Messaging        → Offline message storage and display logic
   Program.cs        → Main entry point

🖼 Screenshots

(Add pictures of your C# application UI, RFID scan event, and admin panel)
📦 Installation

    Install the RFID reader driver.

    Clone or download the Outelsys repository.

    Open the project in Visual Studio.

    Restore NuGet packages (SQLite or SQL Server LocalDB dependencies).

    Run the application and set up the admin account.

🔐 Security

    Offline-only operation for maximum security.

    Local encryption of sensitive data.

    Role-based access (Admin / User).
