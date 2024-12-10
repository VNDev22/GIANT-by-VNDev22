wait(game.Players.LocalPlayer.Character)
wait(1)
game.Players.LocalPlayer.Character:ScaleTo(5)
game.Players.LocalPlayer.Character.Humanoid.JumpHeight = 7.2
gui = Instance.new("ScreenGui")
framePrincipal = Instance.new("Frame")
cornerPrincipal = Instance.new("UICorner")
botaoAbrir = Instance.new("TextButton")
cornerSecundaria = Instance.new("UICorner")
HiVNIsHere = Instance.new("TextLabel")

wait(0.1)
--Frame
framePrincipal.Size = UDim2.new(0.95, 0, 0.95, 0)
framePrincipal.Position = UDim2.new(0.025, 0, 0, 0)
framePrincipal.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
cornerPrincipal.CornerRadius = UDim.new(0.04, 0)
framePrincipal.BackgroundTransparency = 0.1
framePrincipal.Name = "Frame Principal"
--Botão Abrir
botaoAbrir.Name = "Abre/Fecha"
botaoAbrir.Size = UDim2.new(0, 050, 0, 050)
botaoAbrir.Text = "VN"
botaoAbrir.TextColor3 = Color3.fromRGB(255, 255, 255)
cornerSecundaria.CornerRadius = UDim.new(0.2, 0)
botaoAbrir.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
botaoAbrir.Position = UDim2.new(0, 1550, 0, -30)
-- VN is here
HiVNIsHere.Parent = framePrincipal
HiVNIsHere.Name = "HiVNIsHere"
HiVNIsHere.Text = "Hi, the new VN HUB is here!"
HiVNIsHere.TextScaled = true
HiVNIsHere.Font = Enum.Font.FredokaOne
HiVNIsHere.BackgroundTransparency = 1
HiVNIsHere.TextColor3 = Color3.fromRGB(255, 255, 255)
HiVNIsHere.Size = UDim2.new(0, 1000,0, 70)
HiVNIsHere.Position = UDim2.new(0, 400,0, 0)
wait(1)
gui.Parent = game.Players.LocalPlayer.PlayerGui
gui.Name = "VN HUB"
framePrincipal.Visible = false
framePrincipal.Parent = gui
cornerPrincipal.Parent = framePrincipal
botaoAbrir.Parent = gui
cornerSecundaria.Parent = botaoAbrir

--Abrir e fechar
botaoAbrir.MouseButton1Click:Connect(function()
	framePrincipal.Visible = not framePrincipal.Visible
end)
