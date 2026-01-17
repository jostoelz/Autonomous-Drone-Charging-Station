# Abstract  
In this project, I am building an automatic charging device for drones. Once the drone has been landed on a platform by the pilot, a mechanism is activated that moves the drone into the correct position and starts the charging process. After the charging process is complete, the drone is ready for takeoff again.

# Project in Detail
The pilot lands on a landing platform. The landing platform has walls on two sides where two ultrasonic sensors are mounted. On the other two sides, a linear actuator with a slider is attached to each. As soon as the ultrasonic sensors detect a drone on the landing platform, the linear actuators move the drone into the corner until it is in the correct position. A wireless charging transmitter is mounted below the landing platform, while the corresponding wireless charging receiver is located underneath the drone. As soon as the ultrasonic sensors detect that the drone is in the corner, current flows from a power supply to the wireless charging transmitter. The receiver on the drone converts the alternating voltage into direct current, which then flows into the drone's battery, which is connected to the wireless charging receiver via a cable. Once the charging process is complete, the drone can take off again.

## Mandatory
* The drone must be able to land on a platform.
* The drone is moved into the correct position and charged via wireless charging.
* The drone must be able to take off again after the charging process.

## Optional
* The box is equipped with weather sensors and gives the pilot recommendations on whether or not to fly, depending on weather conditions.
* During the charging process and while flying, the box remains closed to protect the drone and the box from precipitation.
* The box is self-sufficient through solar panels and can recharge itself in good weather.
* The station is equipped with LEDs that illuminate the landing site in the dark so that the drone can land safely even at night.
* The station sends notifications to the pilot when the charging process is complete.
* The station can access external weather forecasts and warn the pilot of storm or precipitation warnings.
* The station reads the battery status of the drone and informs the pilot in good time about the need for a landing.
* The station has GPS so that safe landing is possible even without visual contact, the fastest route between the drone and the charging station can be displayed, or tracking can take place if the station has been stolen.

# Schedule
<table>
  <thead>
    <tr>
      <th>Task</th>
      <th>Finished by:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Project description</td>
      <td>19.11.24</td>
    </tr>
    <tr>
      <td>Ordering materials</td>
      <td>26.11.24</td>
    </tr>
    <tr>
      <td>Wireless charging</td>
      <td>17.12.24</td>
    </tr>
    <tr>
      <td>Mechanism: Linear actuators move drone to the correct position once ultrasonic sensors give permission</td>
      <td>07.01.25</td>
    </tr>
    <tr>
      <td>3D printing of the landing platform and drone mount</td>
      <td>14.01.25</td>
    </tr>
    <tr>
      <td>Combine wireless charging, mechanism, and 3D printing</td>
      <td>04.02.25</td>
    </tr>
     <tr>
      <td>Finalize documentation</td>
      <td>11.02.25</td>
    </tr>
    <tr>
      <td>Buffer or install optional features</td>
      <td>18.02.25</td>
    </tr>
    <tr>
      <td>Project submission</td>
      <td>28.02.25</td>
    </tr>
  </tbody>
</table>

# Sketch 
Hardware on the landing platform:
![Hardware on the landing platform](Bilder/Hardware_Landeplattform.jpg)
Hardware on the drone:
![Hardware on the drone](Bilder/Hardware_Drohne.jpg)
Visualization of the landing platform:
![Visualization of the landing platform](Bilder/Visualisierung_Landeplattform.png)

