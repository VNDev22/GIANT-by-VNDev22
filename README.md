wait(game.Players.LocalPlayer.Character)
gui = Instance.new("ScreenGui")
framePrincipal = Instance.new("Frame")
frameGeral = Instance.new("Frame")
cornerPrincipal = Instance.new("UICorner")
botaoAbrir = Instance.new("TextButton")
cornerSecundaria = Instance.new("UICorner")
HiVNIsHere = Instance.new("TextLabel")
VersionVN = Instance.new("TextLabel")
Welcome = Instance.new("TextLabel")
frameTudo = Instance.new("Frame")
homeButton = Instance.new("TextButton")
geralButton = Instance.new("TextButton")
teleportButton = Instance.new("TextButton")
giantButton = Instance.new("TextButton")
botaoFechar = Instance.new("TextButton")
definirTamanhoGigante = Instance.new("TextBox")
tamanhoGigante = Instance.new("NumberValue")
velocidadeButton = Instance.new("TextButton")
definirVelocidade = Instance.new("TextBox")
velocidadeValue = Instance.new("NumberValue")
wait(0.1)
--Frame
framePrincipal.Size = UDim2.new(0.95, 0, 0.95, 0)
framePrincipal.Position = UDim2.new(0.025, 0, 0, 0)
framePrincipal.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
framePrincipal.BackgroundTransparency = 0.1
framePrincipal.Name = "Frame Principal"
framePrincipal.Parent = frameTudo
cornerPrincipal.CornerRadius = UDim.new(0.04, 0)
cornerPrincipal.Parent = framePrincipal
--Frame tudo
frameTudo.Size = UDim2.new(1, 1, 1, 1)
frameTudo.Parent = gui
frameTudo.BackgroundTransparency = 1
frameTudo.Visible = false
--Botão Abrir
botaoAbrir.Name = "Abre"
botaoAbrir.Size = UDim2.new(0.045, 0,0.09, 0)
botaoAbrir.Text = "VN"
botaoAbrir.TextColor3 = Color3.fromRGB(255, 255, 255)
botaoAbrir.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
botaoAbrir.Position = UDim2.new(0.92, 0, 0.02, 0)
botaoAbrir.TextScaled = true
botaoAbrir.Parent = gui
botaoAbrir.Font = Enum.Font.FredokaOne
cornerSecundaria.CornerRadius = UDim.new(0.2, 0)
cornerSecundaria.Parent = botaoAbrir
-- VN is here
HiVNIsHere.Parent = framePrincipal
HiVNIsHere.Name = "HiVNIsHere"
HiVNIsHere.Text = "Hi, the new VN HUB is here!"
HiVNIsHere.TextScaled = true
HiVNIsHere.Font = Enum.Font.FredokaOne
HiVNIsHere.BackgroundTransparency = 1
HiVNIsHere.TextColor3 = Color3.fromRGB(255, 255, 255)
HiVNIsHere.Size = UDim2.new(0.631, 0,0.093, 0)
HiVNIsHere.Position = UDim2.new(0.252, 0,0, 0)
--VN Version
VersionVN.Parent = framePrincipal
VersionVN.Name = "VNVersion"
VersionVN.Text = "Version 0.1"
VersionVN.TextScaled = true
VersionVN.Font = Enum.Font.FredokaOne
VersionVN.BackgroundTransparency = 1
VersionVN.TextColor3 = Color3.fromRGB(255, 255, 255)
VersionVN.Size = UDim2.new(0.631, 0,0.093, 0)
VersionVN.Position = UDim2.new(0.252, 0,0.133, 0)
--Welcome
Welcome.Parent = framePrincipal
Welcome.Name = "Welcome"
Welcome.Text = "山乇ㄥ匚ㄖ爪乇"
Welcome.TextScaled = true
Welcome.BackgroundTransparency = 1
Welcome.TextColor3 = Color3.fromRGB(255, 255, 255)
Welcome.Size = UDim2.new(0.631, 0,0.093, 0)
Welcome.Position = UDim2.new(0.252, 0,0.266, 0)
--Botão home
homeButton.Name = "Home"
homeButton.Size = UDim2.new(0.12, 0,0.063, 0)
homeButton.Text = "Home"
homeButton.TextColor3 = Color3.fromRGB(255, 255, 255)
homeButton.BackgroundTransparency = 1
homeButton.Position = UDim2.new(0.035, 0,0.02, 0)
homeButton.TextScaled = true
homeButton.Parent = gui
homeButton.Visible = false
homeButton.Font = Enum.Font.Arcade
--Botão geral
geralButton.Name = "Geral"
geralButton.Size = UDim2.new(0.12, 0,0.063, 0)
geralButton.Text = "Geral"
geralButton.TextColor3 = Color3.fromRGB(255, 255, 255)
geralButton.BackgroundTransparency = 1
geralButton.Position = UDim2.new(0.035, 0,0.1, 0)
geralButton.TextScaled = true
geralButton.Parent = gui
geralButton.Visible = false
geralButton.Font = Enum.Font.Arcade
-- Botão de teleport
teleportButton.Name = "Teleport"
teleportButton.Size = UDim2.new(0.12, 0,0.063, 0)
teleportButton.Text = "Teleport"
teleportButton.TextColor3 = Color3.fromRGB(255, 255, 255)
teleportButton.BackgroundTransparency = 1
teleportButton.Position = UDim2.new(0.035, 0,0.18, 0)
teleportButton.TextScaled = true
teleportButton.Parent = gui
teleportButton.Visible = false
teleportButton.Font = Enum.Font.Arcade
--Frame geral
frameGeral.Size = UDim2.new(0.95, 0, 0.95, 0)
frameGeral.Position = UDim2.new(0.025, 0, 0, 0)
frameGeral.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
frameGeral.BackgroundTransparency = 0.1
frameGeral.Name = "Frame Geral"
frameGeral.Parent = frameTudo
frameGeral.Visible = false
cornerPrincipal:Clone().Parent = frameGeral
--Mudar tamanho button
giantButton.Name = "Mudar o tamanho"
giantButton.Size = UDim2.new(0.375, 0,0.141, 0)
giantButton.Text = "Mude seu tamanho"
giantButton.TextColor3 = Color3.fromRGB(255, 255, 255)
giantButton.BackgroundTransparency = 1
giantButton.Position = UDim2.new(0.281, 0,0, 0)
giantButton.TextScaled = true
giantButton.Parent = frameGeral
giantButton.Visible = true
giantButton.Font = Enum.Font.Arcade
--Botão fechar
botaoFechar.Name = "Fecha"
botaoFechar.Size = UDim2.new(0.045, 0,0.09, 0)
botaoFechar.Text = "X"
botaoFechar.TextColor3 = Color3.fromRGB(255, 255, 255)
botaoFechar.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
botaoFechar.Position = UDim2.new(0.92, 0, 0.02, 0)
botaoFechar.TextScaled = true
botaoFechar.Parent = gui
botaoFechar.Font = Enum.Font.FredokaOne
botaoFechar.Visible = false
cornerSecundaria.CornerRadius = UDim.new(0.2, 0)
cornerSecundaria.Parent = botaoAbrir
--Tamanho gigante
definirTamanhoGigante.Name = "Tamanho"
definirTamanhoGigante.Size = UDim2.new(0.094, 0,0.141, 0)
definirTamanhoGigante.Text = "Digite aqui o tamanho"
definirTamanhoGigante.TextColor3 = Color3.fromRGB(255, 255, 255)
definirTamanhoGigante.BackgroundTransparency = 1
definirTamanhoGigante.Position = UDim2.new(0.7, 0,0, 0)
definirTamanhoGigante.TextScaled = true
definirTamanhoGigante.Parent = frameGeral
definirTamanhoGigante.Font = Enum.Font.Arcade
--Mudar velocidade button
velocidadeButton.Name = "Mudar a velocidade"
velocidadeButton.Size = UDim2.new(0.375, 0,0.141, 0)
velocidadeButton.Text = "Mude sua velocidade"
velocidadeButton.TextColor3 = Color3.fromRGB(255, 255, 255)
velocidadeButton.BackgroundTransparency = 1
velocidadeButton.Position = UDim2.new(0.281, 0, 0.15, 0)
velocidadeButton.TextScaled = true
velocidadeButton.Parent = frameGeral
velocidadeButton.Visible = true
velocidadeButton.Font = Enum.Font.Arcade
--Velocidade
definirVelocidade.Name = "Velocidade"
definirVelocidade.Text = "Digite aqui a velocidade"
definirVelocidade.TextColor3 = Color3.fromRGB(255, 255, 255)
definirVelocidade.BackgroundTransparency = 1
definirVelocidade.Position = UDim2.new(0.7, 0, 0.15, 0)
definirVelocidade.TextScaled = true
definirVelocidade.Parent = frameGeral
definirVelocidade.Font = Enum.Font.Arcade
definirVelocidade.Size = UDim2.new(0.094, 0,0.141, 0)

