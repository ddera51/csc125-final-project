I am making a program that helps automotive service advisors quickly create quotes using menu item pricing. The prices and descriptions for various services are stored in dictionaries. Then multiple loops are used in order to build a quote while querying the dictionaries to create a very aimple quote.

Then create a dictionary called "prices" that stores the menu prices of the different services (op codes)

    Q1000= 119.95
    SYNWORKS= 129.95
    RWORKS= 329.95
    67=279.95
    D210= 239.95
    EVM=69.95 
    ROTATE= 24.95 
    MSI=35.00 
    MSIC= 169.99 
    AF= 59.95 
    CF= 89.95 
    FCCF=194.95 
    COOL=199.99 
    TF=309.95 
    FDS=229.95 
    RDS=229.95 
    TCS= 229.95 
    DECARB1=249.95 
    MOA=25.00 
    CF5=25.00 
    BALANCE= 100.00 
    MBT1= 24.95
    MBT2=49.90
    MBT3=74.85
    MBT4=99.80
    FBR=215.00  
    RBR=215.00  
    BFLUSH=179.95 
    SP4=194.95  
    SP6=294.95  
    SP8=394.95  
    BULB= 24.95  
    PATS= 99.98  
    PSF= 79.95  
    MUDFLAPS= 99.98  
    TONNEAU=199.95  
    EPR =69.95

Create a second dictionary called help with the descriptions of each service

    Q1000=WORKS (OIL CHANGE & TIRE ROTAION)  
    SYN-WORKS=FULL SYNTHETIC WORKS  
    RWORKS=FULL SYNTHETIC WORKS FOR SUPERCHARGED ENGINE  
    67=DIESEL WORKS (INCLUDES DEF TOP OFF)  
    D210=DIESEL FUEL FILTER  
    EVM=EV SERVICE  
    ROTATE=TIRE ROTATION  
    MSI=MASS STATE INSPECTION 
    MSIC=COMMERCIAL MASS STATE INSPECTION  
    AF=ENGINE AIR FITLER  
    CF=CABIN AIR FILTER  
    FCCF=CABIN AIR FILTER WITH FRIGI CLEANING SERVICE  
    COOL=COOLANT FLUSH  
    TF=TRANSMSSION FLUSH  
    FDS=FRONT DIFF SERVICE  
    RDS=REAR DIFF SERVICE  
    TCS= TRANSFERCASE SERVICE  
    DECARB1=DECARB SERVICE  
    MOA=BG OIL ADDITIVE  
    CF5=BG FUEL ADDITIVE  
    BALANCE=BALANCE ALL 4 TIRE  
    MBT1=MOUNT AND BALANCE 1 TIRES
    MBT2=MOUNT AND BALANCE 2 TIRES  
    MBT3=MOUNT AND BALANCE 3 TIRES  
    MBT4=MOUNT AND BALANCE 4 TIRES  
    FBR=FRONT BRAKE PADS AND ROTORS  
    RBR=REAR BRAKE PADS AND ROTORS  
    BFLUSH=BRAKE FLUSH  
    SP4=4 SPARK PLUGS  
    SP6=6 SPARK PLUGS  
    SP8=8 SPARK PLUGS  
    BULB=BULB REPLACEMENT  
    PATS=CUT AND PROGRAM KEY  
    WIPERS=FRONT WIPER BLADE REPLACEMENT   
    WIPER=REAR WIPER BLADE REPLACEMENT  
    WIPER3= ALL 3 WIPER BLADE REPLACEMENT  
    STP=SET TIRE PRESSURE  
    PSF=POWER SREERING FLUSH  
    MUDFLAPS= INSTALL MUD FLAPS  
    TONNEAU=INSTALL TONNEAU COVER  
    EPR=CRANKCASE CLEANING
    
create an empty list and call it "quote"
create an empty list and call it "description"
creare an variable (float) called "total"
set total equal to 0
Have the user input the Repair order number and save it as a string called "ro"

Loop
    user inputs op code, help, or close
    strip and capitalize user input
    if user enters close, end the loop
    if user enters help, print the "help" dictionary
    if user enters op code, add item to "quote" and print complete
    else print, "Try Again"

new loop
    for each item in quote
    Lookup each item in prices and add it to total
    return total

new loop 
  for each item in quote
    Lookup each item in help and add it to description
    return description
Print Quote Number # (ro)
Print total with $ and two decimal places
Print descriprion of services on the bottom

    
