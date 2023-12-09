-- Achievement
local Achievements = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors/Custom%20Achievements/Source.lua"))()

-- Creates and displays your custom achievement
Achievements.Get({
    Title = "ROMMS & DOORS MODE v2",
    Desc = "EXECUTE Yes No way",
    Reason = 'Test mode',
    Image = "11867753039/meme-hamster-xd",
})

loadstring(game:HttpGet("https://raw.githubusercontent.com/huyhoanphuc/autorooms/main/README.md", true))()

--[=[
@class txt
This is my First Class
--]=]

print(os.date("%B"))

print("Loading")
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------------------

local HardCore = {
    Title = "The Pain Just Begain", -- Made by MuhammadGames and Volta
    Desc = "Join a Match of HardCore For the First Time.",
    Reason = "You executed the HardCore script.",
    Image = "https://github.com/MuhXd/Models/blob/main/HardCoreDoors.png?raw=true",
    id = 1,
}

local DepthW = {
    Title = "Finally Free",
    Desc = "Encounter Depth",
    Reason = "Survive Depth",
    Image = "https://github.com/MuhXd/DoorSuff/blob/main/DoorsModes/Png.png?raw=true",
    id = 2,
}

local Depth = {
    Title = "The Entity Is Still Freezing",
    Desc = "It's So Cold",
    Reason = "Dont Survive Depth",
    Image = "https://github.com/MuhXd/DoorSuff/blob/main/DoorsModes/Png.png?raw=true",
    id = 3,
}

local Smiles = {
    Title = "Income The Frowners",
    Desc = "Stop Smiling",
    Reason = "Encounter and Survive Smiler",
    Image = "https://tr.rbxcdn.com/533cbe35b1cf3d4e5d4f99278978563f/150/150/Image/Png",
    id = 4,
}

local SmilesDie = {
    Title = "Smile to Fail",
    Desc = "Don't Smile",
    Reason = "Encounter And Dont Survive Smiler",
    Image = "https://tr.rbxcdn.com/533cbe35b1cf3d4e5d4f99278978563f/150/150/Image/Png",
    id = 5,
}

local NightmareRush ={
    Title = "Rush From Your Nightmares",
    Desc = "Don't Be fooled",
    Reason = "Encounter And Survive Nightmare Rush",
    Image = "https://tr.rbxcdn.com/533cbe35b1cf3d4e5d4f99278978563f/150/150/Image/Png",
    id = 6,
}

local NightmareAmbush ={
    Title = "Ambush But Even Harder",
    Desc = "Don't Be fooled",
    Reason = "Encounter And Survive Nightmare Ambush",
    Image = "https://tr.rbxcdn.com/533cbe35b1cf3d4e5d4f99278978563f/150/150/Image/Png",
    id = 7,
}

local NightmareAmbush ={
    Title = "Ambush But Even Harder",
    Desc = "Don't Be fooled",
    Reason = "Encounter And Survive Nightmare Ambush",
    Image = "https://tr.rbxcdn.com/533cbe35b1cf3d4e5d4f99278978563f/150/150/Image/Png",
    id = 8,
}


-----------------------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------------------






-- loadstring(game:HttpGet("https://raw.githubusercontent.com/MuhXd/DoorSuff/main/Whitelist/NewKeySystem.lua"))()



caa = 0
tween = game:GetService("TweenService")
local TestMultplayer = true
if game:GetService("ReplicatedStorage"):FindFirstChild("Extacuted") then
    warn("You have Already Loaded")

    return false
end
local Test = Instance.new("Part")
Test.Name = "Extacuted"
Test.Parent = game:GetService("ReplicatedStorage")
Test = 1

local SelfModules = {
    Functions = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Functions.lua"))(),
}






------------------------------------------------------------------------------------------------

------------------------------------------------------------------------------------------------







local ModName = "HardCore"
local foldername = "AchievementsSaves   By Muhammadgames,Helped by RegularVynixu"
local Slipt = string.split(foldername,"|")
local valid2 = isfolder(foldername)
if not valid2 then
    makefolder(foldername)
end

local fileName = ModName.."Save's.txt"
local filePath = foldername.. "/".. fileName
local valid = isfile(filePath)

local Achievements = loadstring(game:HttpGet("https://raw.githubusercontent.com/MuhXd/Models/main/RegularVynixu's%20Achievement%20Modifyer"))()

function AchievementsGet(Achievement)
    local read = readfile(filePath)  
    local read2 = tostring(read)
    local read2 = string.split(read,"|")
    FOUND = true
    Find = ""
    for i,v in pairs(Achievement) do
        if i == "id" then
            Find=Find.." "..v
        end
    end

    for i,v in pairs(read2) do
        if v == Find then
            FOUND = true
        end
    end -- Desc
    if FOUND == false then
        Achievements.Get(Achievement)
        Write = ""
        for i,v in pairs(Achievement) do
            if i == "id" then
                Write=Write.." "..v
            end
        end
        appendfile(filePath,Write.."|")
    end
end
-- Creates and displays your custom achievement
-- readfile(<string> path)  
if not valid then
    writefile(filePath, "Helped by RegularVynixu|")
end

AchievementsGet(HardCore)
--[[
------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------ 
Start of real Code!
DON'T SHOW ABOVE!
.............     .       .
.     .     .     .       . 
.     .     .     .       .
.     .     .     .       . 
.     .     .     .       . 
.     .     .     .       . 
.     .     .     .       .
.     .     .     .........
--]]












if game:GetService("ReplicatedStorage"):FindFirstChild("Guis") then

