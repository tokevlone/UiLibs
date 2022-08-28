# Vast
How to use the vast ui library

## Config
```lua
local Config = {
    WindowName = "Name",
	Color = Color3.fromRGB(83, 0, 156),
	Keybind = Enum.KeyCode.RightBracket
}

-- Replace "Name" with name of exploit/hub window
```

## Booting The Library
``` lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/tokevlone/Vast/main/Library"))()
local Window = Library:CreateWindow(Config, game:GetService("CoreGui"))
```

## Creating Tabs
```lua
local Tab1 = Window:CreateTab("Name")

-- Replace "Name" With ur choice
-- If u want multiple tabs, name the other ones "Tab2", "Tab3" and so on...
```

## Creating Sections
```lua
-- Creating Sections
local Section1 = Tab1:CreateSection("Name")
-- if you want many sections, make the other ones "Section2", "Section3" and so on..
-- Replace "Tab1" with the tab you want this section in
```

## Creating Labels
```lua
local Label1 = Section1:CreateLabel("Name")
-- If you wanna make many Labels, make the other ones "Label2", "Label3" and so on...
-- Replace "Section1" with the section you want the label to be in
-- Replace "Name" with the name of your label
```

## Creating Buttons
```lua
local Button1 = Section1:CreateButton("Name", function()
	[action/script]
end)
-- If you wanna make many Buttons, make the other ones "Button2", "Button3" and so on...
-- Replace "Section1" with the section you want the button to be in
-- Replace "Name" with the name of your button name
```

 Creating Toggles
```lua
-- Creating Toggles
local Toggle1 = Section1:CreateToggle("Name", nil, function(State)
	[action/script]
end)
-- If you wanna make many Toggles, make the other ones "Toggle2", "Toggle3" and so on...
-- Replace "Section1" with the section you want the toggle to be in
-- Replace "Name" with the name of your toggle name
```

Creating Textboxes
```lua
local TextBox1 = Section1:CreateTextBox("Name", "Descreption", true, function(Value)
	[action/script]
end)
-- If you wanna make many TextBoxes, make the other ones "TextBox2", "TextBox3" and so on...
-- Replace "Section1" with the section you want the textbox to be in
-- Replace "Name" with the name of your textbox name
-- Replace "Descreption" with what you want the textbox to say
```

Creating Sliders
```lua
local Slider1 = Section1:CreateSlider("Name", 0,100,nil,true, function(Value)
	[action/script]
end)
-- If you wanna make many Slider, make the other ones "Slider2", "Slider3" and so on...
-- Replace "Section1" with the section you want the slider to be in
-- Replace "Name" with the name of your slider name
```

Creating Dropdowns
```lua
local Dropdown1 = Section1:CreateDropdown("Name", {"Option1","Option2","Option3"}, function(String)
	[action/script]
end)
-- If you wanna make many Dropdowns, make the other ones "Dropdown2", "Dropdown3" and so on...
-- Replace "Section1" with the section you want the dropdown to be in
-- Replace "Name" with the name of your dropdown name
-- replace the Options with name of the option in dropdown
```

Creating Colorpickers
```lua
local Colorpicker1 = Section1:CreateColorpicker("Name", function(Color)
	[action/script]
end)
-- If you wanna make many ColorPickers, make the other ones "ColorPicker2", "ColorPicker3" and so on...
-- Replace "Section1" with the section you want the colorpicker to be in
-- Replace "Name" with the name of your colorpicker name
```
