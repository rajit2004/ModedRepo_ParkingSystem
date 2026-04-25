# 🅿️ Parking Management System
> An upgraded C++ console application for managing real-world parking operations — built on top of an existing project with significant enhancements in security, validation, pricing logic, and OOP architecture.

![C++](https://img.shields.io/badge/C++-17-blue?style=flat&logo=cplusplus)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat&logo=windows)
![License](https://img.shields.io/badge/License-Open%20Source-green?style=flat)

---

## 📌 About This Project

This repository is an **upgraded fork** of [Rishav123918/Parking_Application_C-](https://github.com/Rishav123918/Parking_Application_C-).

The original project provided a basic parking structure. I extended it with a complete redesign including:

- 🔐 Role-based login with security lockout
- 🧠 Rush-hour dynamic pricing engine
- 🔢 Regex-based number plate validation
- 📁 Persistent file storage with auto-load
- 🧱 Full OOP restructure with 5 dedicated classes
- 🛡️ Input validation across all entry points (dates, times, numerics)

---

## 🚀 Features

### 🔐 Role-Based Access Control
- Admin and Staff login roles
- Password masking using `_getch()`
- Change password functionality
- Security lockout after repeated failed attempts

### 🚗 Vehicle Management
- Add Cars and Bikes with auto-generated tokens
- Duplicate vehicle detection
- Regex-based number plate format validation
- Batch checkout with confirmation prompts

### 💰 Smart Fare Calculation
- Time-based duration computation
- Automatic hourly rounding
- Rush-hour pricing (two peak windows)
- Separate rates for cars and bikes

### 💾 Data Persistence
- All data saved to `parking_data.txt`
- Auto-loaded on every startup
- Saved continuously after each update — no data loss

### 📊 Reporting & Search
- Search vehicle by token number
- Full parking report view
- Revenue summary
- Car vs Bike count breakdown

### ✅ Input Validation
- Date validation with leap year handling
- Time format validation
- Numeric input guards
- Structured, readable console UI

---

## 📌 Pricing Model

| Vehicle | Normal (per hour) | Rush Hour (per hour) |
|---------|:-----------------:|:--------------------:|
| Bike    | Rs 10             | Rs 15                |
| Car     | Rs 20             | Rs 30                |

**Rush Hours:** `09:00 – 11:00` and `17:00 – 20:00`

---

## 🧠 Technical Highlights

**Object-Oriented Design** — 5 dedicated classes:
`Vehicle` · `Time` · `Date` · `SecuritySystem` · `ParkingSystem`

**STL Usage:**
`vector` · `algorithm` · `regex` · `sstream`

**Windows Console API:**
- `_getch()` — masked password input
- `Sleep()` — smooth UI transitions
- `system("cls")` — clean screen control

---

## 🛠️ Tech Stack

- **Language:** C++17
- **Libraries:** Standard Template Library (STL)
- **Storage:** File Handling (`fstream`)
- **Validation:** Regex
- **UI:** Windows Console API

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

Or simply run the included `parking_system.exe` directly on Windows.

### Default Login Credentials

| Role  | Username | Password |
|-------|----------|----------|
| Admin | admin    | admin123 |
| Staff | staff    | staff123 |

> ⚠️ Change passwords after first login using the built-in change password feature.

---

## 🎯 What I Changed from the Original

| Feature | Original | This Version |
|--------|----------|--------------|
| Login system | Basic | Role-based with lockout |
| Pricing | Fixed rate | Rush-hour dynamic pricing |
| Plate validation | None | Regex-based format check |
| Data storage | Basic | Auto-load + continuous save |
| OOP structure | Minimal | 5 dedicated classes |
| Input validation | Partial | Full (dates, times, numerics) |

---

## 👨‍💻 Author

**Ranesh Rajit** — B.Tech Computer Science Student, India

[![GitHub](https://img.shields.io/badge/GitHub-rajit2004-black?style=flat&logo=github)](https://github.com/rajit2004)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-ranesh--kun-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/ranesh-kun)

---

> *Original project by [Rishav123918](https://github.com/Rishav123918/Parking_Application_C-) — extended and upgraded by Ranesh Rajit.*
