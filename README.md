# IMADEXAM
# 🌲 Campsite Commander

**Campsite Commander** is an Android application built using **Kotlin** in Android Studio.  
It helps users manage and organise camping gear and food supplies for outdoor adventures using a structured checklist system.

The app demonstrates the use of **arrays, loops, screen navigation, and user input handling**.

---

## 📱 App Overview

This app allows users to:
- Add camping gear and supplies
- Categorise items (e.g. Shelter, Cooking, First Aid, Food)
- View a detailed packing checklist
- Calculate total items packed using loops
- Navigate smoothly between multiple screens

---

## 🎯 Objective

To build an inventory-style app for outdoor trips called **Campsite Commander**, where users can:
- Store gear using parallel arrays
- Organise items by category
- Track quantities and notes
- View a full packing checklist

---

## 🧩 Features

### 🟢 Splash Screen
- Displays app logo (campfire / pine tree theme)
- Shows title: **Campsite Commander**
- Automatically navigates to Main Screen after **3 seconds (3000ms)**

---

### 🏕️ Main Screen
- Button: **Add Gear**
- Displays **Total Items Packed**
  - Calculated using a **loop through arrays**
- Nature-themed / dark mode UI design

---

### 📋 Detailed View Screen
- Displays full list of items:
  - Item Name
  - Category
  - Quantity
  - Comments / Notes
- Includes **Back to Base** button for navigation

---

## 💾 Data Storage

The app uses **parallel arrays**:

```kotlin
var itemNames = arrayOf("Canned Food", "Tent", "Flashlight")
var categories = arrayOf("Food", "Shelter", "Safety")
var quantities = arrayOf(10, 3, 2)
var comments = arrayOf("Beans, fish etc", "One per person", "Check batteries")
🔁 Key Functionality
Loop Example (Total Items Calculation)
var totalItems = 0

for (i in quantities.indices) {
    totalItems += quantities[i]
}
🧭 Navigation Flow
Splash Screen (3s)
        ↓
Main Screen
   ↓        ↓
Add Gear   View Details
              ↓
        Back to Main
⚠️ Error Handling

The app includes:

Input validation for empty fields
Feedback for incorrect or missing entries
Safe array handling to prevent crashes
🎨 UI Design
Dark / nature-inspired theme 🌲🔥
Clean layout with simple navigation
Easy-to-read checklist format
Consistent styling across all screens
🛠️ Tech Stack
Kotlin
Android Studio
XML Layouts / Jetpack Compose (if used)
GitHub Version Control
📦 Project Structure
app/
 ├── MainActivity.kt
 ├── SplashActivity.kt
 ├── AddGearActivity.kt
 ├── DetailActivity.kt
 ├── models/
 ├── layouts/
