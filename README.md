local serv2 = win:Server("⭐️Viet Nam Piece⭐️", "")
local dropsVN = serv2:Channel("main")

dropsVN:Button("kill aura", function()
    getgenv().G = true
    getgenv().Creator = 'https://discord.gg/B3HqPPzFYr - HalloweenGaster'
    spawn(function()
        while getgenv().G and getgenv().Creator == 'https://discord.gg/B3HqPPzFYr - HalloweenGaster' do
            wait(0.9)
            sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", 112412400000)
            sethiddenproperty(game.Players.LocalPlayer, "MaxSimulationRadius", 112412400000)
            for _, d in pairs(game.Workspace:GetDescendants()) do
                if d:IsA("Humanoid") and d.Parent.Name ~= game.Players.LocalPlayer.Name then
                    d.Health = 0
                end
            end
        end
    end)
end)

dropsVN:Button("simple spy", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/realredz/SimpleSpy/refs/heads/main/Mobile.lua"))()
end)

dropsVN:Button("turtle spy", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Turtle-Brand/Turtle-Spy/main/source.lua", true))()
end)

dropsVN:Button("inf yield", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)

local dropsArmors = serv2:Channel("armors")
dropsArmors:Button("copy all armor of sv", function()
    local Players = game:GetService("Players")
    local armors = {"Cursed-Armor", "Unique-Armor", "Darkness-Armor", "Thunder-Armor", "Thunder-Armor", "Diamond-Armor", "Golden-Armor", "Epic-Armor", "Iron-Armor", "Wooden-Armor"}
    for _, player in pairs(Players:GetPlayers()) do
        local backpack = player:FindFirstChild("Backpack")
        if backpack then
            for _, armorName in pairs(armors) do
                local armor = backpack:FindFirstChild(armorName)
                if armor and armor:FindFirstChild("K") and armor.K:FindFirstChild("Fire") then
                    armor.K.Fire:FireServer()
                end
            end
        end
    end
end)

local dropsFastAttack = serv2:Channel("fast attack")

-- Ví dụ nút “cid”
dropsFastAttack:Button("cid", function()
    local args = { [1] = 8, [2] = 1 }
    spawn(function()
        while true do
            pcall(function()
                game:GetService("Players").LocalPlayer.PlayerGui.Tengen.Skill1b.Z.TextButtonm1.Hitbox:FireServer(unpack(args))
            end)
            wait(0.1)
        end
    end)
end)

-- Nút “geto”
dropsFastAttack:Button("geto", function()
    local args = { [1] = 8, [2] = 1 }
    spawn(function()
        while true do
            pcall(function()
                game:GetService("Players").LocalPlayer.PlayerGui.Tengen.Skill1b.Z.TextButtonm1.Hitbox:FireServer(unpack(args))
            end)
            wait(0.1)
        end
    end)
end)

-- Nút “guts”
dropsFastAttack:Button("guts", function()
    local args = { [1] = 8, [2] = 1 }
    spawn(function()
        while true do
            pcall(function()
                game:GetService("Players").LocalPlayer.PlayerGui.Zabuza.Skill1b.Z.TextButtonm1.Hitbox:FireServer(unpack(args))
            end)
            wait(0.1)
        end
    end)
end)

-- Nút “escanor” (sửa lỗi thiếu end và thêm spawn)
dropsFastAttack:Button("escanor", function()
    local args = { [1] = 8, [2] = 1 }
    spawn(function()
        while true do
            pcall(function()
                game:GetService("Players").LocalPlayer.PlayerGui.Zabuza.Skill1b.Z.TextButtonm1.Hitbox:FireServer(unpack(args))
            end)
            wait(0.1)
        end
    end)
end)

-- Nút “yorus v3”
dropsFastAttack:Button("yorus v3", function()
    local args = { [1] = 8, [2] = 3 }
    spawn(function()
        while true do
            pcall(function()
                game:GetService("Players").LocalPlayer.PlayerGui.YoruV3.Skill1b.Z.TextButtonm1.Hitbox:FireServer(unpack(args))
            end)
            wait(0.1)
        end
    end)
end)

local drops = serv2:Channel("quest")

drops:Button("you can get quest 500k at lv 20k lol", function()
end)

