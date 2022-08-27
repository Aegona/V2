
_G.TP = true



local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()

local win = DiscordLib:Window("discord library")

local serv = win:Server("z Aegona Hub z Script V.Beta", " Test")

local btns = serv:Channel("Auto - Farm")
local tp = serv:Channel("TP")
local egg = serv:Channel("EGG")

btns:Toggle("Farm Box -- (ถ้าไม่วาปแปลว่ากล่องไม่เกิด)", nil, function(value)
_G.Farm = value
end)

btns:Button(" วาป ออก จาก กล่อง ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(54.55238342285156, 82.46776580810547, 746.6566162109375)
end)



tp:Button("TP Demon ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42591094970703, 890.6080322265625)
end)

tp:Button("TP OnePiece ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42621612548828, 703.608154296875)
end)

tp:Button("TP Ninja ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42616271972656, 492.1081848144531)
end)

tp:Button("TP DargonCitys ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42616271972656, 296.1081848144531)
end)

spawn(function()
            while wait() do 
                if _G.Farm then
                    pcall(function()
for i,v in pairs(game:GetService("Workspace").BossFightHitboxes:GetDescendants()) do
   if v.Name == "ForceField" then 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Parent.CFrame
wait(30)
end
end
end)
end
end
end)

egg:Toggle("EGG Demon", nil, function(value)
_G.eggdemon = value
end)


spawn(function()
            while wait() do 
                if _G.eggdemon then
                    while _G.eggdemon do wait()  

local args = {
    [1] = "Demon Egg",
    [2] = 4
}

game:GetService("ReplicatedStorage").Remotes.buyEgg:InvokeServer(unpack(args))
wait(.1)
game:GetService("ReplicatedStorage").Remotes.UpdatePetValues:FireServer()

end
end
end
end)

spawn(function()
            while wait(2) do 
                if _G.TP then
        Instance.new("ForceField",game:GetService("Workspace").BossFightHitboxes.HitBox)
end
end
end)

btns:Button("กลับไปในกล่อง ", function()
for i,v in pairs(game:GetService("Workspace").BossFightHitboxes:GetDescendants()) do
   if v.Name == "ForceField" then 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Parent.CFrame
end
end
end)
