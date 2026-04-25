# 🅿️ Parking Management System

> An upgraded C++ console application for managing real-world parking operations — role-based access, dynamic rush-hour pricing, regex validation, and persistent file storage.

[![C++](https://img.shields.io/badge/C++-17-blue?style=flat&logo=cplusplus)](https://isocpp.org/)
[![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat&logo=windows)](https://github.com/rajit2004/ModedRepo_ParkingSystem)
[![GitHub Sponsors](https://img.shields.io/github/sponsors/rajit2004?style=flat&logo=githubsponsors&color=EA4AAA)](https://github.com/sponsors/rajit2004)
[![Fork](https://img.shields.io/badge/Forked%20%26%20Upgraded-orange?style=flat)](https://github.com/Rishav123918/Parking_Application_C-)

---

## 📌 About This Project

This is an **upgraded fork** of [Rishav123918/Parking_Application_C-](https://github.com/Rishav123918/Parking_Application_C-).

The original provided a basic parking structure. I rebuilt and extended it with:

- 🔐 Role-based login with security lockout
- 🧠 Rush-hour dynamic pricing engine
- 🔢 Regex-based number plate validation
- 📁 Persistent file storage with auto-load on startup
- 🧱 Full OOP redesign with 5 dedicated classes
- 🛡️ Complete input validation (dates, times, numerics)

---

## 📸 Screenshots

|  |  |
|--|--|
| **Login & Dashboard** | **Vehicle Entry** |
| **Fare Calculation** | **Parking Report** |

---

## 🚀 Features

- 🔐 **Role-Based Access** — Admin and Staff login with password masking and lockout
- 🚗 **Vehicle Management** — Add Cars/Bikes, auto-generated tokens, duplicate detection
- 💰 **Smart Fare Calculation** — Time-based, hourly rounding, rush-hour pricing
- 💾 **Data Persistence** — Auto-saved to `parking_data.txt`, loaded on every startup
- 📊 **Reporting & Search** — Token search, revenue summary, car/bike breakdown
- ✅ **Input Validation** — Dates (leap year), times, numerics, number plate format

---

## 🧠 How It Works

```
User logs in (Admin / Staff)
        ↓
Add vehicle entry → token auto-generated
        ↓
System tracks duration from entry time
        ↓
Rush-hour check → applies dynamic pricing
        ↓
Checkout → fare calculated + data saved to file
        ↓
Reports & revenue summary available anytime
```

---

## 📌 Pricing Model

| Vehicle | Normal (per hour) | Rush Hour (per hour) |
|---------|:-----------------:|:--------------------:|
| Bike    | Rs 10             | Rs 15                |
| Car     | Rs 20             | Rs 30                |

**Rush Hours:** `09:00 – 11:00` and `17:00 – 20:00`

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Language | C++17 |
| Data Structures | STL (`vector`, `algorithm`, `sstream`) |
| Validation | Regex (`<regex>`) |
| Storage | File Handling (`fstream`) |
| UI | Windows Console API |

---

## 🧱 OOP Architecture

**5 dedicated classes:**

`Vehicle` · `Time` · `Date` · `SecuritySystem` · `ParkingSystem`

**Windows Console enhancements:**
- `_getch()` — masked password input
- `Sleep()` — smooth UI transitions
- `system("cls")` — clean screen control

---

## 🎯 What I Changed from the Original

| Feature | Original | This Version |
|---------|----------|--------------|
| Login system | Basic | Role-based with lockout |
| Pricing | Fixed rate | Rush-hour dynamic pricing |
| Plate validation | None | Regex-based format check |
| Data storage | Basic | Auto-load + continuous save |
| OOP structure | Minimal | 5 dedicated classes |
| Input validation | Partial | Full (dates, times, numerics) |

---

## 📂 Project Structure

```
ModedRepo_ParkingSystem/
├── parking1.cpp           # Full application source
├── parking_system.exe     # Prebuilt Windows executable
└── README.md
```

---

## ⚡ Getting Started

### Prerequisites
- Windows OS
- g++ compiler (MinGW) or MSVC

### Compile & Run

```bash
g++ parking1.cpp -o parking_system.exe -std=c++17
./parking_system.exe
```

Or run the included `parking_system.exe` directly on Windows.

---

## 💖 Support This Project

This project is completely free and open source. If you found it useful or want to support more projects like this:

[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-pink?style=for-the-badge&logo=githubsponsors)](https://github.com/sponsors/rajit2004)

---

## 👨‍💻 Author

**Ranesh Rajit** — B.Tech CS Student, India

[![GitHub](https://img.shields.io/badge/GitHub-rajit2004-black?style=flat&logo=github)](https://github.com/rajit2004)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-ranesh--kun-blue?style=flat&logo=linkedin)](https://linkedin.com/in/ranesh-kun)

---

> *Original project by [Rishav123918](https://github.com/Rishav123918/Parking_Application_C-) — extended and upgraded by Ranesh Rajit.*
