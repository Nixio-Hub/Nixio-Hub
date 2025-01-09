local Nixio = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local Home = Instance.new("Frame")
local Settings = Instance.new("Frame")
local Scripts = Instance.new("Frame")
local Colors = Instance.new("Frame")
local UIPageLayout = Instance.new("UIPageLayout")
local HomeTitle = Instance.new("TextLabel")
local AddScriptButton = Instance.new("TextButton")
local ScriptList = Instance.new("ScrollingFrame")
local UIScrollView = Instance.new("UIScrollView")
local UIGridLayout = Instance.new("UIGridLayout")
local ScriptButton = Instance.new("TextButton")
local SettingsTitle = Instance.new("TextLabel")
local ComingSoonLabel = Instance.new("TextLabel")
local ScriptsTitle = Instance.new("TextLabel")
local CloseButton = Instance.new("TextButton")
local DeviceSelection = Instance.new("Frame")
local PCButton = Instance.new("TextButton")
local MobileButton = Instance.new("TextButton")
local iOSButton = Instance.new("TextButton")
local ColorsTitle = Instance.new("TextLabel")
local ColorPalette = Instance.new("ScrollingFrame")
local ColorButton = Instance.new("TextButton")
local ColorsScrollView = Instance.new("UIScrollView")
local ColorsGridLayout = Instance.new("UIGridLayout")
local FlyButton = Instance.new("TextButton")

-- Nixio Properties
Nixio.Name = "Nixio"
Nixio.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

-- Main Properties
Main.Name = "Main"
Main.Parent = Nixio
Main.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Main.BorderSizePixel = 0
Main.Position = UDim2.new(0.5, -250, 0.5, -250)
Main.Size = UDim2.new(0, 500, 0, 500)
Main.Visible = false -- Initially hidden

-- UIPageLayout Properties
UIPageLayout.Parent = Main
UIPageLayout.SortOrder = "LayoutOrder"

-- Home Properties
Home.Name = "Home"
Home.Parent = Main
Home.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Home.BorderSizePixel = 0
Home.LayoutOrder = 1

-- HomeTitle Properties
HomeTitle.Name = "HomeTitle"
HomeTitle.Parent = Home
HomeTitle.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
HomeTitle.BorderSizePixel = 0
HomeTitle.Position = UDim2.new(0, 10, 0, 10)
HomeTitle.Size = UDim2.new(0, 150, 0, 30)
HomeTitle.Font = Enum.Font.SourceSansSemibold
HomeTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
HomeTitle.Text = "Home"
HomeTitle.TextSize = 14

-- AddScriptButton Properties
AddScriptButton.Name = "AddScriptButton"
AddScriptButton.Parent = Home
AddScriptButton.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
AddScriptButton.BorderSizePixel = 0
AddScriptButton.Position = UDim2.new(0.5, -75, 0.3, 0)
AddScriptButton.Size = UDim2.new(0, 150, 0, 30)
AddScriptButton.Font = Enum.Font.SourceSansSemibold
AddScriptButton.TextColor3 = Color3.fromRGB(255, 255, 255)
AddScriptButton.Text = "Add Script"

-- ScriptList Properties
ScriptList.Name = "ScriptList"
ScriptList.Parent = Home
ScriptList.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
ScriptList.BorderSizePixel = 0
ScriptList.Position = UDim2.new(0.1, 0, 0.4, 0)
ScriptList.Size = UDim2.new(0.8, 0, 0.5, 0)
ScriptList.CanvasSize = UDim2.new(0, 0, 1, 0)

-- UIScrollView Properties
UIScrollView.Parent = ScriptList
UIScrollView.CanvasSize = ScriptList.CanvasSize

-- UIGridLayout Properties
UIGridLayout.Parent = UIScrollView
UIGridLayout.CellSize = UDim2.new(0, 150, 0, 30)
UIGridLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
UIGridLayout.VerticalAlignment = Enum.VerticalAlignment.Center

-- ScriptButton Properties
ScriptButton.Name = "ScriptButton"
ScriptButton.Parent = UIGridLayout
ScriptButton.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
ScriptButton.BorderSizePixel = 0
ScriptButton.Size = UDim2.new(0, 150, 0, 30)
ScriptButton.Font = Enum.Font.SourceSansSemibold
ScriptButton.TextColor3 = Color3.fromRGB(255, 255, 255)

-- Settings Properties
Settings.Name = "Settings"
Settings.Parent = Main
Settings.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Settings.BorderSizePixel = 0
Settings.LayoutOrder = 2

-- SettingsTitle Properties
SettingsTitle.Name = "SettingsTitle"
SettingsTitle.Parent = Settings
SettingsTitle.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
SettingsTitle.BorderSizePixel = 0
SettingsTitle.Position = UDim2.new(0, 10, 0, 10)
SettingsTitle.Size = UDim2.new(0, 150, 0, 30)
SettingsTitle.Font = Enum.Font.SourceSansSemibold
SettingsTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
SettingsTitle.Text = "Settings"

-- ComingSoonLabel Properties
ComingSoonLabel.Name = "ComingSoonLabel"
ComingSoonLabel.Parent = Settings
ComingSoonLabel.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
ComingSoonLabel.BorderSizePixel = 0
ComingSoonLabel.Position = UDim2.new(0.3, 0, 0.5, 0)
ComingSoonLabel.Size = UDim2.new(0, 200, 0, 30)
ComingSoonLabel.Font = Enum.Font.SourceSansSemibold
ComingSoonLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
ComingSoonLabel.Text = "Coming Soon!"

-- Scripts Properties
Scripts.Name = "Scripts"
Scripts.Parent = Main
Scripts.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Scripts.BorderSizePixel = 0
Scripts.LayoutOrder = 3

-- ScriptsTitle Properties
ScriptsTitle.Name = "ScriptsTitle"
ScriptsTitle.Parent = Scripts
ScriptsTitle.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
ScriptsTitle.BorderSizePixel = 0
ScriptsTitle.Position = UDim2.new(0, 10, 0, 10)
ScriptsTitle.Size = UDim2.new(0, 150, 0, 30)
ScriptsTitle.Font = Enum.Font.SourceSansSemibold
ScriptsTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
ScriptsTitle.Text = "Scripts"

-- CloseButton Properties
CloseButton.Name = "CloseButton"
CloseButton.Parent = Main
CloseButton.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
CloseButton.BorderSizePixel = 0
CloseButton.Position = UDim2.new(0.9, 0, 0.05, 0)
CloseButton.Size = UDim2.new(0, 20, 0, 20)
CloseButton.Text = "X"
CloseButton.TextColor3 = Color3.fromRGB(255, 255, 255)

-- DeviceSelection Properties
DeviceSelection.Name = "DeviceSelection"
DeviceSelection.Parent = Main
DeviceSelection.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
DeviceSelection.BorderSizePixel = 0
DeviceSelection.Position = UDim2.new(0.
