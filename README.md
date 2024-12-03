local function RunSampleScript1()
    while Script1Toggled do
        local args = {
    [1] = 100,
    [2] = true
}

game:GetService("ReplicatedStorage"):WaitForChild("events"):WaitForChild("reelfinished"):FireServer(unpack(args))

        print("Script 1 is running...")
        wait(1)
    end
end

-- Function to stop the sample script
local function StopSampleScript1()
    print("Script 1 has stopped.")
end
