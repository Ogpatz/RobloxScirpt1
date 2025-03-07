local module = {}

function module.Run()
    local event = game.ReplicatedStorage:WaitForChild("PaTzEvents"):WaitForChild("KillAll")

    event.OnServerEvent:Connect(function()
        for _, player in pairs(game.Players:GetPlayers()) do
            if player.Character and player.Character:FindFirstChild("Humanoid") then
                player.Character.Humanoid.Health = 0 -- Kill den Spieler
            end
        end
    end)
end

return module
