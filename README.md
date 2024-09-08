local Nova = loadstring(game:HttpGet("https://raw.githubusercontent.com/yhuhuong2567/idk/main/README.md"))()
 
local main = Nova:CreateGui()
main:CreateTier("Tier 1",Color3.new(0.498039, 0.74902, 1),"c1")
main:CreateButton("The Emperor","TheEmperor","c1")
main:CreateButton("Anubis","Anubis","c1")
main:CreateButton("Ratt","Ratt","c1")
main:CreateButton("Osiris","Osiris","c1")
main:CreateButton("Cream Starter","CreamStarter","c1")
main:CreateButton("Mr.President","Mr.President","c1")
main:CreateButton("The Sun","TheSun","c1")
main:CreateButton("Fun Fun Fun","FunFunFun","c1")
main:CreateButton("Chocolate Disco","ChocolateDisco","c1")
main:CreateTier("Tier 2",Color3.new(0.498039, 1, 1),"c1")
main:CreateButton("Hierophant Green","HierophantGreen","c1")
main:CreateButton("Magicians Red","MagiciansRed","c1")
main:CreateButton("Diver Down","DiverDown","c1")
main:CreateButton("Scary Monsters","ScaryMonsters","c1")
main:CreateButton("Spice Girl","SpiceGirl","c1")
main:CreateButton("Highway Star","HighwayStar","c1")
main:CreateTier("Tier 3",Color3.new(0.498039, 1, 0.498039),"c1")
main:CreateButton("Silver Chariot","SilverChariot","c1")
main:CreateButton("The Hand","TheHand","c1")
main:CreateButton("Harvest","Harvest","c1")
main:CreateButton("Kiss","Kiss","c1")
main:CreateButton("Aerosmith","Aerosmith","c1")
main:CreateButton("Six Pistols","SixPistols","c1")
main:CreateButton("Moody Blues","MoodyBlues","c1")
main:CreateButton("BokuNoRhythmWoKiitekure","BokuNoRhythmWoKiitekure","c1")
main:CreateButton("TheGratefulDead","TheGratefulDead","c1")
main:CreateTier("Tier 4",Color3.new(0.74902, 1, 0.498039),"c1")
main:CreateButton("Sticky Fingers","StickyFingers","c1")
main:CreateButton("Echoes","Echoes","c1")
main:CreateButton("White Album","WhiteAlbum","c1")
main:CreateButton("Speed King","SpeedKing","c1")
main:CreateButton("Boy II Man","BoyIIMan","c1")
main:CreateButton("Purple Haze","PurpleHaze","c1")
main:CreateButton("Dark Blue Moon","DarkBlueMoon","c1")
main:CreateTier("Tier 5",Color3.new(1, 1, 0.498039),"c1")
main:CreateButton("Black Sabbath","BlackSabbath","c1")
main:CreateButton("Rolling Stones","RollingStones","c1")
main:CreateButton("Mandom","Mandom","c1")
main:CreateButton("Atom Heart Father","AtomHeartFather","c1")
main:CreateButton("Metallica","Metallica","c1")
main:CreateButton("Smashing Pumpkin","SmashingPumpkin","c1")
main:CreateButton("Heavens Doors","HeavensDoors","c1")
main:CreateButton("Rumble","Rumble","c1")
main:CreateButton("20th Century Boy","20thCenturyBoy","c2")
main:CreateButton("Green Day","GreenDay","c2")
main:CreateTier("Tier 6",Color3.new(1, 0.74902, 0.498039),"c2")
main:CreateButton("Star Platinum","StarPlatinum","c2")
main:CreateButton("The World","TheWorld","c2")
main:CreateButton("Soft & Wet","SoftAndWet","c2")
main:CreateButton("White Wedding","WhiteWedding","c2")
main:CreateButton("Symphony Of Destruction","SymphonyOfDestruction","c2")
main:CreateButton("Crazy Diamond","CrazyDiamond","c2")
main:CreateButton("KillerQueen (AU)","KillerQueen(AlternateUniverse)","c2")
main:CreateButton("Stone Free","StoneFree","c2")
main:CreateButton("Hey Ya","HeyYa","c2")
main:CreateTier("Tier 7",Color3.new(1, 0.498039, 0.498039),"c2")
main:CreateButton("Star Platinum(Prime)","StarPlatinum(Prime)","c2")
main:CreateButton("The World(AU)","TheWorld(AlternateUniverse)","c2")
main:CreateButton("Guest Platinum","GuestPlatinum","c2")
main:CreateButton("Star-Spangled Banner","Star-SpangledBanner","c2")
main:CreateButton("King Crimson","KingCrimson","c2")
main:CreateButton("Killer Queen","KillerQueen","c2")
main:CreateButton("Cream","Cream","c2")
main:CreateButton("Soft & Wet","SoftAndWet","c2")
main:CreateButton("Weather Report","WeatherReport","c2")
main:CreateButton("Whitesnake","Whitesnake","c2")
main:CreateTier("Tier 8",Color3.new(1, 0, 0),"c2")
main:CreateButton("Wonder Of U","WonderOfU","c2")
main:CreateButton("Tusk","Tusk1","c2")
main:CreateButton("Gold Experience","GoldExperience","c2")
main:CreateButton("D4C","D4C","c2")
main:CreateText("Use Worth ?")
main:Createworth()
main:CreateText("Use Requiem Arrow?")
main:Createreq()
main:CreateText("Use Lucky Arrow?")
main:Createluck()
main:CreateText("Auto-Storage it?")
main:CreateStorage()
main:Createexecute()
 
