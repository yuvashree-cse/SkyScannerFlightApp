# ✈️ Flight Info UI App (Backpack Android)

A simple Android UI application built using **Kotlin** and **Skyscanner Backpack Design System**, showcasing structured flight information using card-based UI components.

---

## 📱 App Purpose

This app visually represents flight details using a clean and modern UI:

* Flight Number
* Departure Information
* Arrival Information

Built to practice:

* XML-based UI design
* ConstraintLayout positioning
* Backpack UI components

---

# 🎨 UI DESIGN SPECIFICATION (IMPORTANT)

This is the part most people miss — your UI should feel consistent, not random.

---

## 🟦 1. Flight Information Card

### 🧾 Content:

* Flight Number (e.g., AI-202)

### 🧱 Component Structure:

* `BpkCardView`

  * `BpkText`

### 🎯 Typography:

| Element                | Style                    |
| ---------------------- | ------------------------ |
| Title (optional label) | `@style/bpkTextHeading3` |
| Flight Number          | `@style/bpkTextHeading1` |

### 📏 Example:

```
FLIGHT
AI-202
```

---

## 🟨 2. Departure Card

### 🧾 Content:

* Airport Code (e.g., MAA)
* Departure Time (e.g., 14:30)

### 🧱 Structure:

* `BpkCardView`

  * `LinearLayout (vertical)`

    * `BpkText (Airport Code)`
    * `BpkText (Time)`

### 🎯 Typography:

| Element       | Style                       |
| ------------- | --------------------------- |
| Section Title | `@style/bpkTextHeading3`    |
| Airport Code  | `@style/bpkTextHeading1`    |
| Time          | `@style/bpkTextBodyDefault` |

### 📏 Example:

```
DEPARTURE
MAA
14:30
```

---

## 🟩 3. Arrival Card

### 🧾 Content:

* Airport Code (e.g., DXB)
* Arrival Time (e.g., 18:45)

### 🧱 Structure:

Same as Departure Card

### 🎯 Typography:

| Element       | Style                       |
| ------------- | --------------------------- |
| Section Title | `@style/bpkTextHeading3`    |
| Airport Code  | `@style/bpkTextHeading1`    |
| Time          | `@style/bpkTextBodyDefault` |

### 📏 Example:

```
ARRIVAL
DXB
18:45
```

---

# 🧱 FULL UI HIERARCHY

```
ConstraintLayout (root)
│
├── BpkCardView (Flight Info)
│     └── BpkText (Heading1)
│
├── BpkCardView (Departure)
│     └── LinearLayout (vertical)
│           ├── BpkText (Heading3)
│           ├── BpkText (Heading1)
│           └── BpkText (Body)
│
└── BpkCardView (Arrival)
      └── LinearLayout (vertical)
            ├── BpkText (Heading3)
            ├── BpkText (Heading1)
            └── BpkText (Body)
```

---

# 🛠️ TECH STACK

* Kotlin (Android)
* XML Layouts
* ConstraintLayout
* LinearLayout
* Backpack UI (`net.skyscanner.backpack:backpack-android:43.0.0`)
* Android Studio

---

# 📦 GRADLE DEPENDENCY

```gradle
implementation 'net.skyscanner.backpack:backpack-android:43.0.0'
```

---

# 🚀 HOW TO RUN

1. Open project in Android Studio
2. Wait for Gradle sync
3. Click ▶ Run
4. Launch emulator (API 33+)

---

# 🎯 LEARNING OUTCOMES

* Built structured UI using XML
* Learned Backpack design system usage
* Understood typography hierarchy (Heading1, Heading3, Body)
* Practiced ConstraintLayout positioning
* Created reusable UI card patterns
