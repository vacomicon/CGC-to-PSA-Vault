# CGC-to-PSA-Vault
A chrome extension to quickly pull data from a CGC graded Pokémon for shipment to the PSA vault.

I wrote this extension to help with the laborious task of entering in CGC graded Pokémon card details into the PSA vault system. CGC is a 3rd party grading company, and the PSA Vault is a physical repository to store your already-graded cards, or market them to other collectors on ebay using the PSA Vault interface.

First unzip the extension, and in Chrome, go to Settings - > Extensions - > "Load Unpacked" and choose the root directory of the extension to load.

If you click the exension in the toolbar, you are asked one query: "Set Cost for each card". This helps you measure profit. For me, it is about $15 a card, which is the cost of me shipping it to CGC, getting it graded, and then returned to me. If you wish to set this cost for each card in your submission, click the checkbox, otherwise you can leave it blank, or enter each card's cost manually on the PSA page later.

To use this extension, you will need TWO windows open in Chrome: The CGC Cert lookup page at https://www.cgccards.com/certlookup/ and your personal PSA vault page located at https://app.collectors.com/collection.

When you enter your 10 digit CGC graded card number (found on the back of your graded card), at https://www.cgccards.com/certlookup/ CGC will show you the details of your card.

On this screen, right click your mouse, and choose "Copy Card Info from CGC site", or click the hotkey CTRL-SHIFT-1. you will see a response on the screen that the data has been copied.

Next, move over to your second window, showing https://app.collectors.com/collection. Click "Add Item"
Next choose "My card doesn't have a PSA Grade" in the "search by card name" field, you can right click in the field, and there is a new drop down listed called "Card Data Selector" choose "Insert Card Name" from the sub-menu (you can automate this step by pressing "CTRL-SHIFT-2") This will help you find the corresponding card (watch our for the wrong language, or variants). This part requires a small amount of manual intervention to select the right card. DO NOT JUST CHOOSE THE FIRST CARD LISTED, as it may not alsways be your exact card!

On the next screen, click the very first field and choose "Insert Cert Nunber" (or use the hotkey CTRL-SHIFT-3). After inserting the card nuber, click the SAME FIELD, and choose "Fill CGC details." (or use the Hotkey CTRL-SHIFT-4). Note: You cannot fill the CGC details until AFTER you have entered a cert number. 

Tips for time saving:

Hotkeys have been assigned to each of these 4 functions:
CTRL-SHIFT-1: Copy Card info from CGC site (this can only be done from the CGC window, not the PSA window)
CTRL-SHIFT-2: Insert Card Name (this can only be done from the PSA window) 
CTRL-SHIFT-3: Insert Cert Number (this can only be done from the PSA window)
CTRL-SHIFT-4: Insert CGC Details (this can only be done from the PSA window)

My eyesight is going, and reading those tiny numbers on the back of a card is impossible. Thankfully, I can use a cheap QR scanner to do the work for me!
I use a HANDHELD USB QR scanner with a stand to automatically get the 9 digit code from the back of the card. You can get practically any "2D" barcode canner (so it can do QR codes). Presently these are about $30-35 on Amazon for the scanner plus the stand ("gun" style). VERY IMPORANT 2 steps: I had to "program" the QR gun (using barcodes in the included instructions) to 1) set for "automatic scanning" so all I had to do was stick the cards under the QR gun, and 2)  to ignore 1-D barcodes (Those series of lines) and only read in the QR code. Sadly, each little manual I read calls these 1-D barcodes something a little different, and i cannot offer any tech support for this. Remember: 1-D barcodes are are series of little lines, while 2-D barcodes are a pattern in a square. 

The reason for this is because the barcode on the back of a CGC card will give you a 26 digit result, not the 10 digit result you desire. The embedded QR information on the back of the card actually provides an internal URL for CGC, but CGC's "cert lookup" field will strip all of the unnecessary data, and only insert the desired 10 digit code.



