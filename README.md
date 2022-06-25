# Alexa_ringbell
The objective of this project is to connect a conventionel door bell to Amazon Alexa in order to show bosch eyes camera stream on an Echo Show 10. The intended action flow is shown below:

![imgs/action_flow.png](imgs/action_flow.png)

The easiest input sensor for Alexa routines seem to be reed window sensors. Most window sensors are connected via WiFi which brings two disadvanteages:
1. The need to connect the Alexa account to a 3rd party account of the sensor maker.
2. There is an additional delay, at least when tested with a [Luminea sensor](https://www.pearl.de/a-NX4900-3103.shtml)

Instead of a WiFi sensor I decided to use a Zigbee sensor, which is easily done because the Echo Show 10 includes a Zigbee hub.
The [SONOFF SNZB-04](https://sonoff.tech/product/smart-home-security/snzb-04/) seems as a good choice for my application. It's integration with the custom pull-down circuit into the ringbell houding is shown here:

![imgs/HW_V2_integrated.jpg](imgs/HW_V2_integrated.jpg)