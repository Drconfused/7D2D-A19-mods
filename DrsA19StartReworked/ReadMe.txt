DrsA19StartReworked
Need to add
	palletCompressedCardboard 
	balance loot boxes
		Instead of the Loot Box creating one of 2 different loot boxes as items, make it call to the loot tables instead.
	Tier1-6 quests need the appropriate loot box added.
	
Thoughts
	Add loot boxes to Trader inventory.
	Trader quest
		Base Building
			go to location with spawnchest containing blocks, bars, doors, hatches, ladders
			place blocks, bars, doors, hatches, ladders
			spawn zombies, defend area
			return to Trader

----------------------------------------------------------
002
	Rebalanced Trader Loot Boxes
		added Mixed Loot table in loot.xml
	Adding Ammo loot boxes as a variant for cardboard box loot so it's not only construction loot.
		Loot Box A
			<item name="lootBoxConstructionA"/>			
			<item name="lootBoxAmmoA"/>
		
		Loot Box B
			<item name="lootBoxConstructionB"/>			
			<item name="lootBoxAmmoB"/>
		
		Loot Box C
			<item name="lootBoxConstructionC"/>			
			<item name="lootBoxAmmoC"/>
	Rebalanced the pallet loot boxes so it wasn't so drasticly a monty haul.	
		
001
	Blocks
		BarbedWireSheet 
			- attempting to make it disassemble into itself. Using the wrench or similiar.
			- upgrade into a reinforced barbed wire
		
	Recipes
		BarbedWireSheet


	-Start with more gear.
		Items on enter game
			gunPistol,
			medicalFirstAidBandage,
			DrsStarterKit:
				ammoGasCan				x1000
				ammo9mmBulletBall		x500
				medicalFirstAidBandage	x10
				meleeToolTorch			x2
				foodCanChili			x5
				drinkJarBoiledWater 	x5
				modGunScopeSmall		x1
				modMeleeSerratedBlade	x1
				vehicleBicyclePlaceable	x1
			DrsStarterClothes:
				apparelFlannelShirt		x1
				armorLeatherPants		x1
				apparelOveralls			x1
				armorLeatherGloves		x1
				armorLeatherBoots		x1
			DrsStarterMaterials:
				resourceForgedIron		x100
				resourceIronFragment	x500
				resourceWood			x500
				resourceRockSmall		x500
				resourceClayLump		x500
			Quest1 auto complete	
				quest_BasicSurvival2
				100_Zombies_Killed
				SkillPoints				x2
				casinoCoin				x1000

	-Removes the start quests and hops you right to having to locate the Trader.
		Rewards for finding Trader
			Exp							x1000
			SkillPoints					x2
			burningBarrelPlayer			x1
			DrsTraderToolKit			x1
				meleeToolRepairT1ClawHammer,
				meleeToolPickT1IronPickaxe,
				meleeToolAxeT1IronFireaxe,
				meleeToolWrench,
				ammoGasCan				x1000
			Drs_spawnTraderJen			x1
			DrsStarterMaterials			x1
			vehicleMinibikePlaceable
	 
	-Milestone quest system for killing zombies, after 100 zombie kills player obtains a quest chit that can be crafted into a package that activates a turn in quest to a trader for a reward. *see Zombie Slaughter 100 milestone quest
		Zombie Slaughter 100 milestone quest added to the start auto complete quest as a reward. 
			-100_Zombies_Killed and 100_Zombies_Killed_ are the quest names, they cycle one to the other and back in an endless cycle.
			-For every 100 zombies killed player gains a Quest Chit which can be crafted into a package that starts a Trader quest that rewards you for killing zombies by the hundreds.
				Quest_Chit1
					Exp						x1000
					lootBoxTraderReward		x1
					lootBoxAmmoC			x1
					
				Quest_Chit5
					Exp						x5000
					lootBoxTraderReward		x5
					lootBoxAmmoC			x5
					lootBoxAmmoB			x1
					
				Quest_Chit10
					Exp						x10000
					SkillPoints				x1
					lootBoxTraderReward		x10
					lootBoxAmmoC			x5
					lootBoxAmmoB			x5
					lootBoxAmmoA			x1
					lootBoxFood				x1
					
				Quest_Chit50
					Exp						x50000
					SkillPoints				x5
					lootBoxTraderReward		x10
					lootBoxAmmoA			x5
					lootBoxFood				x5
					
				Quest_Chit100
					Exp						x100000
					SkillPoints				10
					lootBoxTraderReward		x10
					lootBoxAmmoA			x10
					lootBoxFood				x10
	

	-CONSTRUCTION LOOT SYSTEM
		- 3 qualities of construction loot boxes A,B,C
			- following categories in the loot.xml added:
				Materials, Doors Hatches, Furniture and Decorations, Bars, Blocks, Traps, Tools, Electric Construction	
		-Cardboard boxes, white bag pallets, blue tarp pallets, bricks on pallets are all changed to a looting system.
			-Cardboard boxes come in 3 types A,B,C and have a random amount of items within. This rely's on the quest system to work.
			-white bag pallets come in 3 types A,B,C and have a set amount ingredients within.
				CementLootCrateA
					Concrete Mix 				x900
				CementLootCrateB
					Concrete Mix				x600
					Cement						x100
					Crushed Sand				x100
					Rocks						x100
				CementLootCrateC
					Cement						x300
					Crushed Sand				x300
					Rocks						x300
			-Blue Tarp pallets come in 3 types A,B,C and have a set amount ingredients within.
				BlueTarpLootA
					resourceCobblestones		x900
				BlueTarpLootB
					resourceCobblestones		x600
					resourceClayLump			x150
					resourceRockSmall			x150
				BlueTarpLootC
					resourceClayLump			x350
					resourceRockSmall			x350
			-Brick pallets come in 3 types A,B,C and have a set amount ingredients within.
				palletBrickLootA
					pouredConcreteBlockVariantHelper	x100
				palletBrickLootB
					brickBlockVariantHelper				x100
				palletBrickLootC
					flagstoneBlockVariantHelper			x100

	-AMMO LOOT
		- 3 qualities A,B,C 

	-MEDICINE LOOT
		-loot_FirstAid_Kit
			added categories into the loot.xml
				questMedicDrugs = only drug related items in here
				questMedicItems = beakers, candles, cooling mesh, insulated liner, health survival related perk books
				questMedicHollistic = hollistic items related to health survival, also can roll to the questmedicitems table
				questBandageCast = medical bandages/kit, splints, cast.
				questMedicKit = main category for loot_FirstAid_Kit which rolls from each table above, only guarantee is from the bandage/cast list.
		-loot_BloodCase
			case of medical blood - blood would have been a hot item, but as people were turned to zombies they very well would have dropped their blood kits without even knowing the blood was in there as they lost their capacity to think properly.


	-BASE CONSTRUCTOR
		-BC1
			workbench
			trader reward loot
			construction loot
			work order quest schematic



			-meleeToolRepairT3Nailgun,
			-meleeToolAuger,
			-meleeToolChainsaw,






















WISHLIST	
		









