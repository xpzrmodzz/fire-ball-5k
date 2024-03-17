while true do wait
local args = {
    [1] = "damage",
    [2] = {
        ["EnemyHumanoid"] = workspace.MAP:FindFirstChild("5k_dummies").Dummy2.Humanoid
    }
}

game:GetService("ReplicatedStorage").SkillsInRS.RemoteEvent:FireServer(unpack(args))
end
