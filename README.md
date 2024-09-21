## Create Window
```lua
local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/rainhitgrassed/shadowlib/refs/heads/main/lib?token=GHSAT0AAAAAACXFZ6G62GRA4OUCNVSWV4EUZXOBV4Q"))()

local Window = redzlib:MakeWindow({
  Title = "Test",
  SubTitle = "hello",
  SaveFolder = "Redz Config"
})
```

## Create Tab
```lua
local tab1 = Window:MakeTab({"Main", "cool"})
```

## Create Button
```lua
Tab1:AddButton({"Print", function()
  print("Hello World!")
end})
```

## Create Toggle
```lua
local Toggle1 = tab1:AddToggle({
  Name = "Speed",
  Description = "Idk",
  Default = false
})
```

## Create Slider
```lua
tab1:AddSlider({
  Name = "Speed",
  Min = 1,
  Max = 100,
  Increase = 1,
  Default = 16,
  Callback = function(Value)
  game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
  end
})
```