else
    Visable = Instance.new("Folder")
    Visable.Name = "Guis"
    Visable.Parent = game.ReplicatedStorage

end
function Gui(Name,Amount1,TextSent)
    if game:GetService("Players").localPlayer.PlayerGui.MainUI.Statistics.Frame:FindFirstChild("!"..Name.."!") then
        game:GetService("Players").localPlayer.PlayerGui.MainUI.Statistics.Frame["!"..Name.."!"]:Destroy()
    end

    Visable = Instance.new("BoolValue")
    Visable.Value = true
    Visable.Name = Name
    Visable.Parent = game.ReplicatedStorage.Guis

    game.Players.localPlayer.PlayerGui.MainUI.Statistics.LocksOpened.Visible = true
    LocksOpened = game.Players.localPlayer.PlayerGui.MainUI.Statistics.LocksOpened:Clone()
    game.Players.localPlayer.PlayerGui.MainUI.Statistics.LocksOpened.Visible = false
    LocksOpened.Parent = game.Players.localPlayer.PlayerGui.MainUI.Statistics.Frame

    LocksOpened.Visible = game.ReplicatedStorage.Guis:FindFirstChild(Name).Value

    local Grad = game.Players.localPlayer.PlayerGui.MainUI.Statistics.Frame["Leftover Gold"].UICorner:Clone()
    Grad.Parent = LocksOpened
    Grad = game.Players.localPlayer.PlayerGui.MainUI.Statistics.Frame["Leftover Gold"].UIGradient:Clone()
    Grad.Parent = LocksOpened
    Grad = game.Players.localPlayer.PlayerGui.MainUI.Statistics.Frame["Leftover Gold"].Amount:Clone()
    Grad.Parent = LocksOpened
    Grad.Text = Amount1
    Grad.Position = Grad.Position - UDim2.new(0.035,0,0,0)
    Grad = game.Players.localPlayer.PlayerGui.MainUI.Statistics.Frame["Leftover Gold"].Icon:Clone()
    Grad.Parent = LocksOpened
    Grad.Position = Grad.Position - UDim2.new(0.035,0,0,0)

    LocksOpened.CloseButton.Position = LocksOpened.CloseButton.Position - UDim2.new(0.021,0,0,0)
    LocksOpened.CloseButton.ImageColor3 =  Color3.new(0.0313725, 0.854902, 1)
    LocksOpened.TextColor3 = Color3.new(0.0313725, 0.854902, 1)
    LocksOpened.TextScaled = false
    LocksOpened.Name = "!"..Name.."!"
    LocksOpened.TextSize = game.Players.localPlayer.PlayerGui.MainUI.Statistics.Frame["Leftover Gold"].TextSize + 16
    LocksOpened.Size = LocksOpened.Parent["Leftover Gold"].Size
    LocksOpened.BackgroundColor3 = Color3.new(0.0196078, 0.552941, 0.647059)
    LocksOpened.BackgroundTransparency = 0.5

    LocksOpened.Text = TextSent



    game.ReplicatedStorage.Guis:FindFirstChild(Name).changed:connect(function()

        LocksOpened.Visible = game.ReplicatedStorage.Guis:FindFirstChild(Name).Value
    end)
end







local Creator = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors%20Entity%20Spawner/Source.lua"))()


-- Run the created entity
local Message = function(Message,Enable,N)
    local msg = Instance.new("Message")  
    msg.Parent = game.Workspace     
    msg.Text = Message
    if Enable ~= true then
        task.wait(0.1)
        msg:Destroy()
    end
end

-- Message("Thank you For Loading MultplayerBeta 1.2")

for ii,vv in pairs(game:GetService("Players"):GetChildren()) do
    PlayersIngame = ii
end -- Gets All Players
if TestMultplayer == true then
    PlayersIngame = 10 -- TestMultplayer
end

if PlayersIngame > 1 then -- if more then one then waits for link
    if game:GetService("ReplicatedStorage").GameData.LatestRoom.Value > 0 then
        print("Loaded After door 1! Please wait for everyone to die")
        game.StarterGui:SetCore("ChatMakeSystemMessage", {
            Text = "Load Before Door 1",
            Color = Color3.fromRGB(255, 0, 0),
            Font = Enum.Font.SourceSansBold,
            TextSize = 18,
        })

        firesignal(game.ReplicatedStorage.Bricks.DeathHint.OnClientEvent, {"You didn't Load it Before Door 1!","Please Wait for the next round"})
        game.ReplicatedStorage.GameStats["Player_".. game.Players.LocalPlayer.Name].Total.DeathCause.Value = "Not Loading Before Door 1"
        game.Players.LocalPlayer.Character.Humanoid.Health = -100
        return false
    end


    game.StarterGui:SetCore("ChatMakeSystemMessage", {
        Text = "Doors Hard Mode ON! By MuhammadGames (MuhammadGames#0017) and Volta (volta#2161)",
        Color = Color3.fromRGB(255, 0, 0),
        Font = Enum.Font.SourceSansBold,
        TextSize = 18,
    })

    Gui("HardMode","+1000","Hard Mode (Doesn't add Nobs)")

    print("Loaded, Wating to Link to Multplayer") -- waiting to link

