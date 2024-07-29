# orlibrary
```
local MyUILib = require(game:GetService("ReplicatedStorage"):WaitForChild("MyUILib"))

local window = MyUILib:CreateWindow("My UI")
local tab1 = MyUILib:CreateTab(window, "Tab 1")
local tab2 = MyUILib:CreateTab(window, "Tab 2")

MyUILib:CreateButton(tab1, "Click Me", function()
    print("Button clicked!")
end)

MyUILib:CreateDropdown(tab1, "Select Option", {"Option 1", "Option 2", "Option 3"}, function(selected)
    print("Selected:", selected)
end)

MyUILib:CreateToggle(tab1, "Enable Feature", function(toggled)
    print("Toggled:", toggled)
end)
```

```
local MyUILib = loadstring(game:HttpGet("https://raw.githubusercontent.com/Eradate/orlibrary/main/Orlibrary"))()

local window = MyUILib:CreateWindow("My UI")
local tab1 = MyUILib:CreateTab(window, "Tab 1")
local tab2 = MyUILib:CreateTab(window, "Tab 2")

MyUILib:CreateButton(tab1, "Click Me", function()
    print("Button clicked!")
end)

MyUILib:CreateDropdown(tab1, "Select Option", {"Option 1", "Option 2", "Option 3"}, function(selected)
    print("Selected:", selected)
end)

MyUILib:CreateToggle(tab1, "Enable Feature", function(toggled)
    print("Toggled:", toggled)
end)

MyUILib:CreateLabel(tab1, "This is a label")
MyUILib:CreateParagraph(tab1, "This is a paragraph of text that can span multiple lines.")

MyUILib:CreateButton(tab2, "Another Button", function()
    print("Another button clicked!")
end)

MyUILib:CreateLabel(tab2, "This is another label")
