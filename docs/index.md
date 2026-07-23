# Drone & Sensor Platform Guide

> [HEADS UP!]
> **FAA REGULATIONS!:** The remote pilot in command must be in possession of a valid **FAA Part 107 certification** and have it printed and on person at all times during flight operations.

---

## Important Things to Note!

* **Antenna Protocol:** Never power the GCS (controller) or UAV on without first attaching all antennas.
* **Power Sequencing:** Connect batteries to the UAV *before* connecting to the sensor to avoid possible power surges.
* **Battery Health:** Never let the UAV battery fully discharge.
* **Link Management:** The Garmin and carrier link can only speak to one device running HAGC at a time. If connected to the drone via carrier link and Garmin on the computer, you must disable the **RID** feature in HAGC on the controller (and vice versa). Keep the controller completely off until the flight plan is loaded and sent to the UAV from the computer.
* **Flight Limits:**
    * **Target Speed:** 3–6 m/s (Min = 1 m/s, Max = 10 m/s)
    * **Max Wind:** 30 mph = 25 knots = 45 km/h (verify via app)
    * **Max Altitude:** 400 ft AGL = 120 m AGL

* In the field the computer may have trouble connecting if it is too hot. Helpful tips to combat this include staying in the shade with the laptop, sitting in the car with it with AC blasting while drone is setup outside the car, or wetting a bandana and cooling that way. If computer shuts down completely, you can force a reset by pressing and holding the power button for about 30 seconds. 

---

## Instrument Specs

| Parameter | VNIR (Nano) | SWIR |
| :--- | :--- | :--- |
| **Spectral Range** | 400–1000 nm | 900–2500 nm |
| **Spectral Bands** | 340 bands | 267 bands |
| **Spectral Resolution (FWHM)** | 6 nm | 8 nm |
| **Radiometric Resolution** | 12-bit | 16-bit |
| **Spectral Sampling (Dispersion/Pixel)** | 1.76 nm pixel⁻¹ | 6 nm pixel⁻¹ |
| **Spatial Pixels Across Track** | 1020 pixels | 640 pixels |
| **Detector** | CMOS | MCT |