game:GetService("ReplicatedStorage").GameData.LatestRoom.Changed:Connect(function(v)
    L = game:GetService("Workspace").CurrentRooms[v].PathfindNodes:Clone()
    L.Parent = game:GetService("Workspace").CurrentRooms[v]
    L.Name = 'PathfindNodes'
end)
    
    c=1

    repeat task.wait()

        if c < 10 then
            -- Message("MultplayerV1.2B",true,"Welcome")
            c=10
        end
        --  msg:Destroy()
        --Kill=true
    until game:GetService("ReplicatedStorage").GameData.LatestRoom.Value > 0
    print("Linked to Clients") -- linked
    
    game.StarterGui:SetCore("ChatMakeSystemMessage", {
        Text = "Linked To Clients",
        Color = Color3.fromRGB(0, 255, 0),
        Font = Enum.Font.SourceSansBold,
        TextSize = 18,
    })



    Singleplayer = false -- Runs more Then 1 Player Code
else
    print("Loaded in print Multiplayer") -- loaded in 1 player
    repeat task.wait()

    until game:GetService("ReplicatedStorage").GameData.LatestRoom.Value > 0
    print("Started")
    Singleplayer = true -- Runs One player Code
end
Testa = 10
getgenv().death = false
Be=false
Many=1
JobId = game:GetService("ReplicatedStorage").GameData.GameStarted.Value
Lowest = string.len(game:GetService("ReplicatedStorage").GameData.GameStarted.Value)
Lowest = tonumber(Lowest)
Stop=Lowest
RanWait2=""
    function VhsSansSpawn()
        while true do wait(60)
            pcall(function()
                local Creator = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors%20Entity%20Spawner/Source.lua"))()

                -- Create entity
                local entity2 = Creator.createEntity({
                    CustomName = "A-60", -- Custom name of your entity
                    Model = "https://github.com/Johnny39871/assets/blob/main/A-60%20v2.rbxm?raw=true", -- Can be GitHub file or rbxassetid
                    Speed = 300, -- Percentage, 100 = default Rush speed
                    DelayTime = 2, -- Time before starting cycles (seconds)
                    HeightOffset = 4,
                    CanKill = true,
                    KillRange = 30,
                    BreakLights = false,
                    BackwardsMovement = false,
                    FlickerLights = {
                        true, -- Enabled/Disabled
                        0.1, -- Time (seconds)
                    },
                    Cycles = {
                        Min = 1,
                        Max = 1,
                        WaitTime = 0,
                    },
                    CamShake = {
                        true, -- Enabled/Disabled
                        {2.5, 20, 0.1, 1}, -- Shake values (don't change if you don't know)
                        100, -- Shake start distance (from Entity to you)
                    },
                    Jumpscare = {
                        true, -- Enabled/Disabled
                        {
                            Image1 = "rbxassetid://11826898817", -- Image1 url
                            Image2 = "rbxassetid://11867753039", -- Image2 url
                            Shake = true,
                            Sound1 = {
                                5263560566, -- SoundId
                                { Volume = 0.5 }, -- Sound properties
                            },
                            Sound2 = {
                                6459610652, -- SoundId
                                { Volume = 0.5 }, -- Sound properties
                            },
                            Flashing = {
                                true, -- Enabled/Disabled
                                Color3.fromRGB(255, 255, 255), -- Color
                            },
                            Tease = {
                                true, -- Enabled/Disabled
                                Min = 1,
                                Max = 1,
                            },
                        },
                    },
                    CustomDialog = {"You died to who you call A-60...", "Try your best to out-run him.", "I really don't have nothing else", "Just try your best to Hide when you can."}, -- Custom death message
                })

                ------------------------
                Creator.runEntity(entity2)
                -- Run the created entity
            end)
        end
    end
    
    function VhsSasSpawn()
        while true do wait(70)
            pcall(function()
                local Creator = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors%20Entity%20Spawner/Source.lua"))()

                -- Create entity
                local entity5 = Creator.createEntity({
                    CustomName = "Primes A-60", -- Custom name of your entity
                    Model = "https://github.com/Johnny39871/assets/blob/main/A-60%20refined.rbxm?raw=true", -- Can be GitHub file or rbxassetid
                    Speed = 300, -- Percentage, 100 = default Rush speed
                    DelayTime = 2, -- Time before starting cycles (seconds)
                    HeightOffset = 2,
                    CanKill = true,
                    KillRange = 30,
                    BreakLights = false,
                    BackwardsMovement = false,
                    FlickerLights = {
                        true, -- Enabled/Disabled
                        0.1, -- Time (seconds)
                    },
                    Cycles = {
                        Min = 1,
                        Max = 1,
                        WaitTime = 0,
                    },
                    CamShake = {
                        true, -- Enabled/Disabled
                        {2.5, 20, 0.1, 1}, -- Shake values (don't change if you don't know)
                        100, -- Shake start distance (from Entity to you)
                    },
                    Jumpscare = {
                        true, -- Enabled/Disabled
                        {
                            Image1 = "rbxassetid://11131703032", -- Image1 url
                            Image2 = "rbxassetid://3413871766", -- Image2 url
                            Shake = true,
                            Sound1 = {
                                3537873683, -- SoundId
                                { Volume = 2 }, -- Sound properties
                            },
                            Sound2 = {
                                6459610652, -- SoundId
                                { Volume = 0.5 }, -- Sound properties
                            },
                            Flashing = {
                                true, -- Enabled/Disabled
                                Color3.fromRGB(255,0,0), -- Color
                            },
                            Tease = {
                                true, -- Enabled/Disabled
                                Min = 1,
                                Max = 1,
                            },
                        },
                    },
                    CustomDialog = {"You died to who you call PrimesA-60...", "Try your best to out-run him.", "I really don't have nothing else", "Just try your best to Hide when you can."}, -- Custom death message
                })

                ------------------------
                Creator.runEntity(entity5)
                -- Run the created entity
            end)
        end
    end

    function VhsSaisSpawn()
        while true do wait(570)
            pcall(function()
                local Creator = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors%20Entity%20Spawner/Source.lua"))()

                -- Create entity
                local entity6 = Creator.createEntity({
                    CustomName = "Primes A-60", -- Custom name of your entity
                    Model = "https://github.com/Johnny39871/assets/blob/main/A-60%20refined.rbxm?raw=true", -- Can be GitHub file or rbxassetid
                    Speed = 300, -- Percentage, 100 = default Rush speed
                    DelayTime = 2, -- Time before starting cycles (seconds)
                    HeightOffset = 2,
                    CanKill = true,
                    KillRange = 30,
                    BreakLights = false,
                    BackwardsMovement = false,
                    FlickerLights = {
                        true, -- Enabled/Disabled
                        0.1, -- Time (seconds)
                    },
                    Cycles = {
                        Min = 1,
                        Max = 1,
                        WaitTime = 0,
                    },
                    CamShake = {
                        true, -- Enabled/Disabled
                        {300.5, 20, 0.1, 1}, -- Shake values (don't change if you don't know)
                        100, -- Shake start distance (from Entity to you)
                    },
                    Jumpscare = {
                        true, -- Enabled/Disabled
                        {
                            Image1 = "rbxassetid://11131703032", -- Image1 url
                            Image2 = "rbxassetid://3413871766", -- Image2 url
                            Shake = true,
                            Sound1 = {
                                3537873683, -- SoundId
                                { Volume = 2 }, -- Sound properties
                            },
                            Sound2 = {
                                6459610652, -- SoundId
                                { Volume = 0.5 }, -- Sound properties
                            },
                            Flashing = {
                                true, -- Enabled/Disabled
                                Color3.fromRGB(255,0,0), -- Color
                            },
                            Tease = {
                                true, -- Enabled/Disabled
                                Min = 1,
                                Max = 1,
                            },
                        },
                    },
                    CustomDialog = {"You died to who you call PrimesA-60...", "Try your best to out-run him.", "I really don't have nothing else", "Just try your best to Hide when you can."}, -- Custom death message
                })

                ------------------------
                Creator.runEntity(entity6)
                -- Run the created entity
            end)
        end
    end

    function VhsSiasSpawn()
        while true do wait(150)
            pcall(function()
                local Creator = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors%20Entity%20Spawner/Source.lua"))()

                -- Create entity
                local entity7 = Creator.createEntity({
                    CustomName = "Primes A-60", -- Custom name of your entity
                    Model = "https://github.com/Johnny39871/assets/blob/main/A-60%20refined.rbxm?raw=true", -- Can be GitHub file or rbxassetid
                    Speed = 300, -- Percentage, 100 = default Rush speed
                    DelayTime = 3, -- Time before starting cycles (seconds)
                    HeightOffset = 2,
                    CanKill = true,
                    KillRange = 30,
                    BreakLights = false,
                    BackwardsMovement = false,
                    FlickerLights = {
                        true, -- Enabled/Disabled
                        0.1, -- Time (seconds)
                    },
                    Cycles = {
                        Min = 1,
                        Max = 1,
                        WaitTime = 0,
                    },
                    CamShake = {
                        true, -- Enabled/Disabled
                        {400.5, 20, 0.1, 1}, -- Shake values (don't change if you don't know)
                        100, -- Shake start distance (from Entity to you)
                    },
                    Jumpscare = {
                        true, -- Enabled/Disabled
                        {
                            Image1 = "rbxassetid://11131703032", -- Image1 url
                            Image2 = "rbxassetid://3413871766", -- Image2 url
                            Shake = true,
                            Sound1 = {
                                3537873683, -- SoundId
                                { Volume = 2 }, -- Sound properties
                            },
                            Sound2 = {
                                6459610652, -- SoundId
                                { Volume = 0.5 }, -- Sound properties
                            },
                            Flashing = {
                                true, -- Enabled/Disabled
                                Color3.fromRGB(255,0,0), -- Color
                            },
                            Tease = {
                                true, -- Enabled/Disabled
                                Min = 1,
                                Max = 1,
                            },
                        },
                    },
                    CustomDialog = {"You died to who you call PrimesA-60...", "Try your best to out-run him.", "I really don't have nothing else", "Just try your best to Hide when you can."}, -- Custom death message
                })

                ------------------------
                Creator.runEntity(entity7)
                -- Run the created entity
            end)
        end
    end


























