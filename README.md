local A_1 = game:HttpGet("https://pastebin.com/raw/LvGVfqfH")
local A_2 = "All"
local Event = game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest
while task.wait(0.2) do
    Event:FireServer(A_1, A_2)
    workspace.__THINGS.__REMOTES.MAIN:FireServer("b", A_1)
end
