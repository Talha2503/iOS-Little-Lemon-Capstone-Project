# 🍋 Little Lemon — iOS Food Ordering App

<p align="center">
  <img src="https://images.unsplash.com/photo-1515003197210-e0cd71810b5f?auto=format&fit=crop&w=900&q=80" width="700"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white"/>
  <img src="https://img.shields.io/badge/SwiftUI-007AFF?style=for-the-badge&logo=swift&logoColor=white"/>
  <img src="https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=apple&logoColor=white"/>
  <img src="https://img.shields.io/badge/Core%20Data-FFB000?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Xcode-147EFB?style=for-the-badge&logo=xcode&logoColor=white"/>
</p>

## 📱 About the Project

**Little Lemon** is an iOS food ordering application developed with **SwiftUI** as part of the Meta iOS Developer Professional Certificate capstone project.

The application provides users with a simple way to browse the Little Lemon restaurant menu, explore different food categories, search for dishes, and manage their personal profile.

The project brings together the concepts covered throughout the course, including:

- Swift and SwiftUI
- User interface design
- Navigation
- Data persistence
- JSON decoding
- Core Data
- Git and GitHub
- Wireframing and UI design
- State management

---

## 🎯 Project Goals

The main objective of the project is to develop a functional restaurant application while applying modern iOS development practices.

The application focuses on four primary areas:

**🏠 Home**  
A restaurant introduction, search functionality, menu categories, and food listings.

**👤 Onboarding**  
A multi-step registration experience for collecting the user's personal information.

**📋 Menu**  
A browsable collection of restaurant dishes organized by category.

**⚙️ Profile**  
A personal profile where users can view and update their stored information.

---

## 🖼️ Application Preview

### Home Screen

<p align="center">
  <img src="https://images.unsplash.com/photo-1540189549336-e6e99c3679fe?auto=format&fit=crop&w=700&q=80" width="350"/>
</p>

The Home screen introduces Little Lemon and provides access to the restaurant menu.

It includes:

- Restaurant header
- Hero section
- Restaurant description
- Search field
- Menu category filters
- Food menu list

---

### Menu

<p align="center">
  <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=700&q=80" width="350"/>
</p>

Users can browse available dishes and filter the menu using categories such as:

- Starters
- Mains
- Desserts
- Drinks

Each menu item provides a concise overview of the dish.

---

### User Profile

<p align="center">
  <img src="https://images.unsplash.com/photo-1498837167922-ddd27525d352?auto=format&fit=crop&w=700&q=80" width="350"/>
</p>

The Profile screen displays information entered during onboarding.

Users can edit their information, save changes, and log out when required.

---

## 🧭 Application Flow

