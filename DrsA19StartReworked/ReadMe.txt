----------------------------------------------------------
DrsA19StartReworked
----------------------------------------------------------
INDEX
	Thoughts
	XML changes
	Changelog
	Thanks & Credits
	
----------------------------------------------------------
Thoughts
----------------------------------------------------------
	Loot boxes
		add to	
			Trader inventory
			relevant loot tables/containers
	Trader quest
		Base Building
			go to location with spawnchest containing blocks, bars, doors, hatches, ladders
			place blocks, bars, doors, hatches, ladders
			spawn zombies, defend area
			return to Trader
		Base Fine Tuning

	Need to add
		palletCompressedCardboard 
		balance loot boxes
			Instead of the Loot Box creating one of 2 different loot boxes as items, make it call to the loot tables instead.
		Tier1-6 quests need the appropriate loot box added.
	AUGER
		make the burning mod work again with auger
	Lights
		need to be scrappable

	
----------------------------------------------------------
XML changes
----------------------------------------------------------
	BLOCKS
		ADDED
			Drs_spawnTrader
			Drs_spawnTraderRekt
			Drs_spawnTraderHugh
			Drs_spawnTraderBob
			Drs_spawnTraderJen				-currently the reward for finding the trader so that a Trader can be placed at the base. will be attempting to make these traders more unique so they are independant from the vanilla traders in stock and quests if possible. At the very least I want the player to be able to choose which Trader they want.
			palletBrownBoxesBaseA
			palletBrownBoxesBaseB
			palletBrownBoxesBaseC
			palletBrownBoxesBaseLooted
			palletBrownBoxesTileA
			palletBrownBoxesTileB
			palletBrownBoxesTileC
			palletBrownBoxesTileLooted
			palletBrownBoxesTopA
			palletBrownBoxesTopB
			palletBrownBoxesTopC
			palletBrownBoxesTopLooted
			palletBrownBoxesLooseA
			palletBrownBoxesLooseB
			palletBrownBoxesLooseC
			palletBrownBoxesLooseLooted
			palletWhiteBagsBaseB
			palletWhiteBagsBaseC
			palletWhiteBagsTileA
			palletWhiteBagsTileeB
			palletWhiteBagsTileC
			palletWhiteBagsTopB
			palletWhiteBagsTopC
			palletWhiteBagsPartial1A
			palletWhiteBagsPartial1B
			palletWhiteBagsPartial1C
			palletWhiteBagsPartial2A
			palletWhiteBagsPartial2B
			palletWhiteBagsPartial2C
			palletWhiteBagsLooseA
			palletWhiteBagsLooseB
			palletWhiteBagsLooseC
			palletBlueTarpBaseA
			palletBlueTarpBaseB
			palletBlueTarpBaseC
			palletBlueTarpTileA
			palletBlueTarpTileB
			palletBlueTarpTileC
			palletBricksBaseA
			palletBricksBaseB
			palletBricksBaseC
			palletBricksTileA
			palletBricksTileB
			palletBricksTileC
			palletBricksTopA
			palletBricksTopB
			palletBricksTopC
			palletBricksPartial1A
			palletBricksPartial1B
			palletBricksPartial1C
			palletBricksPartial2A
			palletBricksPartial2B
			palletBricksPartial2C
			palletBricksLooseA
			palletBricksLooseB
			palletBricksLooseC
			barbedWireSheet01
			woodBarsCentered_Armoured
			woodBars_Armoured
			ironBarsCentered_Armoured
			ironBars_Armoured
			steelBarsCentered
			steelBars
			steelBarsCentered_Armoured
			steelBars_Armoured
			stainlessSteelBarsCentered
			stainlessSteelBars
			Oil_Extractor
			Oil_Loot_Here	
		CHANGED
			barbedWireSheet		-disassemble harvest into itself using the savage tool. - upgrades into barbedWireSheet01
			burningBarrel		-CanPickup turned on
			burningBarrelPlayer -added the buffBurningElement whith BuffsWhenWalkedOn
			woodBars			-added UpgradeBlock path.
			woodBarsCentered	-added UpgradeBlock path.
			ironBars			-added UpgradeBlock path.
			ironBarsCentered	-added UpgradeBlock path.
			Wild Plants 				-changed to class CropsGrown so they can be picked up with E
			Player Plants				-have to make the extends function exclude the class CropsGrown so they don't get picked up.

	BLOCKPLACEHOLDERS
		ADDED
			
		CHANGED
			Brown Boxes
				palletBrownBoxesBase
				palletBrownBoxesTile
				palletBrownBoxesTop
				palletBrownBoxesLoose
			White Bags
				palletWhiteBagsBase
				palletWhiteBagsTile
				palletWhiteBagsTop
				palletWhiteBagsPartial1
				palletWhiteBagsPartial2
				palletWhiteBagsLoose
			Blue Tarps
				palletBlueTarpBase
				palletBlueTarpTile
			Brick Piles
				palletBricksBase
				palletBricksTile
				palletBricksTop
				palletBricksPartial1
				palletBricksPartial2
				palletBricksLoose

	ITEMS
		ADDED
			DrsStarterKit
			DrsStarterClothes
			DrsStarterMaterials
			DrsTraderToolKit
			
			Paper_Milestone_Zombie_Kill_100
			Quest_Chit
			QuestChit1
			QuestChit5
			QuestChit10
			QuestChit50
			QuestChit100
			
			lootBoxTraderReward
			lootBoxTraderRewardB
			lootBoxTraderRewardC
			
			lootBoxConstructionA
			lootBoxConstructionB
			lootBoxConstructionC
			
			lootBoxAmmoA
			lootBoxAmmoB
			lootBoxAmmoC
			
			lootBoxMedicine
			lootBoxBlood
			
			lootBoxFood
			
			lootBox_A
			lootBox_B
			lootBox_C
			
			CementLootCrateA
			CementLootCrateB
			CementLootCrateC
			
			BlueTarpLootA
			BlueTarpLootB
			BlueTarpLootC
			
			palletBrickLootA
			palletBrickLootB
			palletBrickLootC
			
			WorkOrderQuestSchematic1
			WorkOrderQuestSchematic2
			WorkOrderQuestSchematic3
			WorkOrderQuestSchematic4
			
			MT1_Cobblestone
			MT2_Cobblestone
			MT3_Cobblestone
			MT4_Cobblestone
			
			MT1_ConcreteMix
			MT2_ConcreteMix
			MT3_ConcreteMix
			MT4_ConcreteMix
			
			MT1_Cement
			MT2_Cement
			MT3_Cement
			MT4_Cement
			
			MT1_resourceForgedIron
			MT2_resourceForgedIron
			MT3_resourceForgedIron
			MT4_resourceForgedIron
			
			MT1_resourceForgedSteel
			MT2_resourceForgedSteel
			MT3_resourceForgedSteel
			MT4_resourceForgedSteel
			
			MT1_FlagstoneBlock
			MT2_FlagstoneBlock
			MT3_FlagstoneBlock
			MT4_FlagstoneBlock
			
			MT1_rebarFrameBlock
			MT2_rebarFrameBlock
			MT3_rebarFrameBlock
			MT4_rebarFrameBlock
			
		CHANGED
			meleeToolPickT3Auger 		-modslot amounts changed to 3,4,5,6,7,8
			ModSlots					-all current items with ModSlots value of 1,1,2,2,3,4 changed to 1,2,3,4,5,6
	LOOT
		ADDED
			
		CHANGED			
			Grills					-added resourceCoal

	PROGRESSION
		ADDED
			
		CHANGED			
			max_level				-999
			skill_points_per_level	-2
			perkAdvancedEngineering
				toolBeaker			-level='2,5'
				Oil_Extractor		-level='3,5'
				solarCell,solarbank	-level='5'
			CraftingTier 			-all tiers can be crafted again
			
	RECIPES
		ADDED
			QuestChit1
			QuestChit5
			QuestChit10
			QuestChit50
			QuestChit100
			MT1_Cobblestone	
			MT2_Cobblestone
			MT3_Cobblestone
			MT4_Cobblestone
			MT1_ConcreteMix
			MT2_ConcreteMix
			MT3_ConcreteMix
			MT4_ConcreteMix
			MT1_Cement
			MT2_Cement
			MT3_Cement
			MT4_Cement
			MT1_resourceForgedIron
			MT2_resourceForgedIron
			MT3_resourceForgedIron
			MT4_resourceForgedIron
			MT1_resourceForgedSteel
			MT2_resourceForgedSteel
			MT3_resourceForgedSteel
			MT4_resourceForgedSteel
			MT1_FlagstoneBlock
			MT2_FlagstoneBlock
			MT3_FlagstoneBlock
			MT4_FlagstoneBlock
			MT1_rebarFrameBlock
			MT2_rebarFrameBlock
			MT3_rebarFrameBlock
			MT4_rebarFrameBlock
			WorkOrderQuestSchematic1
			WorkOrderQuestSchematic2
			WorkOrderQuestSchematic3
			WorkOrderQuestSchematic4
			barbedWireSheet
			Oil_Extractor
			toolBeaker
			solarCell
			solarbank
		
		CHANGED
			foodBaconAndEggs			-reduced meat cost
			foodBoiledMeat				-reduced meat cost
			foodCharredMeat				-reduced meat cost -removed need for cooking skill
			foodChiliDog				-reduced meat cost
			foodGrilledMeat				-reduced meat cost
			foodMeatStew				-reduced meat cost
			foodSteakAndPotato			-reduced meat cost
			foodEggBoiled				-removed need for cooking skill
			
			
	QUESTS
		ADDED
			100_Zombies_Killed			-cyclic quest that rewards with every 100 zombie kills and swtiches to 100_Zombies_Killed_
			100_Zombies_Killed_			-cyclic quest that rewards with every 100 zombie kills and swtiches to 100_Zombies_Killed
			Quest_Chit1					-reward when handing in 1 quest chit from the Zombie kill quests
			Quest_Chit5					-reward when handing in 5 quest chit from the Zombie kill quests
			Quest_Chit10				-reward when handing in 10 quest chit from the Zombie kill quests
			Quest_Chit50				-reward when handing in 50 quest chit from the Zombie kill quests
			Quest_Chit100				-reward when handing in 100 quest chit from the Zombie kill quests
			Drs_Reward_Loot
			Drs_Reward_LootB
			Drs_Reward_LootA
			loot_BaseConstructor_Box1
			loot_BaseConstructor_Box2
			loot_BaseConstructor_Box3
			loot_Killer_Box1
			loot_Killer_Box2
			loot_Killer_Box3
			loot_BoxA
			loot_BoxB
			loot_BoxC
			loot_FirstAid_Kit
			loot_BloodCase
			loot_Food_Box1
			quest_MaterialTrader1_Cobblestone
			quest_MaterialTrader2_Cobblestone
			quest_MaterialTrader3_Cobblestone
			quest_MaterialTrader4_Cobblestone
			quest_MaterialTrader1_ConcreteMix
			quest_MaterialTrader2_ConcreteMix
			quest_MaterialTrader3_ConcreteMix
			quest_MaterialTrader4_ConcreteMix
			quest_MaterialTrader1_Cement
			quest_MaterialTrader2_Cement
			quest_MaterialTrader3_Cement
			quest_MaterialTrader4_Cement
			quest_MaterialTrader1_resourceForgedIron
			quest_MaterialTrader2_resourceForgedIron
			quest_MaterialTrader3_resourceForgedIron
			quest_MaterialTrader4_resourceForgedIron
			quest_MaterialTrader1_resourceForgedSteel
			quest_MaterialTrader2_resourceForgedSteel
			quest_MaterialTrader3_resourceForgedSteel
			quest_MaterialTrader4_resourceForgedSteel
			quest_MaterialTrader1_FlagstoneBlock
			quest_MaterialTrader2_FlagstoneBlock
			quest_MaterialTrader3_FlagstoneBlock
			quest_MaterialTrader4_FlagstoneBlock
			quest_MaterialTrader1_rebarFrameBlock
			quest_MaterialTrader2_rebarFrameBlock
			quest_MaterialTrader3_rebarFrameBlock
			quest_MaterialTrader4_rebarFrameBlock
			BaseConstructor1
			BaseConstructor2
			BaseConstructor3
			BaseConstructor4
			BaseConstructor5
			BaseConstructor6
			BaseConstructor7
			BaseConstructor8
			
		CHANGED
			quest_BasicSurvival1		-removed and readded, removed objectives, auto completes, gives start gear.
			quest_BasicSurvival2		-removed and readded, replaces the quest_whiteRiverCitizen1 objectives
			quest_whiteRiverCitizen1	-removed and as note in quest_BasicSurvival2
			all quests containing @id with 'tier' in id name.	-adds lootBoxTraderReward as reward.
		
		XUi
			WINDOWS
				modslots				-possible to have 8 mod slots on items.
				
