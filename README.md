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
        while true do wait(80)
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
        while true do wait(590)
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
		wait(0.9)
		seek.SeekRig.Head.Eye.Decal.Texture = "rbxassetid://11523633591"
		seek.Figure.Scream.SoundId = "rbxassetid://9113985604"
		seek.Figure.Scream.Pitch = 2.8
		workspace.Ambience_Seek.SoundId = "rbxassetid://1839924741 "
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
