# Infotainment

I was originally planning on trying to make an F150 unit work, assuming the fit might not be perfect and CAN functions might be messed up, but then I came across this KSPIV unit designed specifically for the 3rd-gen Expedition.  Overall I'm very happy with it, but it does have a few quirks I'm working through w/ KSPIV.  On that note, I have to commend KSPIV on their very personable support.  These Android units can be fairly complex and they're very responsive and open about how the unit works.

Who needs model numbers when you can have awesome SEO-driven product names like [KSPIV 4G+64G Android 9 Car Stereo 17 Inch Tesla Style Touchscreen for Ford Expedition 2007-2017 High Version Car Radio Bluetooth with Apple Carplay & Android Auto,GPS Navigation Unit,Backup Camera](https://amzn.to/3pxkje4)?
[![KSPIV](kspiv.jpg)](https://amzn.to/3pxkje4)

## Installation Notes

* Keep the clips from your old head and trim as you'll need them to snap the new unit it.  You can set it in place to test without the clips, but it'll fall out on heavy acceleration.
* You need to ground the reverse wire with the bullet end to the head chassis in order for it to properly detect when you're in reverse.

## Features

| Feature | Does it work? | Issue |
| - | - | - |
| Screen | Works OOTB -- vibrant and crisp |
| Split Screen | Works OOTB, but not all apps support it |
| Reverse View | Cam view app works OOTB for rear, front, and side inputs.  Screen goes black when vehicle is in reverse so long as the reverse wire with the bullet end is grounded.  The reverse cam doesn't show up though.  After putting the vehicle back in gear, you have to select the radio again to turn the amp back on. |
| Touch | Works OOTB including multi-touch gestures like pinch/zoom/drag, even with gloves on |
| Autodimming | Works OK OOTB, but doesn't go dim enough for night driving.  Twilight installed from the Play Store does the job better. |
| Virtual Assistant | Barely works -- you don't actually need it and I'd rather disable the overlay, but haven't figured out how to yet.  May need to follow up with KSPIV. |
| Android Auto | Works over USB and Bluetooth, but I'll never use it as native apps are nicer. |
| Cabin Mood Lighting | Has an app that matches the colors of the stock color switcher, but it doesn't seem to do anything.  I'm guessing it runs over the CAN2 connection that doesn't work.  Need to follow up with KSPIV. |
| Wireless Phone Charging | Plug [this charging mat](https://amzn.to/3ret2SZ) into one of the USB ports on the back of the head and route the cable under the unit then you can just throw your phone in the well to charge. |
| Wifi | Works OOTB.  Reception is a bit weak.  Works great with a hotspot in the truck, but can barely see my home wifi from the driveway even though my phone picks it up very well.  Antenna can be replaced, but I haven't found a good one yet. |
| Built-in 4G/5G | Non-existent -- unit does not have a SIM slot |
| Mobile connectivity | Works great OOTB with my phone's Wifi hotspot.  Works great OOTB over USB with a [Netgear M1](https://amzn.to/44uldqt).  The M1 reboots over and over if you don't have the battery in it and if you leave the battery in without driving often, the battery will die and the unit needs a few minutes of charging before it works again.  Still dialing in seamless mobile connectivity and may need to try some 4G/5G dongles, but this setup works "good enough for now". |
| Front A/C Controls | Work great OOTB |
| Rear A/C Controls | Rear Lock appears to be reversed -- rear controls work when Rear Lock is enabled on the head and the head overrides the rear controls when Rear Lock is disabled on the head. |
| Front Heated / Cooled Seats | Not currently working -- on-screen buttons don't respond to taps.  I need to follow up with KSPIV on this one. |
| Steering Wheel Controls | Volume Up/Down/Mute and Prev/Next work OOTB.  Other functions untested. |
| Door Open Display | Works OOTB so long as CAN2 is not connected |
| Speedometer / Tachometer | Don't work with or without CAN2 connected.  KSPIV recommended disconnecting CAN2 so the Door Open Display works properly and is sending me an OBDII dongle to see if we can get speedo and tach that way. |
| AM/FM Radio | Works OOTB |
| Pandora | Installs from Play Store and mostly works OOTB.  Sometimes you have to open up Radio then switch back to Pandora to get audio output. |
| Equalizer | Works OOTB, but can distort at high gain |
| Balance / Fade | L/R Balance works OOTB, but all speakers seem to be fed by the front channels.  Fading the fronts down on the head fades all speakers down and fading the rears down on the head does nothing.  Need to play around a bit with the rear controls and follow up with KSPIV.  Maybe this is similar to the Rear Lock for the A/C and I just haven't found it yet? |
| Amplifier | Works OOTB, but distorts at lower volume levels than I would expect.  You have to select the radio to turn on the amp before any other software can make sound. |
| Speakers | Plug and play with the Sony system in my truck.  My driver's door speaker is dead, but it was dead with the stock head as well -- need to troubleshoot, but it's not a problem w/ the KSPIV. |
| Waze | Installs from Play Store and works OOTB |
| GPS | Works with the antenna that comes with the headunit shoved up under the dash.  Can take a minute to get lock if you don't power it up every day.  Not working with the stock Expedition antenna at this time. Can take quite a while to get lock the very first time -- try sticking the antenna on the roof to get the initial lock before hiding it in the dash. |
| YouTube | Pre-installed and working OOTB |
| Netflix | Not available in the Play Store for Android 9.  If you write to KSPIV support, they'll send you an APK that works along with instructions on how to side-load it. |
| Play Store | Crashed a lot at first.  After finding a work-around to updating Play Store itself, it now works as it should.  Some apps are not available as the head is running Android 9 which is pretty outdated.  KSPIV is working on an Android 11 firmware for this unit that should improve the situation. |

## User Settings

| Setting | Description | Working | Thoughts |
|-|-|-|-|
|Autorun navi|Run preferred navigation app automatically on startup|Yes||
|Auto Split screen in navi|Automatically size your navigation app to half the screen and bring up the Console in the other half of the screen|Yes|Waze looks better with more screen real estate, so I keep this OFF|
|Navi volume|Navigation of the volume app|Untested||
|Track line|Trajectory lines on backup camera display|The lines show up when forcing the reverse display, but even though the lines are curved, they don't move with the steering wheel.|Is this supposed to come over the broken CAN2 connection?|
|Parking sound||Untested||
|Sound attenuation when reversing|Turn down the volume when the vehicle is in reverse|Regardless of how this is set, the unit cuts both the display and the amplifier when the vehicle is in reverse.|Working with KSPIV on this in https://github.com/cilynx/expedition/issues/1 and https://github.com/cilynx/expedition/issues/3 |
|Touch Tone|Beep every time you touch the screen|Yes|The tone isn't nearly as annoying as other Android heads I've played with.  I actually keep it enabled on this one.|
|ACC volume||Untested|
|Display speed|What to show in the console.  Meter: Speedometer and Tachomoter; Compass: Compass, Lat/Long, and Altitude from GPS; Gyroscope: Pitch, Role, and GPS info|GPS stuff works.  Speedo, tach, pitch, and role do not.|Is this supposed to come over the broken CAN2 connection?|
|Speed unit|MPH vs KM/H for the console speedometer|Yes||
|Temp unit|°F vs °C|Unit for the A/C and header bar temperature display|Yes||
|Sleep time|I think this is how long the unit will sleep after turned off before it powers down|Untested|When sleeping, the unit comes back up very quickly and to your prior state.  When powered down, bootup takes longer and goes to your default configured state.|
|Reset when break down|Not sure about this one -- guessing maybe it resets to some sort of failsafe configuration when the unit crashes|Untested||
|Brake detect|Lock out video playback unless the parking brake is on|Untested||
|Output image to external display||Untested||
|Car Auto-Apple device USB setting|Charge Only or Apple CarPlay|Untested|I don't use or want to use Apple CarPlay, so I keep this disabled.|
|Car Auto-Android device USB setting|Charge Only or Android Auto|Yes|I don't use or want Android Auto, so I keep this disabled.|
