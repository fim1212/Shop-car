local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("main GUi Jack Sn", "BloodTheme")
local Tab = Window:NewTab("Shop car")
local Section = Tab:NewSection("Shop Car all in")
Section:NewButton("LightUtility", "500 kg", function()
local args = {
    [1] = "Buy",
    [2] = "LightUtility"
}

game:GetService("ReplicatedStorage"):WaitForChild("Remote"):WaitForChild("Car"):FireServer(unpack(args))

end)

Section:NewButton("Pickup Truck", "150 kg", function()
    local PickupTruck = {
      [1] = "Buy",
      [2] = "Pickup Truck"
    }

    game:GetService("ReplicatedStorage"):WaitForChild("Remote"):WaitForChild("Car"):FireServer(unpack(PickupTruck))

end)

Section:NewButton("Sports Car", "speed car", function()
    local SportsCar = {
      [1] = "Buy",
      [2] = "Sports Car"
    }

    game:GetService("ReplicatedStorage"):WaitForChild("Remote"):WaitForChild("Car"):FireServer(unpack(SportsCar))

end)

Section:NewButton("Super car", "top speedcar", function()
    local Supercar = {
      [1] = "Buy",
      [2] = "Super Car"
    }

    game:GetService("ReplicatedStorage"):WaitForChild("Remote"):WaitForChild("Car"):FireServer(unpack(Supercar))

end)
