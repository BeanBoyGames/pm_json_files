# pm_json_files
Top secret, please don't read.

Decision.json explination
{
  "ID": 3,
  "Title": "Collect Data from Users", 
  "Cost": 0.0,
  "Reputation": 0,
  "Description": "Get a $5M cash boost from selling users data to third party companies, This will also greatly increase the risk of a scandal.",
  "NewsArt": -1, // What news article to put out next round (-1 for no article)
  "Email": 2, // What email  to put out next round (-1 for no email)
  "Elms": 2, // How many stats will be effected 
  "Stats": [ "Money", "Scandal" ], // Stat effects (Must be in a array and length must be equal to "Elms")
  "Effects": [ 5.0, 50.0 ] // How strong the corrisponding stats will be changed
}

GameEvent.json explination
{
  "ID": 4,
  "Chance": 10, // Likely hood that it will succ (out of 100) || (likely hood of success) = ((base event chance) + (corresponding chance stat)) / 100  
  "ChanceStat": "CyberSec", // What stat to check against 
  "SpriteFail": "Cyber_Attack_Fail_Sprite", // Sprite path for a fail
  "SpriteSucc": "Cyber_Attack_Succ_Sprite", // Sprite path for a succ
  "TitleFail": "Cyber Attack Prevented", // Title for fail
  "TitleSucc": "Cyber Attack", // Title for succ
  "DescriptionFail": "Due to the hard workers in the Cyber Security devision, a hacking attempt was found before it was to late and taken care of. (+1 reputation)",
  "DescriptionSucc": "Due to the under-payed and under-staffed Cyber Security devision, a hostile body has taken an unknown amount of information. (-3 reputation)",
  "ElmsFail": 1, // How many elements will be effected on fail
  "StatsFail": [ "Rep" ], // Stat that will change on fail
  "EffectsFail": [ 1.0 ], // How much will the stat change on fail 
  "ElmsSucc": 1, // How many elements will be effected on succ
  "StatsSucc": [ "Rep" ], // Stat that will change on succ
  "EffectsSucc": [ -3.0 ]  // How much will the stat change on succ 
}

mech.json explination
{
  "ID": 0,
  "RenderTexturePath": "RenderTexture/CamRendSpider", // Just name in this convention
  "IconPath": "MechIcons/MechSpiderIcon", // Path
  "Title": "Spider",
  "Price": 1.8, // in Billions
  "BasePrice": 2.5, // How much you can sell for with no reputation or upgrades applied
  "Stats": [ 3, 2, 2, 2 ], // Original stats (0: stopping power, 1: struct-int, 2: style, 3: Utility )
  "UpgradeNames": [ "Name0", "Name1", "Name2" ], // Name of the upgrades 
  "UpgradeDescriptions": [ "Desc0", "Desc1", "Desc2" ], // Description of the upgrades 
  "UpgradePrices": [ 1.1, 2.2, 3.3 ], // Price of upgrades 
  "UpgradeSize0": 2, // How many stats does upgrade 0 change
  "UpgradeEffect0": [ 0, 2 ], // index of stats to change 
  "UpgradeAmount0": [ 3, -1 ], // what to change each stat by 
  "UpgradeSize1": 1,
  "UpgradeEffect1": [ 3 ],
  "UpgradeAmount1": [ 2 ],
  "UpgradeSize2": 4,
  "UpgradeEffect2": [ 0, 1, 2, 3 ],
  "UpgradeAmount2": [ 1, 1, 1, 1 ]
}