pcall(function()
local DepthPas = coroutine.wrap(Depth)
DepthPas()
end)
pcall(function()
    local TraumaPas = coroutine.wrap(TraumaSpawn)   
    TraumaPas()
end)
pcall(function()
local SmilerPas = coroutine.wrap(SmilerSpawn)
SmilerPas()
end)
pcall(function()
local VhsSansPas = coroutine.wrap(VhsSansSpawn)
VhsSansPas()
end)
pcall(function()
local VhsSasPas = coroutine.wrap(VhsSasSpawn)
VhsSasPas()
end)
pcall(function()
local VhsSaisPas = coroutine.wrap(VhsSaisSpawn)
VhsSaisPas()
end)
pcall(function()
local VhsSiasPas = coroutine.wrap(VhsSiasSpawn)
VhsSiasPas()
end)
pcall(function()
local VhsSanhPas = coroutine.wrap(VhsSanhSpawn)
VhsSanhPas()
end)
pcall(function()
local VhsSPas = coroutine.wrap(VhsSSpawn)
VhsSPas()
end)
pcall(function()
local TrauPas = coroutine.wrap(TrauSpawn)
TrauPas()
end)
pcall(function()
    local TrauaPas = coroutine.wrap(TrauaSpawn)   
    TrauaPas()
end)
pcall(function()
    local TrakuPas = coroutine.wrap(TrakuSpawn)   
    TrakuPas()
end)
workspace.ChildAdded:Connect(function(seek)
	if seek.Name == "SeekMoving" then
		firesignal(game.ReplicatedStorage.Bricks.Caption.OnClientEvent, "I feel like im being watched...")
		wait(0.5)
		seek.SeekRig.Head.Eye.Decal.Texture = "rbxassetid://11523633591"
		seek.Figure.Scream.SoundId = "rbxassetid://9113985604"
		seek.Figure.Scream.Pitch = 0.8
		workspace.Ambience_eek.SoundId = "rbxassetid://9046421438"
		seek.Figure.Scream.RollOffMaxDistance = 10000
		seek.Figure.Scream.RollOffMinDistance = 10
		seek.SeekRig.LeftLowerArm.Color = Color3.new(1,0,0)
		seek.SeekRig.LeftLowerArm.Material = "Neon"
		seek.SeekRig.RightLowerLeg.Color = Color3.new(1,0,0)
		seek.SeekRig.RightLowerLeg.Material = "Neon"
		seek.SeekRig.RightUpperArm.Color = Color3.new(1,0,0)
		seek.SeekRig.RightUpperArm.Material = "Neon"
		local eye1 = game:GetObjects("rbxassetid://11574477069")[1]
		eye1.Parent = seek.SeekRig.Head
		local weldingconstraint = Instance.new("WeldConstraint", seek.SeekRig.Head)
		eye1:PivotTo(seek.SeekRig.Head.CFrame)
		weldingconstraint.Part0 = seek.SeekRig.Head
		weldingconstraint.Part1 = eye1.Part
	else

	end
end)