wait(0.01)
gui.Parent = game.Players.LocalPlayer.PlayerGui
gui.Name = "VN HUB"



--Abrir e fechar
botaoAbrir.MouseButton1Click:Connect(function()
	frameTudo.Visible = true
	botaoFechar.Visible = true
	botaoAbrir.Visible = false
	homeButton.Visible = true
	geralButton.Visible = true
	teleportButton.Visible = true
end)
botaoFechar.MouseButton1Click:Connect(function()
	frameTudo.Visible = false
	botaoFechar.Visible = false
	botaoAbrir.Visible = false
	homeButton.Visible = false
	geralButton.Visible = false
	teleportButton.Visible = false
end)
homeButton.MouseButton1Click:Connect(function()
	framePrincipal.Visible = true
	frameGeral.Visible = false
end)
geralButton.MouseButton1Click:Connect(function()
	framePrincipal.Visible = false
	frameGeral.Visible = true
end)
giantButton.MouseButton1Click:Connect(function()
	tamanhoGigante.Value = definirTamanhoGigante.Text
	wait(0.001)
	game.Players.LocalPlayer.Character:ScaleTo(tamanhoGigante.Value)
	game.Players.LocalPlayer.Character.Humanoid.JumpHeight = 7.2
end)
velocidadeButton.MouseButton1Click:Connect(function()
	velocidadeValue.Value = definirVelocidade.Text
	wait(0.001)
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = velocidadeValue.Value
end)
