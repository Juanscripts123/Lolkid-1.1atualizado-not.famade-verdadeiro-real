--carregar biblioteca 
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

local Window = Fluent:CreateWindow({
    Title = "LOLKID HUB" .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "Scripts" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
--parágrafos
Tabs.Main:AddParagraph({ Title = "expl₩ lolkid", Content = "This is a paragraph.\nSecond line!" })
--botões 
Tabs.Main:AddButton({ Title = "tralalelo funk", Callback = function() local soundId = "rbxassetid://109188610023287" 

local sound = Instance.new("Sound")
sound.SoundId = soundId
sound.Parent = workspace -- Ou, se for um LocalScript, player.Character ou player.CharacterAdded:Wait()

sound:Play() end })





