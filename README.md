# ⭐ Starshot UI Library

Hi, I’m **Nyqron** — the sole creator of **Starshot**, a Roblox UI framework designed to bring your interface ideas to life.  

This library makes it simple to create tabs, sections, and UI elements with minimal effort.  

---

## 🚀 Load the Library

```lua
local UI = loadstring(http:get("https://pastebin.com/raw/kbfatKNg"))()
```
OR

Download the model:
https://create.roblox.com/store/asset/121795445220155/Starshot-UI-Library?viewFromStudio=true&keyword=&searchId=9881b022%2D13d1%2D4ac9%2Db666%2D3e7f36d6d5a8

---

## 📖 Creating a Tab

```lua
local MainUI = Starshot.CreateTab("Starshot Demo", "By Creator", "1234", true, "Crimson")
```

**Parameters:**
1. `Starshot Demo` → The **title** of your UI  
2. `By Creator` → The **subtitle** (optional credit/description)  
3. `1234` → The **password** string  
4. `true` → Whether a **password is required** (`true` = required, `false` = no password)  
5. `Crimson` → The **theme**  

---

## 📂 Creating a Section

```lua
local Section1 = Starshot.CreateSection("General")
local Section2 = Starshot.CreateSection("Settings")
```

---

## 🎨 UI Elements

### 🔘 Button
```lua
Starshot.CreateButton(Section1, "Click Me", function()
    print("Button clicked!")
end)
```

---

### ✅ Toggle
```lua
Starshot.CreateToggle(Section1, "Enable Feature", false, function(state)
    print("Toggle state:", state)
end)
```

---

### 🎚️ Slider
```lua
Starshot.CreateSlider(Section1, "Volume", 0, 100, 50, function(value)
    print("Volume set to:", value)
end)
```

---

### ⬇️ Dropdown
```lua
Starshot.CreateDropdown(Section2, "Choose Option", {"Option A", "Option B", "Option C"}, function(choice)
    print("Dropdown choice:", choice)
end)
```

---

### 🏷️ Text Label
```lua
Starshot.CreateTextLabel(Section1, "Thank you for using Astra UI Library.")
```

---

### ➖ Divider
```lua
Starshot.CreateDivider(Section1)
```

---

### 📑 Paragraph
```lua
Starshot.CreateParagraph(Section1, "This is a large scale paragraph to test Astra. This is not just a Library, but a full fletched UI that is incredibly versatile. PLEASE join our Discord.")
```

---

### 🔔 Notification
```lua
Starshot.CreateNotification("Demonstration Notification.", "This is a demonstration for our notification system.", 5)
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
local MainUI = Starshot.CreateTab("Astra Demo", "By Creator", "1234", true, "Crimson")
local Section1 = Starshot.CreateSection("General")
local Section2 = Starshot.CreateSection("Settings")

Starshot.CreateButton(Section1, "Click Me", function()
    print("Button clicked!")
end)

Starshot.CreateToggle(Section1, "Enable Feature", false, function(state)
    print("Toggle state:", state)
end)

Starshot.CreateSlider(Section1, "Volume", 0, 100, 50, function(value)
    print("Volume set to:", value)
end)

Starshot.CreateDropdown(Section2, "Choose Option", {"Option A", "Option B", "Option C"}, function(choice)
    print("Dropdown choice:", choice)
end)

Starshot.CreateTextLabel(Section1, "Thank you for using Astra UI Library.")
Starshot.CreateDivider(Section1)
Starshot.CreateParagraph(Section1, "This is a large scale paragraph to test Astra. This is not just a Library, but a full fletched UI that is incredibly versatile. PLEASE join our Discord.")

Starshot.CreateNotification("Demonstration Notification.", "This is a demonstration for our notification system.", 5)
```

## ❓ Support Server
https://discord.gg/kZKJFRxB

---

## 📌 Notes

- Replace the password string if using password protection.  
- All examples above are copy-paste ready.  

---

## 📜 License
MIT License — free to use, modify, and distribute. Attribution is appreciated but not required.  