----------------------------------------------------------
Changelog
----------------------------------------------------------
003
	Added 
		contents of 
			DrsBarsOverhaul		-
			DrsA19OilNGas		-also locked recipe in progression perkAdvancedEngineering at level='3,5'
			DrsBurningBarrel	-
		recipes
			solar cell
			solarbank
			beaker
	Changed
		meat amount in relevant recipes from 5 to 2.
		charredmeat no longer needs cooking skill
		boiled eggs no longer needs cooking skill
		mod slots can now be up to 8 per item
		meleeToolPickT3Auger 		-modslot amounts changed to 3,4,5,6,7,8
		ModSlots					-all current items with ModSlots value of 1,1,2,2,3,4 changed to 1,2,3,4,5,6	
		Wild Plants can be picked up with E
		Crafting items now works for all tier levels.
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



	
----------------------------------------------------------
Thanks & Credits
----------------------------------------------------------
	From the time I started playing 7 days to die in a17 I started to use mods to slowly adapt the game towards a style I wanted. This lept me into looking at making changes to the xml myself. 
		-Jrbarrio was the first person that got me into the xml and after that I was hooked.
		-Stallionsdens had the greatest impact on my games in regards to the mining and raincatcher as well as all the pallet and shelving becoming lootable. The mining machine became the basis of my oil and gas mod.
		-Mayic/Jayic had the single most impact in actually formulating correct xml and for giving me a home on discord. It always amazed me the wizardry that would ensue when putting a query to him that he didn't know, within hours a full investigation of the xml would have happened on his end and he would end up returning with a certain answer about the query.
		-Stasis was a tremendous wealth of knowledge when it came to xml and ideas. Discussing ideas and xml with him was always fruitful.
		-Xyth's tutorials were indespensable for my power series 1 mod and without those that mod never would have happened. Having a chance to create the upgrade path and damage amounts for his lootable steel bars mod was an honour.
	