```text
                ┌─────────────────┐
                │    App Launch   │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │   Onboarding    │
                │   Registration  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │      Home       │
                └───────┬─┬───────┘
                        │ │
              ┌─────────┘ └─────────┐
              ▼                     ▼
       ┌──────────────┐      ┌──────────────┐
       │    Menu      │      │   Profile    │
       └──────────────┘      └──────────────┘

    
    ✨ Main Features
🔐 Onboarding

The onboarding experience guides new users through the registration process.

It allows users to provide information such as:

First name
Last name
Email address
Phone number

The information is then available through the user's profile.

🏠 Home Dashboard

The Home screen provides the main entry point to the application.

It contains:

Little Lemon branding
Restaurant introduction
Hero section
Search functionality
Menu categories
Food listings
🍽️ Menu Categories

The menu can be filtered according to different food categories.

This allows users to quickly find the type of dish they are interested in.

🔎 Search

The application provides a search interface that allows users to locate menu items more efficiently.

👤 Profile Management

Users can access their personal information through the Profile screen.

Changes made to their profile can be retained between application launches.

🚪 Logout

The application provides a logout option that clears the user's stored profile information and returns the application to the appropriate starting state.

🛠️ Technologies Used
Technology	Purpose
Swift	Application programming language
SwiftUI	User interface development
Core Data	Local data persistence
Foundation	Core system functionality
Xcode	iOS development environment
Git	Version control
GitHub	Remote repository

LittleLemonApp
│
├── Assets.xcassets
│
├── Models
│   ├── MenuItem.swift
│   ├── MenuCategory.swift
│   └── UserProfile.swift
│
├── ViewModels
│   ├── MenuViewModel.swift
│   └── UserViewModel.swift
│
├── Views
│   ├── Onboarding
│   ├── Home
│   ├── Menu
│   ├── Profile
│   └── Components
│
├── CoreData
│   ├── Persistence.swift
│   └── UserDataManager.swift
│
├── Utilities
│
├── LittleLemonApp.swift
│
└── LittleLemonApp.xcodeproj


🧩 Architecture Pattern
The application uses an MVVM-style architecture to separate the user interface from application logic.

        ┌───────────────┐
        │     Views     │
        │   SwiftUI UI  │
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │  ViewModels   │
        │ Business Logic│
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │    Models     │
        │  Application  │
        │     Data      │
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │   Core Data   │
        │   Persistence │
        └───────────────┘

🎨 Design System

The application follows the visual identity of Little Lemon.

Color Palette
struct LittleLemonColors {
    static let green = Color(hex: "#495E57")
    static let yellow = Color(hex: "#F4CE14")
    static let orange = Color(hex: "#EE9972")
    static let beige = Color(hex: "#FBDABB")
    static let lightBackground = Color(hex: "#EDEFEE")
    static let darkText = Color(hex: "#333333")
}

The design emphasizes the restaurant's recognizable green and yellow color combination while maintaining strong readability.


📐 UI Design

The application was designed using wireframing principles before implementation.

The wireframe establishes:

Screen hierarchy
Content placement
Navigation structure
Menu organization
Component positioning

The final SwiftUI interface follows the structure defined during the design phase.

💾 Data Management

The application uses local persistence to maintain user information.

Core Data is used to manage stored information, while SwiftUI state management keeps the interface synchronized with the underlying data.

The project also demonstrates working with structured menu data using Swift's Codable functionality.

Example:

struct MenuItem: Codable {
    let title: String
    let amount: Float
    let highlight: String
    let thumbnail: String
}
🔀 Navigation

The application uses SwiftUI navigation components to allow users to move between screens.

The navigation flow includes:

Onboarding
     │
     ▼
   Home
   /   \
  ▼     ▼
Menu   Profile

Users can navigate to previous screens where appropriate using the navigation stack.

🧪 Testing

The application should be manually tested against the main project requirements.

Onboarding
 First launch displays onboarding
 Onboarding contains three pages
 Next button moves between pages
 User information can be entered
 User can complete onboarding
Home
 Header is displayed
 Hero section is displayed
 Restaurant description is visible
 Search field works
 Menu categories are displayed
 Menu items are visible
Profile
 User information is displayed
 Profile information can be edited
 Changes remain after restarting
 Logout clears stored information
Navigation
 Navigation between screens works
 Back navigation works correctly
🚀 Getting Started
Requirements

To build and run this project, you need:

macOS
Xcode
Swift
iOS Simulator or compatible iOS device

Note: Xcode is only available on macOS. Windows users can view and manage the source code through GitHub, but compiling the iOS application requires access to macOS/Xcode.

Clone the Repository
git clone https://github.com/Willie-Conway/Little-Lemon-Food-Ordering-App.git
Open the Project

Open:

LittleLemonApp.xcodeproj

in Xcode.

Run
Select an iOS Simulator.
Select the application target.
Press Run.
Wait for Xcode to build the project.
Test the application in the simulator.
📂 Repository Contents

The repository contains the main application source code along with design resources.

📁 Application Source
📁 Assets
📁 Core Data
📁 SwiftUI Views
📁 ViewModels
📁 Models
📁 Design Resources
📁 Wireframe
📄 README.md
📄 Xcode Project
🎓 Learning Outcomes

This project demonstrates practical knowledge of:

Swift programming
SwiftUI
Declarative UI development
State management
Navigation
Form design
JSON decoding
Core Data
Local persistence
Git
GitHub
UI/UX wireframing
Responsive interface design
Modular application development
🔮 Possible Future Improvements

The application could be extended with additional functionality such as:

Shopping cart
Order checkout
Order history
Favorites
Restaurant location integration
Push notifications
Online ordering
Payment integration
Backend API integration
User authentication
📌 Project Information

Project: Little Lemon Food Ordering App
Platform: iOS
Language: Swift
Framework: SwiftUI
Database: Core Data
Development Environment: Xcode
Version Control: Git / GitHub

🙏 Acknowledgements

This project was developed as part of the Meta iOS Developer Professional Certificate.

Special thanks to:

Meta
Coursera
Apple Developer Documentation
SwiftUI community
iOS development community



