Tasker.Auto-Tether
==================
Automatic tethering via Bluetooth fro Android / Tasker.

## Requirements
* Tasker (Android App)
* Secure Settings (Tasker Plugin)
* Root Access (Helpful, not required)

## What does it DO?
The goal of this is to configure a Tablet (or other non-Cellular internet capable device) so that it will automaticall connect to and maintain a connection to a bluetooth capable device which shares its Internet connection such as a cell phone.

I designed this to automatically shut off when the device connects to a wireless hot spot of any kind.  Both the phone and the tablet will shut down bluetooth tethering if a hot spot is connected to.  If the bluetooth connection is dropped and no wifi connection was found, the Tablet sets itself up to scan for its pairing partner every so often.

I set this up to use bluetooth because WiFi is battery intensive and bluetooth is much more friendly in that respect.

### Restrictions
* Configured to only connect to one single device via Bluetooth.
* Most stock ROMs, even if rooted, require a device to check if the cellular account has a tethering option, so when your WiFi connecion drops in this situation, you might see a dialog or message pop up saying "Processing..." or "Checking for subscription status...".  This is normal, although annoying.  CyanogenMod doesn't have this problem and I suspect most ASOP based ROMs would not.  It is also possible to disable the check on some stock ROMs if you've got root access, but I don't deal with that here.
* Some modication may be required, as it is designed to work with my Check Internet tasks and profiles.

## Known Bugs
* If a phone tries to check for validation of a tethering subscription too soon, sometimes it stalls or just fails and has to be done again, if this happens consider added a "Wait" or "Wait For" action to the tethering task.
