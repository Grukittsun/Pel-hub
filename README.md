local A = loadstring(game:HttpGet(("https://raw.githubusercontent.com/Grukittsun/Reuo-hub/main/README.md"),true))()

        function CheckingGame1()
        
            getgenv().Get =
                setmetatable(
                {},
                {
                    __index = function(A, B)
                        return game:GetService(B)
                    end
                }
            )
            
            for i, v in pairs(Games) do
                if i == game.PlaceId then
                    loadstring(game:HttpGet(v))()
                end
            end
        end
        CheckingGame1()
