# ♻️ RecyclingFX – JavaFX Recycling Voucher Application  

## 📖 Overview  
**RecyclingFX** is a JavaFX desktop application that simulates a recycling machine where users can:  
- Add recyclable items (cans & bottles).  
- See their total value in real time.  
- Export a **voucher** with item breakdown & totals.  
- Format totals according to **Ireland, France, or Germany**.  

The project demonstrates **UI Design Principles** (consistency, proximity, hierarchy, feedback) and uses **multithreading** to keep the UI responsive during long-running tasks.  

---

## ✨ Features  

✅ **Add Items**  
- `Add Can` → adds €0.15  
- `Add Bottle` → adds €0.25  
- GIF animation plays on each action  

✅ **Voucher Generation**  
- Click **Finish** → exports voucher as `.txt` file  
- Uses **Task + Thread** for smooth background execution  
- **ProgressBar** shows export status  

✅ **Currency Formatting (Extra Feature)**  
- Dropdown menu to switch between:  
  - 🇮🇪 Ireland (€1,234.56)  
  - 🇫🇷 France (1 234,56 €)  
  - 🇩🇪 Germany (1.234,56 €)  

✅ **Quit Button (Extra Feature)**  
- Instantly exits the app  

✅ **User Feedback**  
- Alerts for successful export, empty list, or errors  
- Intuitive grouping of buttons  
- Visual cues with hover/focus states  

---

## 🖼️ Screenshots  

### Main UI  
![Main UI Screenshot](<img width="977" height="737" alt="image" src="https://github.com/user-attachments/assets/0801f2b1-31c1-436d-96e6-db3d0e40d95a" />
)  

### Voucher Export Example  
![Voucher Export Screenshot](<img width="980" height="736" alt="image" src="https://github.com/user-attachments/assets/eac6eb6f-08ac-4b8b-8d44-3817d4d9a3ef" />
)  

---

## 🛠️ Tech Stack  

- **Java 17+**  
- **JavaFX 17+**  
- **Scene Builder** (for designing layouts, optional)  

**Layout Containers:**  
- `VBox (vbMain)` – stacks menu bar & content vertically  
- `GridPane (gp)` – positions labels, buttons, ListView, ImageView, and ProgressBar  

**Naming Convention:**  
- Hungarian notation + camelCase (e.g., `btnAddCan`, `lvItems`, `progBar`)  

---

## 🚀 Getting Started  

### Prerequisites  
- Install [Java 17 or later] 
- Install [JavaFX SDK]
- A Java IDE (IntelliJ / Eclipse / NetBeans)  

### Run the Application  
Clone the repo and run it locally:  

```bash
# Clone repository
git clone https://github.com/your-AnrielAlm/RecyclingFX.git

# Navigate into project
cd RecyclingFX

# Compile & run (example for IntelliJ or using command line)
javac --module-path /path/to/javafx-sdk/lib --add-modules javafx.controls RecyclingFX.java
java --module-path /path/to/javafx-sdk/lib --add-modules javafx.controls RecyclingFX
