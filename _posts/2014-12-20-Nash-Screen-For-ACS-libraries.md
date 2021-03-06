---
layout: post
title: ACS Library Screening with Nash Reagent
category: enzyme_assays
---

## Things that can be done at "waiting steps":
* Prepare labeled plates:
  * assay plates: non-UV 1/2 area plates.  Label non-UV on the left skinny side, and label the date and description on the front wide side.
* add data from the plate reader software to the gSpreadsheet.  
  * Include a title like 141220 plate4 because the R script will parse out the plate number and use it to match to the well description. 
* label calculated uM values on ADH tubes for later freezing.  

## Have ready:
* Purified ADH.
  * Takes a while to thaw from -80oC
  * 150204 idea: move right amount to -20oC the previous night so it goes faster in the AM
* Fully grown-out autoinduced ACS enzyme variants with controls present on the plate.
  * Include a diagonal stripe of the + control ACS L641P, and some P641L and K609A controls elsewhere 
  * Was selective antibiotic included? 
* Plenty of NADH, ATP, CoA (keep an eye for stock running anywhere near low).
* Assay buffer.  Record date of prep in notebook & spreadsheet.
  * currently using 50mM PO4 buffer, pH ~7.4 

## Weigh chemicals
* Keep buffer at room temp; want enzyme reaction to happen at RT. 
* Use spreadsheet to calculate amount of each ingredient to weigh out.
* Prepare eppendorf tubes for cofactors: NADH, CoA, Mg++.  Name & date on top. 
  * Don't put these empty tubes on ice or they will attract water precipitation.  
* Label a 15mL tub for formate: date, formate, concentration, 
* Item locations:
  * NADH, ATP, CoA: -20oC freezer closest to Amanda's bench.  NADH & CoA are in a plastic baggie at the very bottom, in the cl
ear bin.  ATP is in a bigger bottle a few shelves up, and is shared with Amanda. 
  * formate is in the Na (sodium bin), and MgCl2 is in the M bin.  
* Put temperature sensitive reagents on ice.  (NADH, ATP, CoA)
* Weigh on most precise balance, being careful not to get water on the tubes (will effect measurement)
  * CoA is expensive ($231/100mg bottle); don't get much more than is required. NADH is medium-expensive, so don't go crazy with that either. 
  * Watch out for static.
* Record weights measured on tube, in notebook, and in spreadsheet.
* Add the appropriate amount of buffer based on spreadsheet calculations.   
* Make sure we don't run out of reagents:
  * keep an eye on CoA reserves.  If you open the last bottle, order 2-3 more.
  * If the NADH bottle gets low, order another.  (We don't use this one as fast, so we don't need to keep an unopened bottle around.)

## Move the following items to the plate reader
* a 50mL tube with some assay buffer 
* all the electronic and non-electronic pipettes (in a bucket)
* pneumatic pipette
* stopwatch
* BugBuster
* purified ADH
* lab notebook
* leave the ACS cells on the shaker so they don't settle.
* Nash reagent.  Ideally keep on ice in a dark bucket.  Make sure it isn't "to yellow".  Record prep date. 
* falcon tube holder (for buffer & formate stock)
* headphones
* timer

## Prepare the plate reader (only if doing TCA precip & scanning spectrum)
* Establish a connection between the computer & plate reader.  May require restarting the computer. 
* Make or copy an old PDA file into a new folder with the expriment date
  * set spectra to scan from 350nm to 550nm with step size of 2nm
* Note that when you save the PDA files, do save as and change the filename a little bit.  This is because saving is WAY slower than save as.  Eg.  filename--v5.pda is saved as filename--v6.pda
* Naming of the scan is crucial: the name is parsed by the R file, and the plate name is crucial for matching data to the descriptive well information in a different spreadsheet.  

## Screening a whole plate:
* Label plates
  * Plate = 1/2-area polystyrene (non-UV). 
  * Put the date on the A1-H1 side of the plate.  Write non-UV if plate is polystyrene. 
