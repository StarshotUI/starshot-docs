# ⭐ Starshot UI Library

Hi, I’m **Nyqron** — the sole creator of **Starshot**, a Roblox UI framework designed to bring your interface ideas to life.  

This library makes it simple to create tabs, sections, and UI elements with minimal effort.  

---

## 🚀 Load the Library

```lua
local UI = loadstring(http:get("https://pastebin.com/raw/Ba2U3X7c"))()
```

---

## 📖 Creating a Tab

```lua
local MainUI = Astra.CreateTab("Astra Demo", "By Creator", "1234", true, "Crimson")
```

**Parameters:**
1. `Astra Demo` → The **title** of your UI  
2. `By Creator` → The **subtitle** (optional credit/description)  
3. `1234` → The **password** string  
4. `true` → Whether a **password is required** (`true` = required, `false` = no password)  
5. `Crimson` → The **theme**  

---

## 📂 Creating a Section

```lua
local Section1 = Astra.CreateSection("General")
local Section2 = Astra.CreateSection("Settings")
```

---

## 🎨 UI Elements

### 🔘 Button
```lua
Astra.CreateButton(Section1, "Click Me", function()
    print("Button clicked!")
end)
```

---

### ✅ Toggle
```lua
Astra.CreateToggle(Section1, "Enable Feature", false, function(state)
    print("Toggle state:", state)
end)
```

---

### 🎚️ Slider
```lua
Astra.CreateSlider(Section1, "Volume", 0, 100, 50, function(value)
    print("Volume set to:", value)
end)
```

---

### ⬇️ Dropdown
```lua
Astra.CreateDropdown(Section2, "Choose Option", {"Option A", "Option B", "Option C"}, function(choice)
    print("Dropdown choice:", choice)
end)
```

---

### 🏷️ Text Label
```lua
Astra.CreateTextLabel(Section1, "Thank you for using Astra UI Library.")
```

---

### ➖ Divider
```lua
Astra.CreateDivider(Section1)
```

---

### 📑 Paragraph
```lua
Astra.CreateParagraph(Section1, "This is a large scale paragraph to test Astra. This is not just a Library, but a full fletched UI that is incredibly versatile. PLEASE join our Discord.")
```

---

### 🔔 Notification
```lua
Astra.CreateNotification("Demonstration Notification.", "This is a demonstration for our notification system.", 5)
```

---

## 🌗 Themes

Available themes:
- `Dark`  
- `Light`  
- `Ocean`  
- `Forest`  
- `Crimson`  

---

## 🛠️ Full Example

```lua
local MainUI = Astra.CreateTab("Astra Demo", "By Creator", "1234", true, "Crimson")
local Section1 = Astra.CreateSection("General")
local Section2 = Astra.CreateSection("Settings")

Shadow(MainUI)

Astra.CreateButton(Section1, "Click Me", function()
    print("Button clicked!")
end)

Astra.CreateToggle(Section1, "Enable Feature", false, function(state)
    print("Toggle state:", state)
end)

Astra.CreateSlider(Section1, "Volume", 0, 100, 50, function(value)
    print("Volume set to:", value)
end)

Astra.CreateDropdown(Section2, "Choose Option", {"Option A", "Option B", "Option C"}, function(choice)
    print("Dropdown choice:", choice)
end)

Astra.CreateTextLabel(Section1, "Thank you for using Astra UI Library.")
Astra.CreateDivider(Section1)
Astra.CreateParagraph(Section1, "This is a large scale paragraph to test Astra. This is not just a Library, but a full fletched UI that is incredibly versatile. PLEASE join our Discord.")

Astra.CreateNotification("Demonstration Notification.", "This is a demonstration for our notification system.", 5)
```

---

## 📌 Notes

- Replace the password string if using password protection.  
- All examples above are copy-paste ready.  

---

## 📜 License
MIT License — free to use, modify, and distribute. Attribution is appreciated but not required.  

MIT License — free to use, modify, and distribute. Attribution is appreciated but not required.  
