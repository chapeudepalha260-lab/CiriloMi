# CiriloMi
task.spawn(function()
    repeat task.wait() until game:IsLoaded() and game.Players.LocalPlayer
    task.wait(1)
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetTeam", "Pirates")
end)

task.spawn(function()
    repeat task.wait() until game:IsLoaded() and game.Players.LocalPlayer.Character
    pcall(function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/AnhDangNhoEm/TuanAnhIOS/refs/heads/main/CiriloMi"))()
    end)
end)
