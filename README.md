# 🎓 Student Result System

A lightweight, high-performance desktop application built using **.NET MAUI Blazor Hybrid** architecture. This application provides school administrators and teachers with a centralized portal to manage student profiles, log examination marks, and dynamically calculate academic performance grades.

---

## 🏗️ Architecture Overview

Unlike traditional web applications, this app utilizes a hybrid desktop design to execute code locally on the user's machine while rendering a modern user interface using web standards.

* **Native Shell (.NET MAUI):** Manages native Windows application window allocation, OS-level lifecycle events, and secure local file compilation paths.
* **UI Layer (Blazor Webview):** Renders a responsive interface using standard HTML5 and CSS3, eliminating the need for heavy native UI framework dependencies.
* **Layout Context:** Migrated from a traditional vertical layout stack to an expansive, horizontal **Top Navigation Bar Matrix** configured inside the core UI shell.

---
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/d09ea01a-9ae8-4a6a-bad2-03ff55cea8ae" />
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/d6fb35c2-61ce-42cc-977a-2ed28572ff6f" />

## 📂 Project Structure Blueprint

The system architecture cleanly splits data contracts, system utilities, and interface frames into a singular deployment tree to prevent cross-project reference loops:

```text
SimpleTaskApp.Shared/
├── Layout/
│   └── MainLayout.razor       # Core UI Master template (Configured with Top Nav)
├── Models/
│   ├── Student.cs             # Student profile parameters
│   └── MarkRecord.cs          # Academic grading schemas
├── Pages/
│   ├── Home.razor             # Primary administrative entry matrix
│   └── Portal.razor           # Main XYZ School Portal results console
└── _Imports.razor             # Global compilation using directives



