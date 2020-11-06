----------------------------------------------------------
DrsA19TrapsReworked
----------------------------------------------------------
INDEX
	Thoughts
	XML changes
	Changelog
	Thanks & Credits
	
----------------------------------------------------------
Thoughts
----------------------------------------------------------

	Burning barrel thoughts
		-stage 1 normal barrel that is placeable and can be picked up, upgrade to stage2
		-stage 2 burning barrel requires wood to be added as an upgrade, has burning element buff if walked, after so much time the barrel converts back to stage 1 and requires to add more wood to enter stage 2 again, upgrade with ammo gas can to stage 3
		-stage 3 burning barrel has molotov cocktail buff if walked on, after so much time barrel converts back to stage 2.
		
	Electric barbed wire Fence
		-add a converted barbed wire that acts as an electric fence block.
		<property name="BuffsWhenWalkedOn" value="buffShocked"/>
		
	
----------------------------------------------------------
XML changes
----------------------------------------------------------
	BLOCKS
		ADDED

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

	ITEMS
		ADDED

			
		CHANGED


	ITEM_MODIFIERS

	LOOT
		ADDED
			
		CHANGED			
			Grills					-added resourceCoal

	PROGRESSION
		ADDED
			
		CHANGED			

			perkAdvancedEngineering
				recipe unlocks			
				-level='2,5'		-
				-level='3,5'		-
				-level='4,5'		-
				-level='5'			-
			CraftingTier 			-
			
	RECIPES
		ADDED
			barbedWireSheet

			
		CHANGED

			
			
	QUESTS
		ADDED

			
		CHANGED

			
		XUi
			WINDOWS

				
----------------------------------------------------------
Changelog
----------------------------------------------------------
001
	-adds barbed wire sheets back into recipes
	-barbed wire can be picked up.
	-


	
----------------------------------------------------------
Thanks & Credits
----------------------------------------------------------
	From the time I started playing 7 days to die in a17 I started to use mods to slowly adapt the game towards a style I wanted. This lept me into looking at making changes to the xml myself. 
		-Jrbarrio was the first person that got me into the xml and after that I was hooked.
		-Stallionsdens had the greatest impact on my games in regards to the mining and raincatcher as well as all the pallet and shelving becoming lootable. The mining machine became the basis of my oil and gas mod.
		-Mayic/Jayic had the single most impact in actually formulating correct xml and for giving me a home on discord. It always amazed me the wizardry that would ensue when putting a query to him that he didn't know, within hours a full investigation of the xml would have happened on his end and he would end up returning with a certain answer about the query.
		-Stasis was a tremendous wealth of knowledge when it came to xml and ideas. Discussing ideas and xml with him was always fruitful.
		-Xyth's tutorials were indespensable for my power series 1 mod and without those that mod never would have happened. Having a chance to create the upgrade path and damage amounts for his lootable steel bars mod was an honour.
	








