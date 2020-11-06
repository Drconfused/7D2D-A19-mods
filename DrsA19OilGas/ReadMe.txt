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

		
	
----------------------------------------------------------
XML changes
----------------------------------------------------------
	BLOCKS
		ADDED
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

	ITEMS
		ADDED

			
		CHANGED

	LOOT
		ADDED
			
		CHANGED			


	PROGRESSION
		ADDED
			
		CHANGED			
			perkAdvancedEngineering
				recipe unlocks			
				-level='2,5'			
				-level='3,5'		-Oil_Extractor
				-level='4,5'		-
				-level='5'			-
			
	RECIPES
		ADDED
			Oil_Extractor
			
		CHANGED
			
			
	QUESTS
		ADDED

			
		CHANGED

			

----------------------------------------------------------
Changelog
----------------------------------------------------------
		
001
	- adds a craftable block that will produce burning barrels on top of itself after so much time and will contain oil and gas related items.


	
----------------------------------------------------------
Thanks & Credits
----------------------------------------------------------
	From the time I started playing 7 days to die in a17 I started to use mods to slowly adapt the game towards a style I wanted. This lept me into looking at making changes to the xml myself. 
		-Jrbarrio was the first person that got me into the xml and after that I was hooked.
		-Stallionsdens had the greatest impact on my games in regards to the mining and raincatcher as well as all the pallet and shelving becoming lootable. The mining machine became the basis of my oil and gas mod.
		-Mayic/Jayic had the single most impact in actually formulating correct xml and for giving me a home on discord. It always amazed me the wizardry that would ensue when putting a query to him that he didn't know, within hours a full investigation of the xml would have happened on his end and he would end up returning with a certain answer about the query.
		-Stasis was a tremendous wealth of knowledge when it came to xml and ideas. Discussing ideas and xml with him was always fruitful.
		-Xyth's tutorials were indespensable for my power series 1 mod and without those that mod never would have happened. Having a chance to create the upgrade path and damage amounts for his lootable steel bars mod was an honour.
	








