local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()

local win = DiscordLib:Window("discord library")

local serv = win:Server("Preview", "")

local Zero = serv:Channel("Weapons")

local One = serv:Channel("Player")

local Two = serv:Channel("Admin")


One:Button("InmateTeam", function()
local args = {
    [1] = "Bright orange"
}

workspace.Remote.TeamEvent:FireServer(unpack(args))

local args = {
    [1] = "Error0242"
}

workspace.Remote.loadchar:InvokeServer(unpack(args))
end)

One:Button("Guard Team", function()
local args = {
    [1] = "Bright blue"
}

workspace.Remote.TeamEvent:FireServer(unpack(args))
local args = {
    [1] = "Error0242"
}

workspace.Remote.loadchar:InvokeServer(unpack(args))
end)


One:Textbox("WalkSpeed", "Hare!", true, function(t)
    local Player = game.Players.LocalPlayer
    Player.Character.Humanoid.WalkSpeed = t
end)

One:Textbox("JumpPower", "Hare!", true, function(t)
    local Player = game.Players.LocalPlayer
    Player.Character.Humanoid.JumpPower  = t
end)







Two:Button("Admin", function()
    loadstring(game:HttpGet"https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source")()
end)

Zero:Button("AK-47", function()
    local args = {
    [1] = workspace.Prison_ITEMS.giver["AK-47"].ITEMPICKUP
}

workspace.Remote.ItemHandler:InvokeServer(unpack(args))
end)

Zero:Button("Remington 870", function()
    local args = {
    [1] = workspace.Prison_ITEMS.giver["Remington 870"].ITEMPICKUP
}

workspace.Remote.ItemHandler:InvokeServer(unpack(args))
end)

Zero:Button("M9", function()
    local args = {
    [1] = workspace.Prison_ITEMS.giver.M9.ITEMPICKUP
}

workspace.Remote.ItemHandler:InvokeServer(unpack(args))
end)













