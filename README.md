# RENTRUCK-PROJECT

## 📁 Project Structure

```
RENTRUCK/
│
├── home.html                # Main dashboard page
├── styles.css              # css (all)
│
├── Tab/                    
│   ├── customers.html
│   ├── reservations.html
│   ├── missions.html
│   ├── drivers.html
│   ├── vehicles.html
│   ├── invoices.html
│   ├── queries.html
│

```

---

## 🧭 Navigation Overview

* `home.html` → Main dashboard
* All other pages are inside `/Tab`
* Navigation sidebar links everything together

---

## 🎨 Styling System

* All pages use a **shared CSS file**:

  ```
  styles.css
  ```

### 🔗 Important Paths

| Page Location | CSS Path        |
| ------------- | --------------- |
| home.html     | `styles.css`    |
| Tab pages     | `../styles.css` |

---

## UI Components

### 1. Dashboard Layout

* Sidebar (left)
* Main content (auto-fit grid)

### 2. Cards

Used everywhere:

```
<div class="card"></div>
```

Optional:

```
<div class="card card-wide"></div>
```

---

### 3. Buttons

| Type            | Class             |
| --------------- | ----------------- |
| Default         | `btn`             |
| Primary (Add)   | `btn btn-primary` |
| Danger (Delete) | `btn btn-danger`  |
| Small           | `btn btn-sm`      |

---

### 4. Tables

Standard structure:

```
<table>
<tr><th>...</th></tr>
<tr><td>...</td></tr>
</table>
```

---

## 🪟 Modal System (IMPORTANT)

We use **popup modals instead of new pages**.

### Example Usage

#### Button

```
<a class="btn btn-primary" onclick="openXXXModal()">+ Add Customer</a>
```

#### Modal

```
<div id="modalName" class="modal">...</div>
```

#### JS

```
openXXXModal()
closeXXXModal()
```

---




## 👥 Team Notes

* All members should follow **same CSS classes**
* Do NOT create separate CSS files
* Keep everything consistent with existing UI

---

## 🚀 How to Run

1. Open project folder in VS Code
2. Install **Live Server extension**
3. Right-click `home.html` → **Open with Live Server**