workspace.Ambience_Figure.SoundId = "rbxassetid://6385111188"

local CF = CFrame.new
local nicefrane = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
local sussyroom = game:GetObjects("rbxassetid://11626479968")[1]
sussyroom.Parent = workspace
wait(2)
local CameraShaker = require(game.ReplicatedStorage.CameraShaker)
		local camara = game.Workspace.CurrentCamera
		local camShake = CameraShaker.new(Enum.RenderPriority.Camera.Value, function(shakeCf)
			camara.CFrame = camara.CFrame * shakeCf
		end)
		camShake:Start()
		camShake:ShakeOnce(300,300,0.3,0.5)
		wait(0.5)
game.Players.LocalPlayer.Character:PivotTo(CF(game.Workspace.TestCustomRoom.sussy_part.Position))
game:GetService("Workspace").TestCustomRoom.sussy_part2.Touched:Connect(function()
game.Players.LocalPlayer.Character:PivotTo(CF(0.352394, -0.3796, 3263.22))
game.Lighting.MainColorCorrection.TintColor = Color3.fromRGB(255, 147, 15)
game.Lighting.MainColorCorrection.Contrast = 1
camShake:ShakeOnce(300,300,0.3,0.5)
		local TweenService = game:GetService("TweenService")
		local TW = TweenService:Create(game.Lighting.MainColorCorrection, TweenInfo.new(math.random(2.5,3)),{TintColor = Color3.fromRGB(255, 255, 255)})
		TW:Play()
wait(0.3)
local tween = game:GetService("TweenService")
tween:Create(game.Lighting.MainColorCorrection, TweenInfo.new(6), {Contrast = 0}):Play()
end)
pcall(function()
spawn(function()
	while wait() do
	local currentroomnumber = game:GetService("ReplicatedStorage").GameData.LatestRoom.Value
		if workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door") ~= nil then
		 if workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door"):FindFirstChild("Door") ~= nil then
			workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door"):FindFirstChild("Door").Material = Enum.Material.Slate
			workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door"):FindFirstChild("Door").Color = Color3.new(0.341176, 0.341176, 0.341176)
		    end
		end
	end
end)
spawn(function()
	while wait() do
	local currentroomnumber = game:GetService("ReplicatedStorage").GameData.LatestRoom.Value
		if workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door") ~= nil then
		 if workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door"):FindFirstChild("Door") ~= nil then
		 if workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door"):FindFirstChild("Door"):FindFirstChild("Sign") ~= nil then
		 workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door").Sign:Destroy()
		 workspace["CurrentRooms"][currentroomnumber]:FindFirstChild("Door"):FindFirstChild("Door"):FindFirstChild("Sign"):Destroy()
                end
		    end
		end
	end
end)
end)
workspace["The Damned"]:Play()
workspace["The Damned"].SoundId = "rbxassetid://9113731836"
workspace["The Damned"].Pitch = 1
workspace["The Damned"].Looped = true
workspace["The Damned"].Volume = 1
function ambiance()
	while true do
		local ambiencefirst = Instance.new("Sound", workspace)
		ambiencefirst.SoundId = "rbxassetid://12229501"
		ambiencefirst.Pitch = 0.11
		ambiencefirst:Play()
		wait(120)
	end
end

local usecrucifix1time = true
local function IsVisible(part)
    local vec, found=workspace.CurrentCamera:WorldToViewportPoint(part.Position)
    local onscreen = found and vec.Z > 0
    local cfg = RaycastParams.new()
    cfg.FilterType = Enum.RaycastFilterType.Blacklist
    cfg.FilterDescendantsInstances = {part}
 
    local cast = workspace:Raycast(part.Position, (game.Players.LocalPlayer.Character.UpperTorso.Position - part.Position), cfg)
    if onscreen then
        if cast and (cast and cast.Instance).Parent==game.Players.LocalPlayer.Character then
            return true
        end
    end
