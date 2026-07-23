# 3. Set up UAV & NAV (At Site)

Once at the field site:

* Unpack the UAV from case and extend all legs.
* Extend all arms and remove protective covers from the propellers.
    * Check that all propellers and arms are secured.
* Attach all antennas:
    * Color coded to dots on the UAV; **2 red, 2 blue, 1 yellow**.
    * Carrier link attachment to top of UAV: screw in.
    * Carrier link block: **2 long antennas**.
    * GCS: Flat antennas (**do not turn on yet**).
* **Mount the sensor:**
    * With the lidar facing back (opposite RGB), use the central locking system to secure sensor to UAV using ring lock.
    * Rock slightly to ensure sensor is fully attached.
* **Mount the batteries:**
    * Lock on each side (you should hear a click).
* **ALL ANTENNAS SHOULD BE CONNECTED AT THIS PT** (including UAV, GCS, and CarrierLink).
* Connect batteries to UAV by connecting the yellow-capped cables. You will hear the UAV start to hum as the SWIR cooling system turns on.
* Connect the carrier link to the laptop through the USB top port.
* Turn on the **Garmin GPS**.

---

## Calibration

* Connect the sensor to the laptop using **2 ethernet cables** and the **USB connection**.
* Once connected, open **Hyperspec III**:
    * Place the white reference under sensor and remove the cap from the sensor on the bottom.
    * Open the **"Live Video"** for both the VNIR (nano) and SWIR.
    * In the live video windows, select **"crosshair"** and place it in a bright, uniform white area.
    * Adjust the exposure so that the max gain is at **80-90%** in each window:
        * **VNIR:** 3500-3800 cts
        * **SWIR:** 5000 cts
    * Enter your altitude into each window to see calculated speed at the bottom. **VNIR and SWIR speeds should be max 0.5 m/s apart**.
    * Frame period: min **5ms**, same or greater than exposure.
    * Gain = **HIGH**
    * Distance to object: e.g., 50m above tree crowns.
    * Note down your calculated speeds and altitude (distance to objects).
* Still in Hyperspec III:
    * Open **"setup GPS"**.
    * Import the kml polygon file for your flight area of interest for both the VNIR and SWIR windows (must do this twice).
    * Check to see if there is an **x** for the UAV location in relation to the polygon. UAV must be **OUTSIDE** of polygon at this point and for GPS initialization. Calibration tarps must be **INSIDE** the polygon.
* Still Hyperspec III:
    * Open the **"capture"** window.
    * Set to **on-board storage**, set folder prefix.
    * Click **"connect dark reference"**, ensure lens cap gets put on, and click **GO**.
    * Once this is done, check the box that says **"enable GPS triggering"** and click **GO**. It will ask if the lens cap is now **OFF** (remove the cap) and click **GO** again.
    * You should note that there is a **Pause** button. This should remain and means you are good to go.
* Close **Hyperspec III**.

---

## Ground Control & Controller Prep

* Open **HA Ground Control** on laptop:
    * You should see your flight plan. If you need to load your plan, go to file in HAGC and import your saved plan from earlier.
    * Set the speed and flight altitude that you calculated during calibration above in the survey section on the right hand of the screen.
    * Adjust the plan as needed (including launch, tarps, flight lines, etc.).
    * Save plan and click **upload to UAV** (should appear at the top of the screen if you are connected via carrier link. After pressing it you will see a green progress bar).
* Once uploaded: Disconnect the laptop, remove both ethernet cables.
* Connect the **lidar cable** (white) to the VNIR port!
* **Turn on the controller:**
    * Press the power/lock button (top center) and let it turn on.
    * Press & hold the left **DISARM** button for a few seconds to power on NAVBAY, you will hear a beep.
    * Press & hold the radio power button centered on back of control (on top of the navbay system).
    * Check if the radio is on: **blue light** top left.
    * You should see green lights as well that relay the NAVBAY battery level (4 batteries for 25% sections).
    * *The presence of a red LED on the far left indicates that there may be a hardware malfunction with the controller. If this occurs, power cycle the controller and NavBay.*
* **Connect Controller to Garmin:**
    * Open **GNSS** (an app on the controller) and click **connect**.
* Open **HA Ground Control on controller:** Download the flight plan from the UAV.
    * To download you may have to click the file button on ground control and select download from UAV.
    * You should now see your flight plan on the controller and location of yourself and the UAV.
    * Enter correct flight specs (speed, altitude) if they have changed.
    * After changing anything, re-upload the plan to the UAV.
* Remove the lidar and spec covers.
* *If you move locations after you connect the GPS, you way need to reset it. You will get an error that operator location is not set on the controller - go into GNSS and reconnect.*