local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "King HUB", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})


local MainTab = Window:MakeTab({
	Name = "Player",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

OrionLib:MakeNotification({
	Name = "Teste",
	Content = "Notification content... what will it say??",
	Image = "rbxassetid://4483345998",
	Time = 5
})

MainTab:AddToggle({
	Name = "oi",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})
    --// Check Quest
    function CheckLevel()
        local Lv = game:GetService("Players").LocalPlayer.Data.Level.Value
        if First_Sea then
        if Lv == 1 or Lv <= 9 or SelectMonster == "Bandit" or SelectArea == 'Jungle' then -- Bandit
        Ms = "Bandit"
        NameQuest = "BanditQuest1"
        QuestLv = 1
        NameMon = "Bandit"
        CFrameQ = CFrame.new(1060.9383544922, 16.455066680908, 1547.7841796875)
        CFrameMon = CFrame.new(1038.5533447266, 41.296249389648, 1576.5098876953)
        elseif Lv == 10 or Lv <= 14 or SelectMonster == "Monkey" or SelectArea == 'Jungle' then -- Monkey