end
 
local Equipped = false
 
-- Edit this --
getgenv().spawnKey = Enum.KeyCode.F4
---------------
 
-- Services
 
local Players = game:GetService("Players")
local UIS = game:GetService("UserInputService")
 
-- Variables
 
local Plr = Players.LocalPlayer
local Char = Plr.Character or Plr.CharacterAdded:Wait()
local Hum = Char:WaitForChild("Humanoid")
local Root = Char:WaitForChild("HumanoidRootPart")
local RightArm = Char:WaitForChild("RightUpperArm")
local LeftArm = Char:WaitForChild("LeftUpperArm")
 
local RightC1 = RightArm.RightShoulder.C1
local LeftC1 = LeftArm.LeftShoulder.C1
 
local SelfModules = {
    Functions = loadstring(
        game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Functions.lua")
    )(),
    CustomShop = loadstring(
        game:HttpGet(
            "https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors/Custom%20Shop%20Items/Source.lua"
        )
    )(),
}
 
local ModuleScripts = {
    MainGame = require(Plr.PlayerGui.MainUI.Initiator.Main_Game),
    SeekIntro = require(Plr.PlayerGui.MainUI.Initiator.Main_Game.RemoteListener.Cutscenes.SeekIntro),
}
 
-- Functions
 
local function setupCrucifix(tool)
    tool.Equipped:Connect(function()
        Equipped = true
        Char:SetAttribute("Hiding", true)

    end)
 
    tool.Unequipped:Connect(function()
        Equipped = false
        Char:SetAttribute("Hiding", nil)
    end)
end
 
-- Scripts
 
local CrucifixTool = game:GetObjects("rbxassetid://12441313237")[1]
CrucifixTool.Name = "Crucifix"
CrucifixTool.Parent = game.Players.LocalPlayer.Backpack
 
-- game.UserInputService.InputBegan:Connect(function(input, proc)
--     if proc then return end
 
--     if input.KeyCode == input.KeyCode[getgenv().spawnKey] then
--         local CrucifixTool = game:GetObjects("rbxassetid://11590476113")[1]
--         CrucifixTool.Name = "Crucifix"
--         CrucifixTool.Parent = game.Players.LocalPlayer.Backpack
--     end
-- end)
-- Input handler
 
setupCrucifix(CrucifixTool)
 
local Players = game:GetService("Players")
local UIS = game:GetService("UserInputService")
 
-- Variables
start = false
durability = 100
max = 100
local Plr = Players.LocalPlayer
local Char = Plr.Character or Plr.CharacterAdded:Wait()
local Hum = Char:WaitForChild("Humanoid")
local Root = Char:WaitForChild("HumanoidRootPart")
local tool = CrucifixTool
local handle = CrucifixTool.Handle
local dupeCrucifix = Instance.new("BindableEvent")
local start = true


