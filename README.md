local Hint = Instance.new("Hint", game.CoreGui)
Hint.Text = "++Menu | Loading..."
wait(1.3)
local library = loadstring(game:HttpGet("https://pastebin.com/raw/RvJ0qewm", true))()
local main = library:CreateWindow("Hung hub")
local Playset = main:Section("prees v for auto clicker")

local button1 = main:Button("Suicide", function()
game.Players.LocalPlayer.Character.Humanoid.Health = 0
end)

local speed = main:Slider("Speed", {
min=0;
max=80;
flag="Get:Speed%f"}, function(sp)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = sp
end)

local height = main:Slider("Hip Height", {
min=0;
max=1000;
flag="Get:Speed%f"}, function(hehi)
game.Players.LocalPlayer.Character.Humanoid.HipHeight = hehi
end)

local Megajum = main:Button("Mega Jump", function()
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 200
end)

click = false
m = game.Players.LocalPlayer:GetMouse()
m.KeyDown:connect(function(key)
if key == "v" then
if click == true then click = false
elseif
click == false then click = true

while click == true do 
wait(time)
mouse1click()
end
end
end
end)
Hint.Text = "++Menu | Loaded!"
wait(1.5)
Hint:Destroy()
