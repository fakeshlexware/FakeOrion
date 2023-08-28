# Fake Orion Library
This documentation is for the Fake Orion Library.


## Booting the Library
```lua
local FakeOrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/fakeshlexware/FakeOrion/main/source')))()
```


## Creating a Window
```lua
local Window = FakeOrionLib:MakeWindow({Name = "Fake Orion!"})

--[[
Name = <string> - The name of the UI.
]]
```


## Creating a Tab
```lua
local Tab = Window:MakeTab({
	Name = "Tab",
	Icon = "rbxassetid://14595162359"
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
]]
```


## Creating a Section
```lua
local Section = Tab:AddSection({
	Name = "Section!"
})

--[[
Name = <string> - The name of the section.
]]
```


## Creating a Button
```lua
Tab:AddButton({
    Name = "Button!",
    Callback = function()
        
    end
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
```


## Creating a Checkbox toggle
```lua
Tab:AddToggle({
	Name = "Toggle!",
	Default = false,
	Callback = function(state)
		
	end    
})

--[[
Name = <string> - The name of the toggle.
Default = <bool> - The default value of the toggle.
Callback = <function> - The function of the toggle.
]]
```


## Creating a Slider
```lua
Tab:AddSlider({
    Name = "Slider!",
    Max = 100,
    ValueName = "Value!",
    Callback = function(value)
        
    end
})

--[[
Name = <string> - The name of the slider.
Max = <number> - The maxium value of the slider.
ValueName = <string> - The text after the value number.
Callback = <function> - The function of the slider.
]]
```


## Creating a Label
```lua
Tab:AddLabel({
	Name = "Label!"
})

--[[
Name = <string> - The name of the textbox.
]]
```


## Creating an Adaptive Input
```lua
Tab:AddTextbox({
	Name = "Box!",
	Default = "Enter!",
	Callback = function(input)
		
	end	  
})

--[[
Name = <string> - The name of the textbox.
Default = <string> - The default value of the textbox.
Callback = <function> - The function of the textbox.
]]
```
