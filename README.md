# IDK UI Library

## Getting Loadstring
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Mapple7777/UI-Librarys/main/UI-1/UI.lua"))()
```
## Create Window
```lua
local Window = Library:Create("Hub Name","Game Name")
```

## Create Tab
```lua
local Tab1 = Window:Tab("Tab 1",true)
```

## Create Label
```lua
Tab1:Label("Label")
```

## Create Button
```lua
Tab1:Button("Button",function()
    print("pressed btn")
end)
```

## Create Textbox
```lua
Tab1:Textbox("Textbox","Enter Text",function(txt)
    print(txt)
end)
```

## Create Keybind
```lua
Tab1:Keybind("Keybind",Enum.KeyCode.F,function()
    print("Pressed key")
end)
```

## Create DropDown
```lua
Tab1:Dropdown("Dropdown",{"Option 1","Option 2","Option 3"},function(current)
    print(current)
end)
```

## Create Toggle
```lua
Tab1:Toggle("Toggle",function(x)
    print(x)
end)
```

## Create Slider
```lua
Tab1:Slider("Slider",16,500,function(s)
    print(s)
end)
```

# Example

## Example
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Mapple7777/UI-Librarys/main/UI-1/UI.lua"))()

local Window = Library:Create("Hub Name","Game Name")

local Tab1 = Window:Tab("Tab 1",true)

Tab1:Label("Label")

Tab1:Button("Button",function()
    print("pressed btn")
end)

Tab1:Textbox("Textbox","Enter Text",function(txt)
    print(txt)
end)

Tab1:Keybind("Keybind",Enum.KeyCode.F,function()
    print("Pressed key")
end)

Tab1:Dropdown("Dropdown",{"Option 1","Option 2","Option 3"},function(current)
    print(current)
end)

Tab1:Toggle("Toggle",function(x)
    print(x)
end)

Tab1:Slider("Slider",16,500,function(s)
    print(s)
end)

local Tab2 = Window:Tab("Tab 2",false)

Tab2:Label("UI")

Tab2:Keybind("Toggle",Enum.KeyCode.RightShift,function()
    Library:Toggle()
end)
```
