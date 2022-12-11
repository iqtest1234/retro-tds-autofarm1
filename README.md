if game.PlaceId == 7215261025 then
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-131.541016, 180.296371, -151.775513, -0.0575901866, 4.21997584e-08, -0.998340309, 1.8343107e-09, 1, 4.21640998e-08, 0.998340309, 5.96972027e-10, -0.0575901866)
end
if game.PlaceId == 11308981067 then
wait(1)
local args = {
    [1] = "Scout",
    [2] = Vector3.new(-1306.9373779296875, 40.326263427734375, 1077.659423828125),
    [3] = game:GetService("Players").LocalPlayer.PlayerGui.HUD.Troops.Tower1
}

game:GetService("ReplicatedStorage").PlaceTower:FireServer(unpack(args))
wait(50)
game:GetService("ReplicatedStorage").Skipping.Vote:FireServer()
wait(20)
local args = {
    [1] = workspace.Towers.Scout
}

game:GetService("ReplicatedStorage").UpgradeTower:FireServer(unpack(args))
wait(50)
game:GetService("ReplicatedStorage").Skipping.Vote:FireServer()
wait(17)
game:GetService("TeleportService"):Teleport(7215261025)
end
