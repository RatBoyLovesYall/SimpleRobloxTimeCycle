--Add into local script in  ServerScriptService

local lighting = game.Lighting
local delayTime = 1

function timeChange()
	local minutes = 0

	while true do

		minutes += 1

		local minutesInAday = minutes % (60 * 24)
		local hours = minutesInAday / 60

		lighting.ClockTime = hours

		wait(1)

	end
end

timeChange()
