# Vape Library
This documentation is for the stable release of Vape Library.

## Booting the Library
```lua
local lib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/Vape.txt")()
```



## Creating a Window
```lua
local win = lib:Window("PREVIEW",Color3.fromRGB(44, 120, 224), Enum.KeyCode.LeftAlt)
```



## Creating a Tab
```lua
local tab = win:Tab("Tab 1")
```


## Creating a Button
```lua
tab:Button("Button", function()
print("Vape Ontop")
end)
```


## Creating a Checkbox toggle
```lua
tab:Toggle("Toggle",false, function(t)
print(t)
end)
```
## Creating A Notification
```lua
lib:Notification("Notification", "Hello!", "Hi!")
```

## Creating a Color Picker
```lua
tab:Colorpicker("Colorpicker",Color3.fromRGB(255,0,0), function(t)
print(t)
end)
```

### Setting the color picker's value
```lua
ColorPicker:Set(Color3.fromRGB(255,255,255))
```


## Creating a Slider
```lua
tab:Slider("Slider",0,100,30, function(t)
print(t)
end)
```

## Creating a Label
```lua
tab:Label("Label")
```

## Creating a Keybind
```lua
tab:Bind("Bind",Enum.KeyCode.RightShift, function()
print("Pressed!")
end)
```

## Creating a Dropdown menu
```lua
tab:Dropdown("Dropdown",{"Option 1","Option 2","Option 3","Option 4","Option 5"}, function(t)
print(t)
end)
```


