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
* Fully grown-out autoinduced ACS enzyme variants with controls present on the plate.
  * Include a diagonal stripe of the + control ACS L641P, and some P641L and K609A controls elsewhere 
  * Was selective antibiotic included? 
* Plenty of NADH, ATP, CoA (keep an eye for stock running anywhere near low).
* Assay buffer.  Record date of prep in notebook & spreadsheet.
  * currently using 50mM PO4 buffer, pH ~7.4 

## Weigh chemicals
* Use spreadsheet to calculate amount of each ingredient to weigh out.
* Prepare eppendorf tubes for cofactors: NADH, CoA, Mg++.  Name & date on top.  
* Label a 15mL tub for formate: date, formate, concentration, 
* Item locations:
  * NADH, ATP, CoA: -20oC freezer closest to Amanda's bench.  NADH & CoA are in a plastic baggie at the very bottom, in the clear bin.  ATP is in a bigger bottle a few shelves up, and is shared with Amanda. 
* Put temperature sensitive reagents on ice
* Weigh on most precise balance, being careful not to get water on the tubes (will effect measurement)
  * CoA is expensive ($231/100mg bottle); don't get much more than is required. NADH is medium-expensive, so don't go crazy with that either. 
* Record weights measured on tube, in notebook, and in spreadsheet.  

## Move the following items to the plate reader
* a 50mL tube with some assay buffer 
* all the electronic and non-electronic pipettes
* BugBuster
* purified ADH
* lab notebook
* headphones
* leave the ACS cells on the shaker so they don't settle.
* Nash reagent.  Ideally keep on ice in a dark bucket.  Make sure it isn't "to yellow"

## Prepare the plate reader
* Establish a connection between the computer & plate reader.  May require restarting the computer. 
* Make or copy an old PDA file into a new folder with the expriment date
* Note that when you save the PDA files, do save as and change the filename a little bit.  This is because saving is WAY slower than save as.  Eg.  filename--v5.pda is saved as filename--v6.pda
* Naming of the scan is crucial: the name is parsed by the R file, and the plate name is crucial for matching data to the descriptive well information in a different spreadsheet.  

## Current recipe:
Current recipe as of 141220:
* 2uL of autoinduced ACS cells
* 2uL of 10X BugBuster (fairly arbitrary given the rxn volume is 40uL)
* 3uL of NADH (3uL of 80mM in 40 uL --> 6mM)
* 3uL of ATP/CoA/Mg2+ mix, which includes:
  * stock concentrations: 15.15 mM CoA, 75.72 mM MgCl2, 60.6mM ATP
  * final concentrations: 1mM CoA, 5mM MgCl2, 4mM ATP.  
* __uL of purified NADH.  Want ~__uM for 2uL of autoinduced ACS cell extract. 

## Make a stock right before prepping a plate:
* Use a rinsed (DI water) or new pipette boat to mix in.  
* Make excess of the mix.  ~20% extra is appropriate.
* Load ACS cells first, using sterile technique at the bench

## Start the formaldehyde producing reaction
* First make *sure* the plate reader file is ready: 
  * Scan from ~350 to 500 nm, with 2 nm steps.  Scanning a whole plate this way takes ~10 minutes!
    * Can use less steps if it is a less important read. 
  * 
* Decide how long the reaction will be run.  Include this in the file name. 
* Start reaction by adding 40-x uL of the reaction cocktail that includes formate, ATP, CoA, Mg++, purified ADH, BugBuster, and make-up buffer. 
* Put a cover on the plate to help prevent formaldehyde evaporation (this may not actually help; to be tested)

## Add Nash reagent 
* Usually an equal volume of Nash reagent is added.  The reaction essentially(?) stops when the Nash reagent is added.  
* Move plate to 55oC or 61oC box for color development. 
* Remove plate to scan spectrum.

## If you want to plot the data, TCA precipitation is necessary
* This removes flecks of precipitated protein

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
  * Store up to 5 strains on a plate. 
* 


<div class="message">
Screening enzymes is so cool!
</div>

* Image test:
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")


     _____________
    < I love milk >
     -------------
            \   ^__^
             \  (oo)\_______
                (__)\       )\/\
                    ||----w |
                    ||     ||


