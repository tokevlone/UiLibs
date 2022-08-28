# Vast Ui Library
How to use the vast ui library [OpenSource] [Not for skids]

## Config
```lua
local Config = {
    WindowName = "Name",
	Color = Color3.fromRGB(83, 0, 156),
	Keybind = Enum.KeyCode.RightBracket
}
```

## Booting The Library
``` lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/tokevlone/Vast/main/Library"))()
local Window = Library:CreateWindow(Config, game:GetService("CoreGui"))
```

## Creating Tabs
```lua
local Tab1 = Window:CreateTab("Name")
```

## Creating Sections
```lua
 Section1 = Tab1:CreateSection("Name")
```

## Creating Labels
```lua
local Label1 = Section1:CreateLabel("Name")
```

## Creating Buttons
```lua
local Button1 = Section1:CreateButton("Name", function()
	[action/script]
end)
```

## Creating Toggles
```lua
-- Creating Toggles
local Toggle1 = Section1:CreateToggle("Name", nil, function(State)
	[action/script]
end)
```

## Creating Textboxes
```lua
local TextBox1 = Section1:CreateTextBox("Name", "Descreption", true, function(Value)
	[action/script]
end)
```

## Creating Sliders
```lua
local Slider1 = Section1:CreateSlider("Name", 0,100,nil,true, function(Value)
	[action/script]
end)
```

## Creating Dropdowns
```lua
local Dropdown1 = Section1:CreateDropdown("Name", {"Option1","Option2","Option3"}, function(String)
	[action/script]
end)
```

## Creating Colorpickers
```lua
local Colorpicker1 = Section1:CreateColorpicker("Name", function(Color)
	[action/script]
end)
```


## Creating Ui Toggle
```lua
local Toggle1 = Section1:CreateToggle("Name", nil, function(State)
	Window:Toggle(State)
end)
Toggle3:CreateKeybind(tostring(Config.Keybind):gsub("Enum.KeyCode.", ""), function(Key)
	Config.Keybind = Enum.KeyCode[Key]
end)
```

## Creating Ui Color Changer
```lua
local Colorpicker1 = Section1:CreateColorpicker("Name", function(Color)
	Window:ChangeColor(Color)
end)
Colorpicker1:UpdateColor(Config.Color)
```
