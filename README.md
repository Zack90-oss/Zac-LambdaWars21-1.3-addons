To install:

Download needed (.vpk) addon file
into
(path to steam library)SteamLibrary\steamapps\common\Lambda Wars\lambdawars\addons
(if "addons" folder do not exist, then create it)

REMEMBER TO CHECK ADDONS YOU'RE DOWNLOADING FOR ANY UNWANTED/MALICIOUS COMPONENTS BEFORE INSTALLING THEM

ChangeList.txts:

lw21_1.3_smarter_barreltraps_and_mortars.vpk:{
  Barrel Traps and Combine Mortars no longer will autocast strike right on themselves and generally make semi-smart decisions
}

lw21_1.3_rebel_vehicles.vpk:{
* ConVars
	rebel_vehicles_sv_enable_jeep 0
	rebel_vehicles_sv_enable_minivan 1
	Enables / Disables Jeep and/or minivan construction in junkyard
	Set them BEFORE starting a match

* Rebel team
	Restored unit_jeep:
		Created at Junkyard Building in 50 seconds
		75 Requisition, 75 Scrap
		4 Population
		500 health, 500 speed
		attributes['metal', 'large', 'tau']
		requires rebel tech centre

		Mounted tau gun with the same damage as one human troop is equiped with
		Turbo charge ability [Instant] (Speeds up the vehicle by 1.5 times for 5 seconds with 15 seconds cooldown)
		Tau charge ability (The same as the one used by human, but made so that it works with this thingy)
		
		Main differences from Tau Gun unit:
			Shares the same attack range with the Veteran unit.
			Has 300 more health and "metal" attribute.
			Is wayyyy faster.
			Can easily 1v1 a hunter if it's not attacking from blindspots.
			Less manuverable (check spelling).

		Balance:
			Well, this is almost a direct upgrade to tau gun unit but still serves whole another purpose as an artillery.
			Still is nuked by crab synth 1v1 and maybe 2v1???? (didn't check).
			Still is harrased by strider if in strider's cannon blast range.
			Absolutely nukes hunters and, if used correctly, kills striders (especially if in group).
			Harrased by light and medium units cause no damage bonus against them.

		"A fast-moving vehicle which needs driver(Well, that is a lie (it looked ugly, so I disabled this)) in order to move around and is equipped with long range Tau Gun.\nCan be used as an offensive weapon for taking sniper shots as well as defensive.\n\nMain purpose and difference from other units:\nAnti-synth and heavy artillery to support your CQB troops"
	
	Added unit_minivan:
		Created at Junkyard Building in 35 seconds
		50 Requisition, 30 Scrap
		4 Population
		400 health, 250 speed
		attributes['metal', 'large']
		requires rebel munitions depot (early game building, not the late game one)
		
		Balance:
			Kinda imbalanced, as it provides units such as veterans or combine snipers with the ability to shoot while moving.
			Have less damage resistance than bunker 0.65 mul against 0.35 mul inside bunker.
			Can be killed by hunter (2 bursts) if hunter haven't died already from 3 tau gunners / rpgs inside of the vehicle.
		
		"A Moving Castle.\nProvides 0.65 damage multiplier to units inside (less damage resistance than a bunker though).\nCombine with veterans or snipers to do some trolling (To be fixed)"
}
