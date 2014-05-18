Tasker.Auto-Tether
==================

Automatic tethering for Tasker

The goal of this is to configure a Tablet (or other non-Cellular internet capable device) so that it will automaticall connect to and maintain a connection to a bluetooth capable device which shares its Internet connection such as a cell phone.

I designed this to automatically shut off when the device connects to a wireless hot spot of any kind.  Both the phone and the tablet will shut down bluetooth tethering if a hot spot is connected to.  If the bluetooth connection is dropped and no wifi connection was found, the Tablet sets itself up to scan for its pairing partner every so often.

I set this up to use bluetooth because WiFi is battery intensive and bluetooth is much more friendly in that respect.

Retrictions:
1)  Configured to only connect to one single device via Bluetooth.
2)  Most stock ROMs, even if rooted, require a device to check if the cellular account has a tethering option, so when your WiFi connecion drops in this situation, you might see a dialog or message pop up saying "Processing..." or "Checking for subscription status...".  This is normal, although annoying.  CyanogenMod doesn't have this problem and I suspect most ASOP based ROMs would not.  It is also possible to disable the check on some stock ROMs if you've got root access, but I don't deal with that here.
