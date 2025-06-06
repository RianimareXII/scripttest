local Players = game:GetService("Players")
local LocalPlayer = Players.LocalPlayer

local function sendChatMessage(msg)
    game.ReplicatedStorage.DefaultChatSystemChatEvents.SayMessageRequest:FireServer(msg, "All")
end

LocalPlayer.Chatted:Connect(function(msg)
    if msg:lower() == "/start" then
        sendChatMessage("Скрипт активирован")
        wait(0.2)
        sendChatMessage("script by RianimareXII")
    end
end)
