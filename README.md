# ccw-price-hider
JS scripts for blocking pricing view on CCW

Before: <img width="1467" height="931" alt="image" src="https://github.com/user-attachments/assets/ed354f73-f00d-4c1a-94a2-6fb8f121809d" />

After: <img width="1493" height="791" alt="image" src="https://github.com/user-attachments/assets/e3b691b9-6550-4566-8d48-05c8c2f4edee" />

Before: <img width="1822" height="719" alt="image" src="https://github.com/user-attachments/assets/d9e0d4bf-7953-4e0b-baa8-72b59527a0fe" />

After: <img width="1817" height="715" alt="image" src="https://github.com/user-attachments/assets/72944567-488a-401a-8d20-7e3f920dc758" />

---

## How to Install the Cisco CCW Pricing Hider

This guide will help you install a small tool that automatically hides certain pricing and financial info sections on Cisco CCW estimate pages, making the view cleaner for you, when you're showing it to someone who doesn't care about the price info.

What you'll need:

*   Google Chrome web browser (or Firefox/Edge, instructions are similar)
*   About 5-10 minutes of your time

---

### Step 1: Install Tampermonkey

1.  Open Google Chrome.
2.  Click on the link to go to the Tampermonkey installation page:
    *   [Tampermonkey for Chrome](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
    *   [Tampermonkey for Firefox](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
    *   [Tampermonkey for Edge](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpbldcldlgbcefcobcblnpfmhg)
3.  On the Tampermonkey page, click the blue button that says "Add to Chrome" (or "Get" for Firefox/Edge).
4.  A window might pop up asking for confirmation. Click "Add extension".
5.  You should now see a new icon appear in the top-right corner of your browser, next to your address bar. It looks like a black square with two circles (like two eyes). This is the Tampermonkey icon.

---

### Step 2: Install the Pricing Hider Scripts

Now we'll add the specific code that does the hiding.

1.  Click on the Tampermonkey icon in the top-right of your browser.
2.  From the menu that appears, click on "Create a new script...".
3.  A new tab will open with a code editor. You will see some example code already there. DELETE ALL OF THIS EXAMPLE CODE and make sure the editor window is completely empty.
      Tip: Click anywhere in the code editor, then press `Ctrl+A` (on Windows) or `Cmd+A` (on Mac) to select everything, then press `Delete` or `Backspace`.
4.  Now, copy the script codes linked below. Make sure you copy ALL of it, from `// ==UserScript==` to the very end `})();`.

      * [CCW Price Hider - Main Estimate](https://github.com/pbritoferreira/ccw-price-hider/blob/main/ccw-price-hider-main) This will block pricing info on the main estimate page.
    
      * [CCW Price Hider - Item config](https://github.com/pbritoferreira/ccw-price-hider/blob/main/ccw-price-hider-item-config) This will block pricing info inside an item configuration.

6.  Paste the copied code into the empty Tampermonkey editor window.
      Tip: Click in the empty editor, then press `Ctrl+V` (on Windows) or `Cmd+V` (on Mac).
7.  Save the script.
    *   Go to "File" in the top menu of the editor.
    *   Click "Save". (Or simply press `Ctrl+S` on Windows / `Cmd+S` on Mac).
    *   You can now close this tab.
8.  Enable non-official scripts by right clicking the Tampermonkey extension on your browser, then "Manage extension". Find the "Allow userscripts" toggle and turn it on. Make sure to save or hit the back arrow to ensure the configuration is taken.

---

### Step 3: Use the Script on Cisco CCW

1.  Go to any Cisco CCW Estimate page (e.g., `https://apps.cisco.com/ccw/cpc/estimate/...`).
2.  You should immediately see the pricing-related columns and the "Financial Summary" section disappear!

    *   Uh oh... it hasn't disappeared...
        *   Try a "hard refresh": Press `Ctrl+F5` (on Windows) or `Cmd+Shift+R` (on Mac).
        *   Check the Tampermonkey icon in your browser's top-right corner. It should have a small red number on it (like `1` or `2`), indicating a script is active on the page. If it doesn't, click the icon and make sure "Enabled" is checked, and then go to "Dashboard" to ensure "Cisco CCW Pricing Hider" is turned on (green toggle).
        

---

### Step 4: How to Turn the Script Off/On (If needed)

1.  Click on the Tampermonkey icon in the top-right of your browser.
2.  Click on "Dashboard".
3.  You will see a list of your installed scripts. Find "Cisco CCW Pricing Hider" and "Cisco CCW Pricing Hider - Item config", and enable/disable both, as needed, by clocking the toggle next to it. Green for on (princing info will be blocked) and gray for off (pricing info will be shown)
4.  After changing the setting, go back to your Cisco CCW page and reload it (F5) for the change to take effect. Use normally.

---

This script only changes what you see on your screen; it doesn't affect the actual pricing data or CCW. It's a purely cosmetic and safe way to customize your CCW experience.  
 
