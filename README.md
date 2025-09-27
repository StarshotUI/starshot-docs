# ⭐ Starshot UI Library

Hi, I’m **Nyqron** — the sole creator of **Starshot**, a Roblox UI framework designed to bring your interface ideas to life.  

This library makes it simple to create tabs, themes, and UI structures with minimal effort.

---

## 🚀 Getting Started

Load Starshot into your game:

```lua
local UI = loadstring(http:get("https://pastebin.com/raw/Ba2U3X7c"))()
```

# 📂 Basic Example
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
```
Astra.CreateNotification("Demonstration Notification.", "This is a demonstration for our notification system.", 5)

```
