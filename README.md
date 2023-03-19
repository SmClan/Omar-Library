# تثبيت المكتبه في السكربت :
```lua
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
```
# طريقة عمل نافذه

```lua
local Window = OrionLib:MakeWindow({Name = "اسم نافذة السكربت", HidePremium = false, SaveConfig = true, ConfigFolder = "OMAR"})
```


# طريقة عمل صفحه
```lua
local Tab = Window:MakeTab({
	Name = "اسم الصفحه",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
```

# طريقة عمل قسم
```lua
local Section = Tab:AddSection({
	Name = "Section"
})
```

# اضافة اشعار
```lua
OrionLib:MakeNotification({
	Name = "Title!",
	Content = "Notification content... what will it say??",
	Image = "rbxassetid://4483345998",
	Time = 5
})
```

# عمل زر

```lua
Tab:AddButton({
	Name = "Button!",
	Callback = function()
      		print("button pressed")
  	end    
})
```

# اضافة switch
```lua
Tab:AddToggle({
	Name = "This is a toggle!",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})
```

# عمل مغير الوان
```lua
Tab:AddColorpicker({
	Name = "Colorpicker",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})
```

# عمل شريط
```lua
Tab:AddSlider({
	Name = "Slider",
	Min = 0,
	Max = 20,
	Default = 5,
	Color = Color3.fromRGB(255,255,255),
	Increment = 1,
	ValueName = "bananas",
	Callback = function(Value)
		print(Value)
	end    
})
```

# اضافة نص
```lua
Tab:AddLabel("Label")
```
