---
layout: post
title: ADH purification using liters of culture
category: protein
---


## Grow cultures
* Day 1: Restreak -80oC stock onto an LB + Km plate
	* Strain 78: pET29b ALD 3K9D from Amanda.  Pink tube.  Always check description on the side of the tube, and use an unopened streaking tip tube for -80oC stocks. 
		* [-80oC stock spreadsheet](https://docs.google.com/spreadsheet/ccc?key=0AlVxrZi130nMdHlsaml2OGFDUW9zRlVBdkRKaXVEbkE#gid=11)

* Day 2: Prepare inoculum and liters of autoinduction media
	* Inoculate 1-5 colonies into an overnight flask with LB + Km 
	* Prepare autoinduction media: [recipe](https://docs.google.com/spreadsheets/d/1EM-sfk65Xf5F3q3316Yw_b5y0U5GasYQLF6Ug5sa7Y8/edit#gid=0)
		* Weigh ingredients into 2.8L flasks, add millipore DI H2O, cover with foil and autoclave tape, and autoclave. 
	* Weigh out Km to be dissolved and filter sterilized directly into flasks. 
		* 100mg per L of culture
* Day 3: Inoculate big flasks
	* Finish preparing autoinduction media:
		* ADD SUGAR MIX TO AUTOINDUCTION MEDIA. 40mL per liter of culture. 
		* Resuspend the Kanamycin and syring filer it into the flasks
		* Inoculate the flasks with ~10mL of overnight culture per liter of autoinduction media base
## Day before purification
* Finalize purification plans
	* Use [this spreadsheet](https://docs.google.com/spreadsheets/d/1oLDPxM6pbjul0TU0kZnZZwuXRpIY0xC7nsihhSPGGJ0/edit#gid=2074177923) as a guide.  All info should be entered in here upon completion. 
	* Previously used or new resin? 
	* Include controls like new resin done in parallel? 
* Prepare the large french press cell
	* Do rubber seals look good?
	* Wash it if you weren't the last one to use it. 
	* Move whole assembly to the walk-in fridge. 
	* E-mail the group to notify of french press plans if others are using it heavily recently.
* Prepare tubes: 
	* Prepare tubes for saving aliquots of the lysate, flow-through, and washes. 
	* Prepare tubes for the elutions
	* Pepare a tube for the water wash(es) and MES buffer wash(es)

## Centrifuge in the Sorvoll floor centrifuge
* Use the larger GS-3 rotor that holds 0.5L bottles. 
* Spin for ~10min pretty fast.  7,500 RPM = max speed.   
	* The centrifuge takes a while to slow down.
* Switch rotor to the SS-34 rotor for future use
* Pour extra culture (beyond what fits into the ultra) into 50mL tubes and consider pooling it.


## Collect cell pellets
* Goal: scrape all the pellets into a falcon tube, which can be vortexed to resuspend the cells.
	* Use a weighing scoop from the media room.
	* Don't try to resuspend bottle by bottle. Vortex after all the globs are in the falcon tube.  
* Try using only 20mL of resuspension buffer (50mM PO4 buffer + 0.3M NaCl) because the final volume in the falcon tube should be <=45mL to have a chance at effective vortexing.
* Use the buffer to rinse whatever cells are stuck to the tube after scraing. 
* Vortex aggressively.  Ideally there will be no clumbs loaded into the french press cell. 

## French press in the large french press cell
* French press parameters:
	* Load ~25mL.  This cell is too heavy to be filled upside down.  This means air on top of the sample is unavoidable.  In order to get the piston down enough to load onto the pressurizing machine, you can't have too much liquid volume.  
	* Don't go above 500 PSI until we learn more about our particular press and cell. 
* Get large french press cell from the cold room
* Do a test run with cold (ideally sterile) water
	* This ensures a final check that the seals are effective and lowers the stress level when processing the sample. 
* French press the sample
	* Use a new nylon bead in the valve that controls flow
	* Make sure outlet flow is closed before loading sample.  (Otherwise it will leak onto the floor.)
	* Load up to 30mL of the sample into the french press.  More might make it hard to get the plunger down enough to fit on the pressure stand. 
	* Pressurize to 500 PSI
	* Let the sample drip (ideally as few as a few drops per minute) into a Falcon tube
	* Repeat with the other half of the ADH sample
	* French press the samples agin.  
* DNAse can be added to reduce viscosity downstream
	* Currently we don't have any DNAse, but we do have some "lysonase" we can try. 

## Clairify lysates in the Sorvoll 
* Move the lysates into 2 SS-34 bottles
	* Balance by eyeball. 
* Centrifuge for 20+ minutes
	* This time has not been optimized yet.  

## Prepare resin
* Find a way to hold the column up
	* Tape the 50mL tube rack to something heavy.  Def want to tape so I won't knock it over and break the column's glass! 
* If the resin is new:
	* Load it into the blue column
	* Rinse it with >3 column volumes of the lysis buffer.  Repeat. 
* If the resin is old:
	* Note the date it was first used, and how many uses.  Update the identifying sticker. 
	* Wash off the 20% ethanol buffer it is stored in with 2 repeats of >3 column volumes of lysis buffer. 

## Load clairified lysate onto resin
* Put cap on the outlet of the column to stop flow.
* Filter resin through a 5uM filter if you see chunks when you pipette the clarified lysate up from the SS-34 centrifuge bottles
* Add the supernatant to the resin. 
* Put the caps on the top to prevent leaking
* Move the assembly to the fridge room and rock the resin for up to 30 minutes to bind the His-tagged protein
	* Make sure the resin is being sloshed and doesn't sit in one end of the column. 

## Wash loaded resin
* Retreive column from cold room rocker.
* Take off the top cap and make sure there isn't resin stuck up there
* Allow the lyate to flow through the column.  
	* Collect some of the flow-through for gel analysis.  Can keep it all if you think there is a chance you will capture more protein from the flow-through. 
* Wash resin
	* collect all the flow-through from each wash in a used tip tray.  Mix it up and save some for gel analysis after each wash is completed. 
	* typically up to 20mM imidazole is used in the washes.  
	* 10mM showed a lot of ADH washing of 150126
	* Try washing with NaCl PO4 (no imidazole), PO4 without NaCl or imidazole, and finally 10mM imidazole PO4. 

## Elute ADH from the resin
* Use 200mM imidazole to elute the protein
	* Can add 1.5 - 4mL at a time, depending on goals.
	* First 1.5mL had <10mM ADH in 150126 purification. 
* Put eluted fractions on ice. 

## Quantify uMs via NanoDrop A280 readings
* Take 3-6 NanoDrop A280 readings for each elution.  
	* Blank with water
	* Save file often because software tends to crash.
* Enter A280 values into [this spreadsheet](https://docs.google.com/spreadsheets/d/1oLDPxM6pbjul0TU0kZnZZwuXRpIY0xC7nsihhSPGGJ0/edit#gid=2074177923). 

## Clean resin for re-use
* Rinse the column with the MES NaCl buffer.  Use a few column volumes.
	* Save some of this for SDS-PAGE
* Rinse resin with a whole column of water.  Repeat.
	* consider saving some of these washes for SDS-PAGE

## Pool desirable elutions
* Decide what uM you want the final mix to be before pooling.
* Mix elutions you want to keep in a 15mL tube.  
* Re-measure A280
* Enter A280 values into [this spreadsheet](https://docs.google.com/spreadsheets/d/1oLDPxM6pbjul0TU0kZnZZwuXRpIY0xC7nsihhSPGGJ0/edit#gid=2074177923)
* Decide how many uL of frozen ADH you want in each eppendorf. 
* Label eppendorf tubes for freezing.  Put date and the fact that it is ADH on there. 

## Flash freeze and store at -80oC 
* Use liquid nitrogen to flash freeze the proteins. 

## End of day checklist:
* Make sure re-use of resin is noted if it is
* Centrifuge off, rotors in the fridge
* french press area clean; french press cell washed & returned to fridge. 

## Record notes
* [this spreadsheet](https://docs.google.com/spreadsheets/d/1oLDPxM6pbjul0TU0kZnZZwuXRpIY0xC7nsihhSPGGJ0/edit#gid=2074177923) will contain the parameters for all ADH batch purifications we do. 
	* Was yield as is expected? 
	* Is yield declining with resin re-use? 
	* Is it time to test regeneration of resin by Adam's protocol?

## Run SDS-PAGE
Recommended volumes: 

solution | typical volumes | comments | amt to load in SDS-PAGE
---------------|-------------
lysate | 20mL | Want to be able to vortex in a 50mL tube so try to keep final volume < 40mL by using < 20mL resuspension buffer | __uL of 20X diluted sample   
washes | 10mL | washing strips some ADH off of column so don't wash excessively | 10uL
elutions | 1.5mL - 4mL | chose smaller volumes if you want to get a few fractions with really high concentrations. | 8-16 uL*uM  
 