drops:Button("click npc and click quest 1,2,3", function()
end)

drops:Button("quest 1", function()
-- Script 3: Quest Accept 1
while wait() do
    game:GetService("Players").LocalPlayer.PlayerGui.QuestTake.Accept1.RemoteEvent:FireServer()
end
end)

drops:Button("quest 2 ", function()
-- Script 2: Quest Accept 2
while wait() do
    game:GetService("Players").LocalPlayer.PlayerGui.QuestTake.Accept2.RemoteEvent:FireServer()
end
end)

drops:Button("quest 3 ", function()
-- Script 1: Quest Accept 3
while wait() do
    game:GetService("Players").LocalPlayer.PlayerGui.QuestTake.Accept3.RemoteEvent:FireServer()
end
end)

local dropsRandom = serv2:Channel("random secret")
dropsRandom:Button("if script dont work, go to that island", function()
    -- Không có hành động nào
end)

dropsRandom:Button("secret sea 1", function()
    spawn(function()
        while true do
            pcall(function()
                fireclickdetector(game:GetService("Workspace").MAP["STARTER ISLAND [ Lv 1+ ]"]["Secret Random"].RANDOM)
            end)
            wait(0.1)
        end
    end)
end)

dropsRandom:Button("secret sea 2", function()
    spawn(function()
        while true do
            pcall(function()
                fireclickdetector(game:GetService("Workspace").MAP["STARTER ISLAND [ Lv 1+ ]"]["Secret Random"].RANDOM)
            end)
            wait(0.1)
        end
    end)
end)

dropsRandom:Button("yorus v3", function()
    spawn(function()
        while true do
            local clickDetector = game.Workspace:FindFirstChild("MAP")
                and game.Workspace.MAP:FindFirstChild("DAK ISLAND [Lv 1350+]")
                and game.Workspace.MAP["DAK ISLAND [Lv 1350+]"]:FindFirstChild("Yoru V3 random")
                and game.Workspace.MAP["DAK ISLAND [Lv 1350+]"]["Yoru V3 random"]:FindFirstChild("ClickDetector")
            if clickDetector then
                fireclickdetector(clickDetector)
            else
                warn("Không tìm thấy ClickDetector!")
            end
            wait(0.1)
        end
    end)
end)

dropsRandom:Button("wando sea 2", function()
    spawn(function()
        while true do
            local clickDetector = game.Workspace:FindFirstChild("Platinum Town [ 2000 - 3000 ]")
                and game.Workspace["Platinum Town [ 2000 - 3000 ]"]:FindFirstChild("PlatinumMAP")
                and game.Workspace["Platinum Town [ 2000 - 3000 ]"].PlatinumMAP:FindFirstChild("GodBox")
                and game.Workspace["Platinum Town [ 2000 - 3000 ]"].PlatinumMAP.GodBox:FindFirstChild("ClickDetector")
            if clickDetector then
                fireclickdetector(clickDetector)
            else
                warn("Không tìm thấy ClickDetector!")
            end
            wait(0.1)
        end
    end)
end)

local drops = serv2:Channel("teleports")

drops:Button("sea 1👇", function()
end)

drops:Button("started island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(485.583771, 35.5632935, -511.945404)

end)

drops:Button("snow island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-915.918945, 33.7605095, 282.443604)

end)

drops:Button("sand island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-708.765259, 69.1108398, 1745.13916)

end)

drops:Button("sky island ", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4594.52393, 4279.44092, 474.423523)

end)

drops:Button("end island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2223.75146, 36.3414612, 1965.90369)

end)

drops:Button("minhmama island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2569.90283, 51.1074524, -65.4458542)

end)

drops:Button("dark island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3465.68188, 66.2542191, 3718.19531)

end)

drops:Button("sea 2 👇", function()
end)

drops:Button("kaido island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-685, 87690, 789)

end)

drops:Button("platinum island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1258, 87700, 3260)

end)

drops:Button("marine island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-160, 87750, -2010)

end)

drops:Button("nickbeo island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1600, 87700, 637)

end)

drops:Button("garou island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1600, 87700, 1073)

end)

drops:Button("sukuna island", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1500, 87700, 2800)

end)

drops:Button("credits chon", function()
end)
