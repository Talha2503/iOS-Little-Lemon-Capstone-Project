# 🍋 Little Lemon Food Ordering App — iOS Capstone Project

<p align="center">
  <img src="https://raw.githubusercontent.com/Talha2503/iOS-Little-Lemon-Capstone-Project/main/little-lemon-app/Little%20Lemon%20App%20Assets/Little%20Lemon.jpg" width="280" />
</p>

<p align="center">
  <strong>Meta iOS Developer Professional Certificate — Capstone Project</strong>
</p>

<p align="center">
  A SwiftUI-based iOS food ordering application inspired by the Little Lemon restaurant.
</p>

---

## 📱 Project Overview

The **Little Lemon Food Ordering App** is an iOS application developed as the final capstone project of the **Meta iOS Developer Professional Certificate**.

The application provides users with a simple and intuitive experience for browsing restaurant menu items, viewing categories, managing their profile, and navigating through different sections of the application.

The project demonstrates fundamental and intermediate concepts of **Swift, SwiftUI, Git, Core Data, navigation, UI design, and data persistence**.

---

## ✨ Features

### 🏠 Home Screen

The Home screen is organized into the main sections required by the project:

- Header
- Hero section
- Restaurant description
- Search functionality
- Menu category selection
- Food menu list
- Menu item summaries

### 👋 Onboarding

The application includes a multi-step onboarding experience where users can enter their personal information.

- Three onboarding pages
- Next button navigation
- User information collection
- Form validation
- Persistent user data

### 👤 Profile

The Profile section allows users to view and update their personal information.

- First name
- Last name
- Email
- Phone number
- Profile information
- Persistent changes
- Logout functionality

### 🍽️ Menu

Users can browse different menu categories and view available food items.

Supported categories include:

- Starters
- Mains
- Desserts
- Drinks

Menu items include relevant information such as:

- Name
- Description
- Price
- Category
- Image

### 🔎 Search

The Home screen includes search functionality that allows users to quickly find menu items.

### 💾 Data Persistence

User information can be stored and retrieved using Apple's built-in persistence technologies.

The project demonstrates the use of:

- Core Data
- UserDefaults
- SwiftUI state management

---

## 🎨 Design

The application follows the visual identity associated with Little Lemon.

### Color Palette

| Color | Hex |
|---|---|
| Little Lemon Green | `#495E57` |
| Little Lemon Yellow | `#F4CE14` |
| Secondary Orange | `#EE9972` |
| Secondary Beige | `#FBDABB` |
| Light Gray | `#EDEFEE` |
| Dark Gray | `#333333` |

### Typography

The design uses typography inspired by the Little Lemon design system:

- **Markazi Text** — Headings
- **Karla** — Body text and navigation

---

## 🖼️ Project Screens

<p align="center">
  <img src="https://raw.githubusercontent.com/Talha2503/iOS-Little-Lemon-Capstone-Project/main/little-lemon-app/Little%20Lemon%20App%20Assets/Wireframe.png" width="180" />
  <img src="https://raw.githubusercontent.com/Talha2503/iOS-Little-Lemon-Capstone-Project/main/little-lemon-app/Little%20Lemon%20App%20Assets/Greek%20salad.png" width="180" />
  <img src="https://raw.githubusercontent.com/Talha2503/iOS-Little-Lemon-Capstone-Project/main/little-lemon-app/Little%20Lemon%20App%20Assets/Bruschetta.png" width="180" />
  <img src="https://raw.githubusercontent.com/Talha2503/iOS-Little-Lemon-Capstone-Project/main/little-lemon-app/Little%20Lemon%20App%20Assets/Hero%20image.png" width="180" />
</p>

---

## 🧱 Project Structure

```text
iOS-Little-Lemon-Capstone-Project/
│
├── little-lemon-app/
│   │
│   ├── Assets.xcassets/
│   │   ├── AppIcon.appiconset/
│   │   ├── Logo.imageset/
│   │   ├── Hero Image.imageset/
│   │   └── Menu Item Images/
│   │
│   ├── CoreData/
│   │   ├── Persistence.swift
│   │   └── UserDataManager.swift
│   │
│   ├── Models/
│   │   ├── MenuItem.swift
│   │   ├── MenuCategory.swift
│   │   └── UserProfile.swift
│   │
│   ├── Views/
│   │   ├── Onboarding/
│   │   ├── Home/
│   │   ├── Menu/
│   │   ├── Profile/
│   │   └── Components/
│   │
│   ├── ViewModels/
│   │   ├── MenuViewModel.swift
│   │   └── UserViewModel.swift
│   │
│   ├── Utilities/
│   │   ├── Constants.swift
│   │   ├── Extensions.swift
│   │   └── Validators.swift
│   │
│   └── LittleLemonApp.swift
│
├── Design Assets/
│   ├── Canvas_Wireframe.fig
│   ├── Canvas_Wireframe_Final.fig
│   └── my-wireframe.pdf
│
├── Screenshots/
│   ├── Onboarding.png
│   ├── Home.png
│   ├── Profile.png
│   └── Menu Detail.png
│
├── README.md
└── LittleLemonApp.xcodeproj
