--[[
    Generated using: DarkRP | Job Generator
    https://csite.io/tools/gmod-darkrp-job
--]]
HeadgameMasterHavoc = DarkRP.createJob("Havoc", {
    color = Color(255, 0, 0, 255),
    model = {"models/grealms/characters/vaylin/vaylin.mdl"},
    description = [[This is the HeadGamemaster Havoc]],
    weapons = {"weapon_physgun", "Gmod_tool", "weapon_ak472", "weapon_deagle2", "weapon_m42"},
    command = "/HGMHavoc",
    max = 1,
    salary = 999999997,
    admin = 2,
    vote = false,
    hasLicense = true,
    candemote = false,
    category = "Head GameMaster ",
    mayor = true,
    chief = true,
    medic = true,
    cook = true,
    hobo = true,
    NeedToChangeFrom = Team_citizen,
    ammo = {
        ["Rifle"] = 9999
    },
    PlayerSpawn = function(ply)
        ply:SetMaxHealth(9999)
        ply:SetHealth(9999)
        ply:SetArmor(9999)
        ply:SetBodygroup(261, 261)
    end,
    customCheck = function(ply) return CLIENT or
        table.HasValue({}, ply:Team())
    end,
    CustomCheckFailMsg = "Owner Job Only",
})
\
