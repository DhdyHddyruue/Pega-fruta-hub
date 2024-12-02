-- Script para pegar frutas automaticamente no Blox Fruits
while true do
    wait(1)
    for i, v in pairs(game.Workspace:GetChildren()) do
        if v:IsA("Tool") and v.Name == "Fruit" then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame
            wait(0.5)
            fireclickdetector(v.Handle.ClickDetector)
        end
    end
end
