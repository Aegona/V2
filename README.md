-----------------------------------------------------------------------------------------
-- script ผมทำเอง ขอบคุณที่พี่ สนับสนุนผม Script by AegonaChannel
-----------------------------------------------------------------------------------------


-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local BG1 = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local BG2 = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local Rady = Instance.new("TextLabel")
local Loadscript = Instance.new("TextLabel")
local loadbg = Instance.new("Frame")
local UICorner_3 = Instance.new("UICorner")
local loading = Instance.new("Frame")
local UICorner_4 = Instance.new("UICorner")
local ImageLabel = Instance.new("ImageLabel")
local TextLabel = Instance.new("TextLabel")
local TextButton = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

BG1.Name = "BG1"
BG1.Parent = ScreenGui
BG1.BackgroundColor3 = Color3.fromRGB(231, 231, 231)
BG1.Position = UDim2.new(0.5, -248, 0.5, -57)
BG1.Size = UDim2.new(0, 496, 0, 115)

UICorner.Parent = BG1

BG2.Name = "BG2"
BG2.Parent = BG1
BG2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BG2.BorderSizePixel = 0
BG2.Position = UDim2.new(0.233870968, 0, 0, 0)
BG2.Size = UDim2.new(0, 264, 0, 45)

UICorner_2.Parent = BG2

Rady.Name = "Rady"
Rady.Parent = BG2
Rady.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Rady.BackgroundTransparency = 1.000
Rady.BorderSizePixel = 0
Rady.Position = UDim2.new(0.112536669, 0, 0.144927531, 0)
Rady.Size = UDim2.new(0, 203, 0, 38)
Rady.Visible = false
Rady.Font = Enum.Font.SpecialElite
Rady.Text = "READY !!"
Rady.TextColor3 = Color3.fromRGB(0, 0, 0)
Rady.TextSize = 31.000
Rady.TextWrapped = true

Loadscript.Name = "Loadscript"
Loadscript.Parent = BG2
Loadscript.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Loadscript.BackgroundTransparency = 1.000
Loadscript.BorderSizePixel = 0
Loadscript.Position = UDim2.new(0.112536669, 0, 0.0560386479, 0)
Loadscript.Size = UDim2.new(0, 203, 0, 38)
Loadscript.Font = Enum.Font.Oswald
Loadscript.Text = "🔰  ∞ Load Script  ∞ 🔰"
Loadscript.TextColor3 = Color3.fromRGB(0, 0, 0)
Loadscript.TextScaled = true
Loadscript.TextSize = 14.000
Loadscript.TextWrapped = true

loadbg.Name = "loadbg"
loadbg.Parent = BG1
loadbg.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
loadbg.BorderSizePixel = 0
loadbg.Position = UDim2.new(0.0766129047, 0, 0.686956525, 0)
loadbg.Size = UDim2.new(0, 433, 0, 22)

UICorner_3.Parent = loadbg

loading.Name = "loading"
loading.Parent = loadbg
loading.BackgroundColor3 = Color3.fromRGB(0, 114, 236)
loading.BorderSizePixel = 0
loading.Position = UDim2.new(-0.00190900487, 0, 0, 0)
loading.Size = UDim2.new(0, 0, 0, 21)

UICorner_4.Parent = loading

ImageLabel.Parent = ScreenGui
ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ImageLabel.Position = UDim2.new(-0.241845667, 0, -0.417163283, 0)
ImageLabel.Size = UDim2.new(0, 1941, 0, 1448)
ImageLabel.Visible = false
ImageLabel.Image = "http://www.roblox.com/asset/?id=10076753898"

TextLabel.Parent = ImageLabel
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.LayoutOrder = 1
TextLabel.Position = UDim2.new(0.158122405, 0, 0.550093353, 0)
TextLabel.Size = UDim2.new(0, 530, 0, 219)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "เซ้กกับอ้ายบ๋ "
TextLabel.TextColor3 = Color3.fromRGB(19, 203, 87)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

TextButton.Parent = ImageLabel
TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton.BackgroundTransparency = 0.500
TextButton.Position = UDim2.new(0.591552436, 0, 0.627377212, 0)
TextButton.Size = UDim2.new(0, 369, 0, 129)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "ยอมโดนเซ้ก เพื่อเล่น"
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextScaled = true
TextButton.TextSize = 14.000
TextButton.TextWrapped = true

-- Scripts:

local function EBUQL_fake_script() -- loading.LocalScript 
	local script = Instance.new('LocalScript', loading)

	
	wait(2)
	script.Parent:TweenSize(UDim2.new(0, 120,0, 21),"Out", "Sine", 1)
	wait(1)
	script.Parent:TweenSize(UDim2.new(0, 190,0, 21),"Out", "Sine", 1)
	wait(1)
	script.Parent:TweenSize(UDim2.new(0, 299,0, 21),"Out", "Sine", 1)
	wait(1)
	script.Parent:TweenSize(UDim2.new(0, 350,0, 21),"Out", "Sine", 1)
	
	wait(1)
	script.Parent:TweenSize(UDim2.new(0, 435,0, 21),"Out", "Sine", 1)
	wait(1)
	script.Parent.Parent.Parent.BG2.Loadscript.Visible = false
	wait(.1)
	script.Parent.Parent.Parent.BG2.Rady.Visible = true
	wait(.6)
	script.Parent.Parent.Parent.Parent.BG1:TweenPosition(UDim2.new(1,0,0.2,0),"Out", "Sine", 1)
	wait(1)
	script.Parent.Parent.Parent.Parent.BG1.Visible = false
	wait(.1)
	script.Parent.Parent.Parent.Parent.ImageLabel.Visible = true
end
coroutine.wrap(EBUQL_fake_script)()
local function UVLQOBD_fake_script() -- TextButton.LocalScript 
	local script = Instance.new('LocalScript', TextButton)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Parent.ImageLabel.Visible = false
	end)
end
coroutine.wrap(UVLQOBD_fake_script)()


wait(14)


local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()

local win = DiscordLib:Window("z Aegona Hub z")

local serv = win:Server("⛏️Script⛏️ V.Beta", " Test")

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

tp:Button("TP อิหยิป ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(470.537598, 71.0699539, -3749.54199, 1, 0, 0, 0, 1, 0, 0, 0, 1)
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





spawn(function()
    while wait() do
        if _G.Farm then

wait(.1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(54.55238342285156, 82.46776580810547, 746.6566162109375) -- onepiece
wait(.1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42591094970703, 890.6080322265625) -- Demon
wait(.1)

game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42616271972656, 492.1081848144531)
wait(.1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42616271972656, 296.1081848144531)
wait(.1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(470.537598, 71.0699539, -3749.54199, 1, 0, 0, 0, 1, 0, 0, 0, 1)




wait(1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BossFightHitboxes.HitBox.CFrame * CFrame.new(0,0,10)
wait(30)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(54.55238342285156, 82.46776580810547, 746.6566162109375) -- onepiece
wait(1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42591094970703, 890.6080322265625) -- Demon
wait(1)

game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42616271972656, 492.1081848144531)
wait(1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123.56641387939453, 73.42616271972656, 296.1081848144531)
wait(1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(470.537598, 71.0699539, -3749.54199, 1, 0, 0, 0, 1, 0, 0, 0, 1)
wait(.1)
end
end
end)


egg:Toggle("EGG Demon", nil, function(value)
_G.EggDemon = value
end)
