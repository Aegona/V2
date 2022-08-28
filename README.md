-----------------------------------------------------------------------------------------
-- script ผมทำเอง ขอบคุณที่พี่ สนับสนุนผม Script by AegonaChannel
-----------------------------------------------------------------------------------------


-- Gui to Lua
-- Version: 3.2

-- Instances:

local Aegona = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local ImageLabel = Instance.new("ImageLabel")
local TextLabel = Instance.new("TextLabel")

--Properties:

Aegona.Name = "Aegona"
Aegona.Parent = game.CoreGui
Aegona.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Frame.Parent = Aegona
Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame.Size = UDim2.new(0, 1257, 0, 839)

ImageLabel.Parent = Frame
ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ImageLabel.Position = UDim2.new(0.0310262535, 0, 0, 0)
ImageLabel.Size = UDim2.new(0, 1199, 0, 839)
ImageLabel.Image = "http://www.roblox.com/asset/?id=6403436054"

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 0.550
TextLabel.BorderSizePixel = 15
TextLabel.Position = UDim2.new(0.119331747, 0, 0.655542314, 0)
TextLabel.Size = UDim2.new(0, 911, 0, 251)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "เดียวผม กลับมา "
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

wait(2)
game:GetService("CoreGui").Aegona:Destroy()

local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()

local win = DiscordLib:Window("z Aegona Hub z")

local serv = win:Server("⛏️Script⛏️ V.Beta", " Test")

local btns = serv:Channel("Auto - Farm")
local tp = serv:Channel("TP")
local egg = serv:Channel("EGG")

btns:Toggle("Farm Box -- (ถ้าไม่วาปแปลว่ากล่องไม่เกิด)", nil, function(value)
_G.Farm = value
end)

btns:Toggle("TP Part ไป กล่องอื่น อัตโนมัติ", nil, function(value)
    while value do wait()
Instance.new("ForceField",game:GetService("Workspace").BossFightHitboxes.HitBox)

end
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

tp:Button("TP อิหยิป ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(470.537598, 71.0699539, -3749.54199, 1, 0, 0, 0, 1, 0, 0, 0, 1)
end)

egg:Toggle("EGG Demon", nil, function(value)
_G.EggDemon = value
end)



spawn(function()
            while wait() do 
                if _G.TP then
                    pcall(function()
Instance.new("ForceField",game:GetService("Workspace").BossFightHitboxes.HitBox)
end)
end
end
end)


btns:Toggle("Clicks", nil, function(value)
while value do wait()
    game:GetService("ReplicatedStorage").Remotes.DamageBoss:FireServer()
wait(.1)
game:GetService("ReplicatedStorage").Remotes.Click:InvokeServer()
wait(.1)
end
end)

btns:Toggle("รีเบิรด์", nil, function(value)
_G.Reb = value
end)


spawn(function()
    while wait() do
        if _G.Reb then
                    game:GetService("ReplicatedStorage").Remotes.Rebirth:FireServer()
end
end
end)

spawn(function()
    while wait() do
        if _G.Farm then
for i,v in pairs(game:GetService("Workspace").BossFightHitboxes:GetDescendants()) do
   if v.Name == "ForceField" then 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Parent.CFrame
wait(1)
_G.TP = true

wait(1)
end
end
end
end
end)


spawn(function()
    while wait() do
        if _G.EggDemon then
local args = {
    [1] = "Demon Egg",
    [2] = 4
}

game:GetService("ReplicatedStorage").Remotes.buyEgg:InvokeServer(unpack(args))
wait(.1)
end
end
end)
