# 2. Pre-Flight Planning on Laptop

Before you head to the field for a flight, you must complete the following steps and have the needed maps downloaded for offline use:

## Determine Your Flight Area of Interest
* Open **Google Earth Engine**.
* Create a polygon over your area of interest for flight planning.
    * The sensor will record data *inside/* the polygon only, so all calibration tarps and flightlines must be within this area.
    * The UAV setup and launch will occur *outside/* of this polygon.
* Save this polygon as a **.kml** on the laptop. 

## Make your Flight Plan
* Open **HA Ground Control** and click the file button on the left hand side.
* Navigate to where you stored the .kml of your flight area and import the polygon. 
* You should see the polygon appear on the map. On the right hand side you should see a survey button. Click it and there you can adjust flight lines etc. 
    * Fly in cardinal directions if possible, but whatever makes the mose sense for your area. 
    * Set over lab to 40% (Dependent on timing and size, but try to not go below 30%)
    * You will adjust the capture speed after calibration, but for right now set it to 3m/s - 5m/s
    * Move the launch button to where you will launch from, and then on the left hand side click "return" that will include that in the plan. 
        * You can adjust the entrance point in the survey section on the right hand side by clicking *rotate entrance point/* 
    * On the right hand side you should also see a fence button. You can add a flight fence to the area

    * On the top of the screen you should see estimates flight time. This should NOT be over 15 minutes. Preferably with some wiggle room. 

* On the left hand side click **files** again and save.as - you can then save your flight plan to a local folder etc so you can find it again in teh field. 

## Download Your Necessary Offline Maps
* In **HA Ground Control** on both laptop and the controller.
* Click the HA in the upper left-hand corner and click application settings.
* Go to offline maps and select **"add new set"**.
* Move your screen to the area you want captured and set the zoom levels to what is needed for your flight plan (what you can/want to see resolution-wise).
* Download tiles for **Bing Hybrid** as well as **Copernicus Elevation**.
* Ensure tiles are fully downloaded on laptop and controller before going into the field.
    * I like to put everything on airplane mode and see if things are loading properly as if I was in teh field. 

## Turn off the Controller!
* Before you headout, may sure the NavBay and controller are completely powered off. Press and hold that top middle button until a power off button appears on the screen. Click it. 

## Summary Checklist
You should now have downloaded:
* Kml for flight area including calibration tarps.
* .plan file stored locally
* Offline maps loaded onto both computer and the GCS in HA Ground Control.