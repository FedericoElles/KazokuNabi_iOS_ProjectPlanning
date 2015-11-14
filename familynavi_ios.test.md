TEST FamilyNavi iOS

# Smoke Test
PREREQ Internet & Location available
- Install app
> App icon looks nice
- Open App
> Splash Screen displayed
- Functionality
> App opens, location is displayed
> Buttons clickable
> Google Maps displayed
> Links open in Safari
> Phonenumbers open Dialer
- Test special features
> Contact form works
> Back button works
> Home button available and works if appropriate
- Go on a walk
> After approx. 10m there is a "Location updated" hint
- Open a list of POIs
> The calc. distance changes as you walk
- Close app
- Reopen app and walk
> Location updates are still valid

# Offline mode
PREREQ Disabled Internet
- Force close and reopen app
> App works as in Smoke Test
> Locations is found and displayed as coordinates
> No error message
- Try to load a map
> Not displayed, no error
- Try to open a link
> Safari opens and displays offline hint

# No Location - Fix
PREREQ Disabled Internet
- Force close and reopen app
> App opens, hint that location must be enabled
- Click OK
> You are taken to the application settings
- Enable location settings
- Go back to app
> No error, location is found

# No location - No fix
PREREQ Disabled Location
- Force close and reopen app
> App opens, hint that location must be enabled
- Click abort
> You can click on offline mode
- App works, but without distances calculated

# No location - Offline mode
PREREQ Disabled Location
- Force close and reopen app
- Do not go to location settings
> App works, no errors
> No distances are calculated



