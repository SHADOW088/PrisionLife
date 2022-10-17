local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()

local win = DiscordLib:Window("DirectServer")

local serv = win:Server("Script", "")

local q = serv:Channel("Info")

local w = serv:Channel("Player")

local e = serv:Channel("Local")

local r = serv:Channel("Admin")

q:Label("===================DIRECTSERVER=================")

q:Label("Note: Thx for using the script!")

q:Label("Scripter: Error0242#0170")

q:Label ("Discordserver: https://discord.gg/ndMmjhDw")

w:Label("<====================WEAPONS==================>")

w:Button("Ak-47", function()
        local args = {
    [1] = workspace.Prison_ITEMS.giver["AK-47"].ITEMPICKUP
}

workspace.Remote.ItemHandler:InvokeServer(unpack(args))
end)

w:Button("Remington", function()
        local args = {
    [1] = workspace.Prison_ITEMS.giver["Remington 870"].ITEMPICKUP
}

workspace.Remote.ItemHandler:InvokeServer(unpack(args))
end)

w:Button("M9", function()
        local args = {
    [1] = workspace.Prison_ITEMS.giver.M9.ITEMPICKUP
}

workspace.Remote.ItemHandler:InvokeServer(unpack(args))
end)

w:Label("<====================HUMANOID==================>")

w:Textbox("WalkSpeed", "Hare!", true, function(t)
    local Player = game.Players.LocalPlayer
    Player.Character.Humanoid.WalkSpeed = t
end)

w:Textbox("JumpPower", "Hare!", true, function(t)
    local Player = game.Players.LocalPlayer
    Player.Character.Humanoid.JumpPower  = t
end)

w:Label("<====================TEAMS====================>")

w:Button("Guard Team", function()
local args = {
    [1] = "Bright blue"
}

workspace.Remote.TeamEvent:FireServer(unpack(args))
local args = {
    [1] = "Error0242"
}

workspace.Remote.loadchar:InvokeServer(unpack(args))
end)

w:Button("InmateTeam", function()
local args = {
    [1] = "Bright orange"
}

workspace.Remote.TeamEvent:FireServer(unpack(args))

local args = {
    [1] = "Error0242"
}

workspace.Remote.loadchar:InvokeServer(unpack(args))
end)

w:Label("<======================TP======================>")

w:Button("Prision", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(924.399658, 99.9899826, 2388.50073, -1, 0, 0, 0, 1, 0, 0, 0, -1)
end)

w:Button("Police Room", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(835.008972, 99.9899826, 2311.98584, 0.999964535, 1.00178063e-07, -0.00842255261, -9.99406637e-08, 1, 2.86076105e-08, 0.00842255261, -2.77648411e-08, 0.999964535)
end)

w:Button("CriminalBase", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-919.982056, 94.1287613, 2062.64819, 0.00146690395, 3.05949541e-08, 0.999998927, 2.89634059e-08, 1, -3.0637473e-08, -0.999998927, 2.90083175e-08, 0.00146690395)
end)    

w:Button("Yard", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(778.381897, 97.9999237, 2462.85303, -0.9997105, 3.40313981e-08, 0.0240603928, 3.59947236e-08, 1, 8.11667391e-08, -0.0240603928, 8.20092865e-08, -0.9997105)
end)

w:Button("PrisionEntrance", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(522.09613, 98.039917, 2215.78076, -0.0295868292, 7.55666036e-08, 0.999562204, 5.22465875e-08, 1, -7.40532116e-08, -0.999562204, 5.0032714e-08, -0.0295868292)
end)

w:Button("SniperWall", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(822.959229, 130.039902, 2582.1958, 0.999391913, 4.739098e-08, 0.034868218, -4.78131454e-08, 1, 1.12736043e-08, -0.034868218, -1.29339082e-08, 0.999391913)
end)

r:Button("Admin", function()
    loadstring(game:HttpGet"https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source")()
end)

e:Button("DestroyDoor", function()
    
end)

e:Button("Admin", function()
    loadstring(game:HttpGet"https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source")()
end)

e:Button("Admin", function()
    loadstring(game:HttpGet"https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source")()
end)

e:Button("Admin", function()
    loadstring(game:HttpGet"https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source")()
end)