* Pipette autoinduced cells into 96-well plate.  
  * Do at bench with flame and cheap non-filtered but sterile tips. 
  * Make sure source cells just came off the shaker so they will not have settled out of solution. 
  * Eyeball that each tip does in fact have 4uL of cell suspension.  (Loose fitting pipette tips don't suck up liquid).
  * Put cells at the bottom of the wells so they will be sure to be in the reaction. 
* Make a master mix of ADH (7uM final), NADH (6mM final), CoA (1mM final), ATP (4mM final), Mg2+ (5mM final), and formate (700+mM final) according to gSpreadsheet
  * Make sure:
    * the uM of the ADH stock represents what you are going to use (different batches have different final uM values)
    * the number of plates is set correctly (usually 4)
    * you are making an appopriate amount of formate
  * Excess factor should be ~1.2
    * 1.1 is definitely not enough 141215 JM. 1.2x was too much 150204. 1.15 was too little 150409. Settle for 1.18
  
## -OR-Current recipe when NOT using a master mix:
Current recipe as of 141220:
* 4uL of autoinduced ACS cells
* 2uL of 10X BugBuster (fairly arbitrary given the rxn volume is 40uL)
* 3uL of NADH (3uL of 80mM in 40 uL --> 6mM)
* 3uL of ATP/CoA/Mg2+ mix, which includes:
  * stock concentrations: 15.15 mM CoA, 75.72 mM MgCl2, 60.6mM ATP
  * final concentrations: 1mM CoA, 5mM MgCl2, 4mM ATP.  
* _X_uL of purified ADH.  Want ~7uM for 4uL of autoinduced ACS cell extract. 

## Make a stock right before prepping a plate:
* Use a rinsed (DI water) or new pipette boat to mix in.  
* Make excess of the mix.  ~20% extra is appropriate.
* Load ACS cells first, using sterile technique at the bench

## Start the formaldehyde producing reaction
* First make *sure* the plate reader file is ready: 
  * Scan from ~350 to 500 nm, with 2 nm steps.  Scanning a whole plate this way takes ~10 minutes!
    * Can use less steps if it is a less important read. 
* Decide how long the reaction will be run.  Include this in the file name. 
  * Assume 15 minutes for now.  
    * 10 min not enough JM 150129 <-- ?? 
  * 7 minutes has been used since 2/4/2014 for 1/2 mL autoinduced cultures
  * May need to change the time as the autoinduction media recipe and culture volume changes. 
* Start reaction by adding 40-x uL of the reaction cocktail that includes formate, ATP, CoA, Mg++, purified ADH, BugBuster, and make-up buffer. 
  * **37uL if 4uL of cells per well**
    * Set pipette to 4*36uL dispensing.  Don't want "soapy" solution sucked into the pipette itself. 
  * Move tips & waste close together so loading time is quick and wells have comparable reaction times. 
  * ** Use new tips for each pipetting up** because BugBuster makes sucking bubbles into the pipette likely.
* Put a cover on the plate to help prevent formaldehyde evaporation (this may not actually help; to be tested).
* Start a timer when the first plate's loading is complete.  

## Add Nash reagent 
* Usually an equal volume of Nash reagent is added.  The reaction essentially(?) stops when the Nash reagent is added.  
* Move plate to 55oC or 61oC box for color development. ~30 minutes is appropriate. 
  * Note the temperature of the box in a notebook.  
* Remove plate to scan spectrum.

## If you want to scan the plate to plot the data, TCA precipitation is necessary
* **See safety notes below**
* This removes flecks of precipitated protein
* Add 40uL to a 40uL rxn with 40uL Nash? 
  * LOOK UP OLD DATA! 
* Centrifugation is necessary to push down particulates. 

## Copy data into electronic spreadsheet/notebook
* Export data from .pda to a text file. 
  * Select the plate reads you want to include.  You can only do within one experiment at a time
  * Verify that the assay plate number is included in the file names
  * Save to same folder as the PDA files, or a sub-folder
  * Open .txt files with Vim, and copy to the google spreadsheet. 
* Optional: go through plate and assign approximate yellowness values to each well.
  * 2 = comparable to average + control yellowness
  * 1 = less yellow than control
  * 3 = noticeably more yellow than + control. 


## Archive cells
* Record in lab notebook
* Restreak on an LB plate with the appropriate antibiotic.  
  * Are you restreaking for single colonies or just putting blobs on agarose? 
  * For single colonies, store up to 5 strains on a plate. 
  * Can squeeze 20+ on a plate if you just want blobs. 
* Put cell-filled 96-well plates in the fridge with aluminum seals. 

## Deposit summary here:
* [2015 Nash ACS assay screening records summary](https://docs.google.com/spreadsheets/d/1LfRP2Cc1TUjtHdHLKXzJmNh5pnyUYxsQ0h3w_pG4NQI/edit?usp=sharing): A spreadsheet that summarises our library screening efforts. 
*  Add any investigations done here: [2014_10_31 Nash Assay tests for HTS - SUMMARY of findings](https://docs.google.com/document/d/1jzvRbE3xuGehs7rV7GfHlY1QQp6DXSYDmVM4dGbo5B4/edit?usp=sharing)
  * Mostly about whole-cell scans, but if you do tests such as the ratio of ACS:ADH required, record it. 

## Clean up 
* Charge electronic pipettes that are low in battery.
* Make sure the plate shaker is turned off.
* Return pipettes to appropriate places
* Discard used 96-well plates.  

## Trichloroacetic Acid Safety ##
* **Trichloroacetic acid is a strong acid that will burn your skin and eyes very badly.**
  * In 2/2015 Janet got a tiny bit (smaller than a "drop") on her arm and it left a brown spot where it burned.  
* Proper handling:
  * gloves and closed-toe, skin-covering shoes are mandatory
  * goggles and a lab coat are encouraged. 
  * do not wear shoes that fail to protect your feet (e.g. mary jane shoes or sandals) 
* If you do get some on you, wash it off immediately.
  * It probably won't cause cancer, but will definitely leave a mark. 
* See the [EPA notes[(http://www.epa.gov/iris/toxreviews/0655tr.pdf) about toxicology to better understand the health hazards. 