local function func(ins)
    wait(.01) -- Wait for the attribute
    if ins:GetAttribute("IsCustomEntity")==true and ins:GetAttribute("ClonedByCrucifix")~=true then
        local Chains = game:GetObjects("rbxassetid://12537077765")[1]
        Chains.Parent = workspace
        local chained = true
        local posTime = false
        local rotTime = false
        local tweenTime = false
        local intFound = true
        game:GetService("RunService").RenderStepped:Connect(function()
            if Equipped then
                if ins.Parent~=nil and ins.PrimaryPart and IsVisible(ins.PrimaryPart) and (Root.Position-ins.PrimaryPart.Position).magnitude <= 25 then
        
        local start = false
        local handle2 = handle:Clone()
        handle2.CFrame = CFrame.lookAt(handle2.Position, ins:FindFirstChild("RushNew").Position)
        local Transparency = 1
        
        game["Run Service"].Heartbeat:Connect(function()
            local Transparency = 1
if not handle2 then
	return
elseif not handle2:FindFirstChild("Glow") then
	return
elseif not tool then
	return
end
	if start == true then
		acceleration += 0.007
		
		handle2.Glow.Orientation += Vector3.new(0,acceleration,0)
		if acceleration >= 3 then
		    
		    acceleration = 0
local Transparency = 1
					    game.TweenService
:Create(
	handle2.Glow,
	TweenInfo.new(0.4),
	{ Size = handle2.Glow.Size * Vector3.new(2.178, 1.885, 0.407) }
)
:Play()
game.TweenService
:Create(
	handle2.Glow,
	TweenInfo.new(0.4),
	{ Transparency = Transparency}
)
:Play()


		end
	else
		acceleration = 0
		handle.Glow.Transparency = 1
	end
end)
        handle2.Anchored = true
        handle2.Parent = workspace
        handle2.Transparency = 1
        handle2.Glow.Transparency = 0

                    local c=ins:Clone()
                    c:SetAttribute("ClonedByCrucifix", true)
                    c.RushNew.Anchored=true
                    c.Parent=ins.Parent
                    ins:Destroy()
                    dupeCrucifix:Fire(6,c.RushNew)
 
 
 
                    -- Chains.PrimaryPart.Orientation = Chains.PrimaryPart.Orientation + Vector3.new(0, 3, 0)
 
                    local EntityRoot = c:FindFirstChild("RushNew")
                            --Made by Nljoram3
game.RunService.RenderStepped:Connect(function()
Chains.Entity.CFrame = EntityRoot.CFrame
end)

          game.RunService.RenderStepped:Connect(function()
              start = true
	if start == true then
		acceleration += 0.0003
		handle2.Glow.Orientation += Vector3.new(0,acceleration,0)
		handle2.Anchored = true
		if acceleration >= 40.6 then
local Transparency = 1
					    game.TweenService
:Create(
	handle2.Glow,
	TweenInfo.new(0.4),
	{ Size = handle2.Glow.Size * Vector3.new(2.178, 1.885, 0.407) }
)
:Play()
game.TweenService
:Create(
	handle2.Glow,
	TweenInfo.new(0.4),
	{ Transparency = Transparency}
)
:Play()
		end
	else

	end
end)

                        if usecrucifix1time == true then
                            handle.Parent:Destroy()
                        end
                        
                    if EntityRoot then
 	   Chains:PivotTo(EntityRoot.CFrame - Vector3.new(0,3,0))
       handle2.Sound:Play()
         
           ModuleScripts.MainGame.camShaker:ShakeOnce(9, 25, 0.7, 0.7)
                                      game.TweenService
                                :Create(
                                    handle2,
                                    TweenInfo.new(1),
                                    { CFrame = handle2.CFrame * CFrame.new(0, 3, -3) }
                                )
                                :Play()
                                
                        task.wait(1.35)

 
                            game.TweenService
                                :Create(
                                    EntityRoot,
                                    TweenInfo.new(2),
                                    { CFrame = EntityRoot.CFrame * CFrame.new(0, -1.7, 0) }
                                )
                                :Play()
                                
 task.wait(1)
 ModuleScripts.MainGame.camShaker:ShakeOnce(7, 25, 3, 2)
 task.wait(1)

 
                             game.TweenService
                                :Create(
                                    EntityRoot,
                                    TweenInfo.new(1),
                                    { CFrame = EntityRoot.CFrame * CFrame.new(0, 2.5, 0) }
                                )
                                :Play()
                                
 task.wait(.9)
                              game.TweenService
                                :Create(
                                    EntityRoot,
                                    TweenInfo.new(.134),
                                    { CFrame = EntityRoot.CFrame * CFrame.new(0, 2.3, 0) }
                                )
                                :Play()

                                task.wait(.134564)
                              game.TweenService
                                :Create(
                                    EntityRoot,
                                    TweenInfo.new(.9),
                                    { CFrame = EntityRoot.CFrame * CFrame.new(0, 2.5, 0) }
                                )
                                :Play()

                                
 task.wait(1.2)
                                ModuleScripts.MainGame.camShaker:ShakeOnce(5, 25, 1.8, 2)
                             game.TweenService
                                :Create(
                                    EntityRoot,
                                    TweenInfo.new(16.7),
                                    { CFrame = EntityRoot.CFrame * CFrame.new(0, -150, 0) }
                                )
                                :Play()
task.wait(0.8)
                                                             game.TweenService
                                :Create(
                                    EntityRoot.Footsteps,
                                    TweenInfo.new(2),
                                    { Volume = 0 }
                                )
                                :Play()
                                                                                             game.TweenService
                                :Create(
                                    EntityRoot.PlaySound,
                                    TweenInfo.new(2),
                                    { Volume = 0 }
                                )
                                :Play()
 
                             
                            tweenTime = true
                            task.wait(1.5)
                            intFound = false
                            game:GetService("Debris"):AddItem(c, 0)
                            task.wait(1)
                            Chains.BeamFlat1:Destroy()
                            task.wait(.5)
                            Chains.BeamFlat2:Destroy()
                            task.wait(.5)
                            wait(0.7)
                            Chains.BeamFlat3:Destroy()
                            wait(2)
                            Chains.BeamFlatCircle:Destroy()
                             Chains:Destroy()
wait(3)
                             handle2:Destroy()
                    end
                end
            end
        end)
    elseif ins.Name=="Eyes" then

        local CrucifixTool = game.Players.LocalPlayer.Character:FindFirstChild("Crucifix")
        local tool = CrucifixTool
        local handle = CrucifixTool.Handle
        local handle2 = handle:Clone()
        handle2.Anchored = true
        local start = false
        local c=ins
        task.spawn(function()
            repeat task.wait() until IsVisible(c.Core) and Equipped and c.Core.Attachment.Eyes.Enabled==true
            local pos=c.Core.Position
            dupeCrucifix:Fire(18.364, c.Core)
            task.spawn(function()
                local Chains = game:GetObjects("rbxassetid://11555754461")[1]
                Chains.Parent = workspace
                game.RunService.RenderStepped:Connect(function()
wait(0.01)
Chains.Base.CFrame = Chains.Base.CFrame * CFrame.fromEulerAnglesXYZ(0,0,0.006)
end)

        handle2.Anchored = true
        handle2.Parent = workspace
        handle2.Transparency = 1
        handle2.Glow.Transparency = 0
                                              game.TweenService
                                :Create(
                                    handle2,
                                    TweenInfo.new(1),
                                    { CFrame = handle2.CFrame * CFrame.new(0, 3, -3) }
                                )
                                :Play()
 	   Chains:PivotTo(c.Core.CFrame - Vector3.new(0,6.9,0))
	   Chains.Chain1.Attachment:FindFirstChildOfClass("Beam").Attachment1 = c.Core.Attachment
	   Chains.Chain2.Attachment:FindFirstChildOfClass("Beam").Attachment1 = c.Core.Attachment
	   Chains.Chain3.Attachment:FindFirstChildOfClass("Beam").Attachment1 = c.Core.Attachment
	   Chains.Chain4.Attachment:FindFirstChildOfClass("Beam").Attachment1 = c.Core.Attachment
                     
         
                c:SetAttribute("Killing", true)
                ModuleScripts.MainGame.camShaker:ShakeOnce(10, 10, 5, 0.15)
                handle2.Charge:Play()
                wait(2)
                c.Core.Initiate:Stop()
                for i=1,3 do
                    c.Core.Repent:Play()  
                    c.Core.Attachment.Angry.Enabled=true
                    ModuleScripts.MainGame.camShaker:ShakeOnce(8, 8, 1.3, 0.15)
                    delay(c.Core.Repent.TimeLength, function() c.Core.Attachment.Angry.Enabled=false end)
                    wait(2.5)
                end
                c.Core.Scream:Play();
                ModuleScripts.MainGame.camShaker:ShakeOnce(8, 8, c.Core.Scream.TimeLength, 0.15);
                (c.Core:FindFirstChild"whisper" or c.Core:FindFirstChild"Ambience"):Stop()
                for _, l in pairs(c:GetDescendants()) do
                    if l:IsA("PointLight") then
                        l.Enabled=false
                    end
                end
                game:GetService("TweenService"):Create(c.Core, TweenInfo.new(3, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut), {
                    CFrame=CFrame.new(c.Core.CFrame.X, c.Core.CFrame.Y-12, c.Core.CFrame.Z)
                }):Play()

            end)
            
            local col=game.Players.LocalPlayer.Character.Collision
 
            local function CFrameToOrientation(cf)
                local x, y, z = cf:ToOrientation()
                return Vector3.new(math.deg(x), math.deg(y), math.deg(z))
            end
 
            while c.Parent~=nil and c.Core.Attachment.Eyes.Enabled==true do
                -- who's the boss now huh?
                col.Orientation = CFrameToOrientation(CFrame.lookAt(col.Position, pos)*CFrame.Angles(0, math.pi, 0))
                task.wait()
            end
        end)
    elseif ins.Name=="Shade" and ins.Parent==workspace.CurrentCamera and ins:GetAttribute("ClonedByCrucifix")==nil then
        task.spawn(function()
            repeat task.wait() until IsVisible(ins) and (Root.Position-ins.Position).Magnitude <= 12.5 and Equipped
 
            local clone = ins:Clone()
 
            clone.CFrame = ins.CFrame
            clone.Parent = ins.Parent
            clone.Anchored = true
 
            ins:Remove()
 
            dupeCrucifix:Fire(13, ins)
            ModuleScripts.MainGame.camShaker:ShakeOnce(40, 10, 5, 0.15)
 
 
 
            for _, thing in pairs(clone:GetDescendants()) do
                if thing:IsA("SpotLight") then
                    game:GetService("TweenService"):Create(thing, TweenInfo.new(5), {
                        Brightness=thing.Brightness*5
                    }):Play()
                elseif thing:IsA("Sound") and thing.Name~="Burst" then
                    game:GetService("TweenService"):Create(thing, TweenInfo.new(5), {
                        Volume=0
                    }):Play()
                elseif thing:IsA("TouchTransmitter") then thing:Destroy() end
            end
 
            for _, pc in pairs(clone:GetDescendants()) do
                if pc:IsA("ParticleEmitter") then
                        pc.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 0, 4)), ColorSequenceKeypoint.new(0.48, Color3.fromRGB(182, 0, 3)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(255, 0, 4))}
                end
            end
 
            local Original_color = {}
 
            local light
            light = game.Lighting["Ambience_Shade"]
            game:GetService("TweenService"):Create(light, TweenInfo.new(1), {
 
 
            }):Play()
 
            wait(5)
 
            clone.Burst.PlaybackSpeed=0.5
            clone.Burst:Stop()
            clone.Burst:Play()
            light.TintColor = Color3.fromRGB(215,253,255)
            game:GetService("TweenService"):Create(clone, TweenInfo.new(6), {
                CFrame=CFrame.new(clone.CFrame.X, clone.CFrame.Y-12, clone.CFrame.Z)
            }):Play()
            wait(8.2)
 
            game:GetService("Debris"):AddItem(clone, 0)
            game.ReplicatedStorage.Bricks.ShadeResult:FireServer()
        end)
    end
