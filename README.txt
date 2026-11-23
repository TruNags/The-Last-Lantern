THE LAST LANTERN - OWLBEAR RODEO EXTENSION
==========================================

Owlbear Rodeo extensions are loaded from a web address, so this folder has to
be hosted somewhere first. Then you give Owlbear the address of manifest.json.

1. HOST THE FOLDER (pick one, all free)
   - GitHub Pages: put the contents of this folder in a repository, then
     Settings > Pages > deploy from the main branch. Your manifest will be at
     https://YOURNAME.github.io/REPO/manifest.json
   - Netlify: drag this whole folder onto https://app.netlify.com/drop
     (the included _headers file adds the CORS header Owlbear needs).
   - Cloudflare Pages: same idea; _headers is honored there too.

   Whatever you use, the manifest must be reachable from other websites
   (the header "Access-Control-Allow-Origin: *"). GitHub Pages does this by
   default.

2. ADD IT TO OWLBEAR RODEO
   Open your Profile > Extensions > Add Extension, and paste the full URL of
   manifest.json.

3. USE IT
   A lantern icon appears in the left toolbar. Click it to open the roller.
   - "Order a Drink" rolls a random drink.
   - The dropdown + "Pour It" picks a specific drink.
   - Leave "Tell the rest of the table" ticked and everyone else in the room
     who has the extension added sees a short notification with the drink and
     its effect. Untick it to keep your roll private.

4. CUSTOMISE THE MENU PER ROOM
   Click "Edit this room's menu" in the popover.
   - Remove any default drink (and bring it back later with Restore).
   - Add your own drinks: a name, a description, and an effect (leave the
     effect blank for a drink with no effect).
   - Changes are saved to the Owlbear room itself, so everyone in that room
     sees the same menu live, and your other rooms are untouched.
   - By default only the GM can edit the menu. The GM can tick "Let players
     edit the menu too" at the bottom of the editor.
   - Room storage is limited, so custom drinks share a small budget (about
     12 KB, roughly 30 average-length drinks). The editor shows how much is
     used. Removing default drinks costs almost nothing.

NOTE: the notification only reaches players who also have the extension
installed (it runs a small background page for each of them).