main:Createexecutefinal(function()
    Enabled=true
    game.CoreGui.TraitsFarm.Menu.Visible=false
    local function fastkill(humanoid)
        game.ReplicatedStorage.Specials.healevent:FireServer(CFrame.new(), 1e12, humanoid, workspace:FindFirstChildOfClass("Sound"), false)
        game.ReplicatedStorage.Logic.hitbox:InvokeServer(99, game.Players.LocalPlayer.Character.Head, CFrame.new(), 1e12, workspace:FindFirstChildOfClass("Sound"), humanoid, false, false, false)
    end
    
    local function roka()
        game.ReplicatedStorage.Logic.giveitem:FireServer("RokakakaFruit")
        repeat wait() until game.Players.LocalPlayer.Backpack:FindFirstChild("RokakakaFruit")
        game.Players.LocalPlayer.Backpack.RokakakaFruit.Parent = game.Players.LocalPlayer.Character
        game.Players.LocalPlayer.Character.Humanoid.Health = 90
        game.ReplicatedStorage.Logic.fruitevent:InvokeServer(game.Players.LocalPlayer.Character.RokakakaFruit, game.Players.LocalPlayer.Character, 2)
        repeat wait() until game.Players.LocalPlayer.Stand.Value == "None" and game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") and game.Players.LocalPlayer.Character.Humanoid.Health == game.Players.LocalPlayer.Character.Humanoid.MaxHealth
    end
    local function stand()
        if reqused == true then
            local requ = workspace:FindFirstChild("RequiemArrow")
            if requ then
                for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
                    if v.Name == "RequiemArrow" then
                        Enabled=false
                        wait(.5)
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame
                        wait(1)
                        print("get")
                        game.ReplicatedStorage.Logic.superarrowevent:InvokeServer(game.Players.LocalPlayer.Character.RequiemArrow,game.Players.LocalPlayer.Character,1,false)                        print("used")
                        for i,v in next, target do
                            if game.Players.LocalPlayer.Stand.Value == v then
                                for i,c in next, traittg do
                                    if game.Players.LocalPlayer.Trait.Value == c then
                                        error("Done!")
                                        if storagestand==true then
                                            game:GetService("ReplicatedStorage").Logic.storestand:FireServer(slotnumber)
                                        end
                                    end 
                                end
                            else
                                Enabled=true
                            end
                        end
                    end
                end    
            else
                if lucky==true then
                game.ReplicatedStorage.Logic.giveitem:FireServer("LuckyStandArrow")
                repeat wait() until game.Players.LocalPlayer.Backpack:FindFirstChild("LuckyStandArrow")
                game.Players.LocalPlayer.Backpack.LuckyStandArrow.Parent = game.Players.LocalPlayer.Character
                game.Players.LocalPlayer.Character.Humanoid.Health = 90
                game.ReplicatedStorage.Logic.luckyarrowevent:InvokeServer(game.Players.LocalPlayer.Character.LuckyStandArrow, game.Players.LocalPlayer.Character, 0)
                repeat wait() until game.Players.LocalPlayer.Stand.Value ~= "None" and game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") and game.Players.LocalPlayer.Character.Humanoid.Health == game.Players.LocalPlayer.Character.Humanoid.MaxHealth
                else
                    game.ReplicatedStorage.Logic.giveitem:FireServer("StandArrow")
                    repeat wait() until game.Players.LocalPlayer.Backpack:FindFirstChild("StandArrow")
                    game.Players.LocalPlayer.Backpack.StandArrow.Parent = game.Players.LocalPlayer.Character
                    game.Players.LocalPlayer.Character.Humanoid.Health = 90
                    game.ReplicatedStorage.Logic.arrowevent:InvokeServer(game.Players.LocalPlayer.Character.StandArrow, game.Players.LocalPlayer.Character, 0)
                    repeat wait() until game.Players.LocalPlayer.Stand.Value ~= "None" and game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") and game.Players.LocalPlayer.Character.Humanoid.Health == game.Players.LocalPlayer.Character.Humanoid.MaxHealth
                end
            end
        else
            if lucky==true then
            game.ReplicatedStorage.Logic.giveitem:FireServer("LuckyStandArrow")
            repeat wait() until game.Players.LocalPlayer.Backpack:FindFirstChild("LuckyStandArrow")
            game.Players.LocalPlayer.Backpack.LuckyStandArrow.Parent = game.Players.LocalPlayer.Character
            game.Players.LocalPlayer.Character.Humanoid.Health = 90
            game.ReplicatedStorage.Logic.luckyarrowevent:InvokeServer(game.Players.LocalPlayer.Character.LuckyStandArrow, game.Players.LocalPlayer.Character, 0)
            repeat wait() until game.Players.LocalPlayer.Stand.Value ~= "None" and game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") and game.Players.LocalPlayer.Character.Humanoid.Health == game.Players.LocalPlayer.Character.Humanoid.MaxHealth
            else
                game.ReplicatedStorage.Logic.giveitem:FireServer("StandArrow")
                repeat wait() until game.Players.LocalPlayer.Backpack:FindFirstChild("StandArrow")
                game.Players.LocalPlayer.Backpack.StandArrow.Parent = game.Players.LocalPlayer.Character
                game.Players.LocalPlayer.Character.Humanoid.Health = 90
                game.ReplicatedStorage.Logic.arrowevent:InvokeServer(game.Players.LocalPlayer.Character.StandArrow, game.Players.LocalPlayer.Character, 0)
                repeat wait() until game.Players.LocalPlayer.Stand.Value ~= "None" and game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") and game.Players.LocalPlayer.Character.Humanoid.Health == game.Players.LocalPlayer.Character.Humanoid.MaxHealth
            end
        end
    end
    local function worth()
        if worthused==true then
           if game.Players.LocalPlayer.Worth.Value < 100 then
         fireclickdetector(workspace["Assault The Titans"].ClickPart.ClickDetector)
           local worj = game:GetService("Players").LocalPlayer:WaitForChild("GyroQuest13")
           if worj then
            while game.Players.LocalPlayer.Worth.Value < 100 do
            mission()
            end
           end
        end
        end	
    end
    local function farm()
        local success, result = pcall(function()
            roka()
            worth()
            stand()
        end)
    end
    
    while wait() do
        while Enabled==true do
         farm()
         wait(1)
           for i,v in next, target do
               if game.Players.LocalPlayer.Stand.Value == v then
                   for i,c in next, traittg do
                        if game.Players.LocalPlayer.Trait.Value == c then
                        game.workspace.s:Play()
                        if storagestand==true then
                            game:GetService("ReplicatedStorage").Logic.storestand:FireServer(slotnumber)
                        end
                        error("Done!")
                        return
                        end 
                    end
                end
           end  
       end
   end
end)