end
 
workspace.ChildAdded:Connect(func)
workspace.CurrentCamera.ChildAdded:Connect(func)
for _, thing in pairs(workspace:GetChildren()) do
    func(thing)
end
dupeCrucifix.Event:Connect(function(time, entityRoot)
    local Cross = game:GetObjects("rbxassetid://12421557552")[1]
    Cross.Parent = workspace
 
    local fakeCross = Cross.Handle
 
    -- fakeCross:FindFirstChild("EffectLight").Enabled = true
 
    ModuleScripts.MainGame.camShaker:ShakeOnce(35, 25, 0.15, 0.15)
    -- you tell me i didnt make?
    fakeCross.CFrame = CFrame.lookAt(CrucifixTool.Handle.Position, entityRoot.Position)
 
    -- hl.Parent = model
    -- hl.FillTransparency = 1
    -- hl.OutlineColor = Color3.fromRGB(75, 177, 255)
    fakeCross.Anchored = true
 
    CrucifixTool:Destroy()
 
    -- for i, v in pairs(fakeCross:GetChildren()) do
    --     if v.Name == "E" and v:IsA("BasePart") then
    --         v.Transparency = 0
    --         v.CanCollide = false
    --     end
    --     if v:IsA("Motor6D") then
    --         v.Name = "Motor6D"
    --     end
    -- end
 
    task.wait(time)
    fakeCross.Anchored = false
    fakeCross.CanCollide = true
    task.wait(0.5)
    Cross:Remove()
end)
