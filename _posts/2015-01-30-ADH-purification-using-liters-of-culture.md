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
		* 100mg per L of culture. Use 2mL/100mg weighed.  Make a little bit of excess(didn't have enough 3/10/2015). 
* Day 3: Inoculate big flasks
	* Finish preparing autoinduction media:
		* ADD SUGAR MIX TO AUTOINDUCTION MEDIA. 40mL per liter of culture. so 60mL/flask. 
		* Resuspend the Kanamycin and syring filer (0.22uM pore size) it into the flasks
		* Inoculate the flasks with ~15mL of overnight culture per liter of autoinduction media base.  (1/100 dilution)

## Day before purification
* Finalize purification plans
	* Use [this spreadsheet](https://docs.google.com/spreadsheets/d/1oLDPxM6pbjul0TU0kZnZZwuXRpIY0xC7nsihhSPGGJ0/edit#gid=2074177923) as a guide.  All info should be entered in here upon completion.
		* Use A280 --> uM conversions found here: [A280 --> uM conversion numbers](https://docs.google.com/spreadsheets/d/1wMYTvu2YntoR3f-yfBMaQvffDbppOh3cMIEnPt8FHBY/edit#gid=0) 
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
* Before spinning down everything, measure OD600 and take off a little aliquot for SDS-PAGE analysis/troubleshooting. 
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
	* Load up to 45mL of the sample into the french press.  More might make it hard to get the plunger down enough to fit on the pressure stand. 
		* If doing 45mL, the cell must be loaded upside down (piston in, bottom cap off). This requires substantial strength; we could have a stand made. 
	* Pressurize to 500 PSI
	* Let the sample drip (ideally as few as a few drops per minute) into a Falcon tube
<!---	* Repeat with the other half of the ADH sample -->
	* French press the samples agin.  
* DNAse can be added to reduce viscosity downstream
	* Currently we don't have any DNAse, but we do have some "lysonase" we can try. 

## Clairify lysates in the Sorvoll 
* Move the lysates into 2 SS-34 bottles
	* Balance by eyeball. 
* Centrifuge for 20+ minutes
	* This time has not been optimized yet.  

## Prepare resin
* Amount to purify:
	* This is still being tuned. 
	* **Add notes from 1st round**
	* 3L of autoinduced culture that was french pressed 2x failed to saturate 3mL of unused resin (6mL of slurry) 1/26/2015 JM 
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
	* 150126: I used a Millex-SV filter (info taped to pg 575) and it was very hard to push through the syringe.  I had the aparatus on the floor and was using my body weight.  Adam uses something a little bit wider on a sample treated with DNAse and has no flow problems. 
	* 150204: looking for wider diameter filters, but found none.  Asked VWR rep.  These filters are a few dollars each, so it might be cheaper to just add DNAse.  And then the flow-through step would happen much faster too. 
* Add the supernatant to the resin. 
* Put the caps on the top to prevent leaking
* Move the assembly to the fridge room and rock the resin for up to 30 minutes to bind the His-tagged protein
	* Make sure the resin is being sloshed and doesn't sit in one end of the column. 

## Wash loaded resin
* 2015/2 update: **10mM imidazole strips off ADH 3K9D significantly**.  Only do one wash at this concentration.  Test 5mM imidazole next.
	* [experiment notes](https://docs.google.com/document/d/17OYVWsVnC6aX0Kxfoia7YyDMZiUqvZTHGkiAZ90MAuQ/edit?usp=sharing) & [spreadsheet](https://docs.google.com/spreadsheets/d/1-z3U3QN12Qyb0_aAMQLHAI_rHCZkWilnr8UYWF22tAw/edit?usp=sharing) (note: they are embedded in another experiment!)
* Retreive column from cold room rocker.
* Take off the top cap and make sure there isn't resin stuck up there
* Allow the lyate to flow through the column.  
	* Collect some of the flow-through for gel analysis.  Can keep it all if you think there is a chance you will capture more protein from the flow-through. 
* Wash bound resin
	* collect all the flow-through from each wash in a used tip tray.  Mix it up and save some for gel analysis after each wash is completed. (Don't want to catch only first or last drips through column; need to homogenize for gel)
	* typically up to 20mM imidazole is used in the washes.  
	* 10mM showed a lot of ADH washing of 150126
	* Try washing with NaCl PO4 (no imidazole), PO4 without NaCl or imidazole, and finally 10mM imidazole PO4. 

## Elute ADH from the resin
* Use 200mM imidazole to elute the protein
	* Can add 1.5 - 4mL at a time, depending on goals.
	* First 1.5mL had <10mM ADH in 150126 purification. 
	* Got 2 high-yield 3mL batches 150310
* Put eluted fractions on ice. 

## Quantify uMs via NanoDrop A280 readings
* Take 3-6 NanoDrop A280 readings for each elution.  
	* Blank with water
	* Save file often because software tends to crash.
* Enter A280 values into [this spreadsheet](https://docs.google.com/spreadsheets/d/1oLDPxM6pbjul0TU0kZnZZwuXRpIY0xC7nsihhSPGGJ0/edit#gid=2074177923). 

## Clean resin for re-use
* Note: 2015/2 this worked well.  Re-used buffer worked great.
	* notes: [experiment notes](https://docs.google.com/document/d/17OYVWsVnC6aX0Kxfoia7YyDMZiUqvZTHGkiAZ90MAuQ/edit?usp=sharing) & [spreadsheet](https://docs.google.com/spreadsheets/d/1-z3U3QN12Qyb0_aAMQLHAI_rHCZkWilnr8UYWF22tAw/edit?usp=sharing) (note: they are embedded in another experiment!)

* Rinse the column with the MES NaCl buffer.  Use a few column volumes.
	* Use 14mL so you can drip it into a Falcon tube, vortex, and sample for SDS-PAGE. 
	* Save some of this for SDS-PAGE
* Rinse resin with a whole column of water.  Repeat.
	* consider saving some of these washes for SDS-PAGE
* Store in 20% EtOH, 80% DI water
	* Note: some protocols use sodium azide to prevent microbial growth.  Sodium azide is toxic and the Baker Lab (specifically Adam W.) doesn't use it so we aren't either. 

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
lysate | 20mL | Want to be able to vortex in a 50mL tube so try to keep final volume < 40mL by using < 20mL resuspension buffer | ~4uL of 20X diluted sample   
washes | 10mL | washing strips some ADH off of column so don't wash excessively | 10uL
elutions | 1.5mL - 4mL | chose smaller volumes if you want to get a few fractions with really high concentrations. | 8-16 uL*uM  

## Deposit results in the archive:
* [2015 ADH megabatch purification records](https://docs.google.com/spreadsheets/d/1oLDPxM6pbjul0TU0kZnZZwuXRpIY0xC7nsihhSPGGJ0/edit?usp=sharing) 
* [2015 SDS-PAGE archive - Protein Purifications](https://docs.google.com/document/d/1I9xvb7WwAv4btEJM00hS3RkJfiWSESyACu6yhzmHhf8/edit) 

## Buffer Summary

solution       |composition                         | uses
---------------|------------------------------------|-------------
"basic" PO4    | 50mM NaCl PO4, ~pH 7.4		    | used to make most buffers, can be used to wash resin
PO4 + NaCl     |  50mM NaCl PO4, ~pH 7.4 + 0.3M NaCl| lysis, potentially 1st wash
salty wash     | "PO4 + NaCl" buffer + 10mM imidazole | wash resin
UNsalty wash   | "basic PO4" buffer + 10mM imidazole| wash resin
elution buffer |"basic PO4" buffer + 200mM imidazole| elute washed protein from resin
MES buffer     | MES (Sigma M2933) 20mM + 0.3M NaCl.  Can include sodium azide but doesn't for now* |washing resin
20% EtOH, unbuffered | 20% (v/v) ethanol in water | storing H2O and MES washed resin 

\* sodium azide can prevent "critters" from growing on stored resin, but is explosive and toxic.  The lethal dose for an adult human is only ~ 0.7 grams!  Adam W. from the Baker lab omits it from his buffer.  The 20% ethanol should be an effective inhibitor for short term storage. 