# Cost Estimation
<table>
  <thead>
    <tr>
      <th>Components</th>
      <th>Price per piece</th>
      <th>Link</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Wireless charging transmitter & receiver</td>
      <td>7.71 Fr.</td>
      <td>https://www.mouser.ch/ProductDetail/Seeed-Studio/106990017?qs=SElPoaY2y5KdLskE1shzqQ%3D%3D&mgh=1&utm_id=20002739518&gad_source=1&gclid=CjwKCAiA3ZC6BhBaEiwAeqfvyuNlfda5-xuXoLrLc3qdhUh8dxR87X4ZW45SWwa3tzxUaDRKo-8zQBoC-xEQAvD_BwE</td>
    </tr>
    <tr>
      <td>Open end to USB C</td>
      <td>5.45 Fr.</td>
      <td>https://www.conrad.ch/de/p/usb-c-3-1-stecker-mit-offenem-kabelende-usb-c-3-1-tc-2509033-tru-components-inhalt-1-st-1587137.html</td>
    </tr>
    <tr>
      <td>Power supply</td>
      <td>5.33 Fr.</td>
      <td>https://www.reichelt.com/ch/de/shop/produkt/steckernetzteil_10_w_5_v_2_a-370227?PROVID=2808&gad_source=1&gclid=Cj0KCQiAi_G5BhDXARIsAN5SX7rT-tWpARV_9-TJFdsRmyKfdBHIgLwCn7fREIx21GYVdz2y2PMDzvgaAjFpEALw_wcB&q=%2Fch%2Fde%2Fshop%2Fsteckernetzteil-10-w-5-v-2-a-ys12v-0502000e-p370227.html </td>
    <tr>
      <td>Transformer</td>
      <td>3.90 Fr.</td>
      <td>https://www.bastelgarage.ch/dc-dc-1-5a-step-up-boost-converter </td>
    </tr>
    <tr>
      <td>Mosfet</td>
      <td>2.25 Fr.</td>
      <td>https://www.adafruit.com/product/355 </td>
    </tr>
    <tr>
      <td>Linear actuator</td>
      <td>35.90 Fr.</td>
      <td>https://www.bastelgarage.ch/6v-electric-cylinder-100mm-128n?gad_source=1&gclid=Cj0KCQiAi_G5BhDXARIsAN5SX7pOlEy0XSUf0RxYFtqWwyanmA4Y5NWjRPP5CRwlg6IoworPIEc1klAaAvznEALw_wcB</td>
    </tr>
    <tr>
    <td>Motor driver</td>
    <td>6.60 Fr.</td>
    <td>https://www.conrad.ch/de/p/joy-it-sbc-motodriver2-entwickler-platine-1-st-1573541.html?utm_source=google-shopping-de&utm_medium=search&utm_campaign=shopping-online-de&utm_content=shopping-ad_cpc&WT.srch=1&ef_id=Cj0KCQiAi_G5BhDXARIsAN5SX7o6_0Nbb4KqGNjm55Ye8g1xzGAJNyGisIYAgcIQBwoagaDJP2YjFNAaAjlnEALw_wcB%3AG%3As&utm_source=google&utm_medium=cpc&utm_campaign=ade_3_shopping_GERMAN&utm_id=319998844&gad_source=1&gclid=Cj0KCQiAi_G5BhDXARIsAN5SX7o6_0Nbb4KqGNjm55Ye8g1xzGAJNyGisIYAgcIQBwoagaDJP2YjFNAaAjlnEALw_wcB </td>
    </tr>
    <tr>
    <td>Ultrasonic sensor</td>
    <td>3.28 Fr.</td>
    <td>https://www.reichelt.com/ch/de/shop/produkt/entwicklerboards_-_ultraschall_abstandssensor_hc-sr04-161487?PROVID=2788&gad_source=1&gclid=CjwKCAiAl4a6BhBqEiwAqvrquhSdVMxJ-SXono8RQaygsfe0myq6rt9zlikawhww3HqIJLXRNSHbShoCsIEQAvD_BwE&q=%2Fch%2Fde%2Fshop%2Fentwicklerboards-ultraschall-abstandssensor-hc-sr04-debo-sen-ultra-p161487.html </td>
    </tr>
  </tbody>
</table>

Note: I need two linear actuators and two ultrasonic sensors. Furthermore, resistors, LEDs, a display, a potentiometer, and a switch were not mentioned.
