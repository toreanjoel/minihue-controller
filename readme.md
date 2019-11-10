# **miniHue-FK**

#### How it works:
This will take a string and will run the string as a method name. There will be delimiters that will split the strings and separate strings as well as be passing arguments to the functions.

Currently you will be sending commands using any bluetooth terminal or serial device when connected to a computer. You will be expected to either write your own (CMD tools, Python scripts, Node modules etc.)

###### Future Additions:

 - Planning in finishing the desktop application and allow adhoc means to send serial data easier
 - Convert the application to a mobile app (bluetooth protocol)

###### Note:

 - One of the two above will be made and it might be more app than desktop.
 - The COLOR and BRIGHTNESS values that you use after calling the function i.e "c?100.100.20" - range between 0 - 255
 
###### Constants used below:

- RED: 0 - 255
- GREEN: 0 - 255
- BLUE: 0 - 255
- BRIGHTNESS: 0 - 255
- MODE:
	- 0: Custom mode where the user changes the color
	- 1: Animation mode

###### Commands:

 - **`ping`** - returns current status of all the values that are being run. Brightness levels, color value, mode etc.

 - **`on`** - turns the lamp on

 - **`off`** - turns off the lamp

 - **`c?{RED.GREEN.BLUE}`**

    - Then comes the rgb color string (note the full stops between the values)
    - e.g `c?255.0.0`

 - **`m?{MODE_NUMBER}`** - Mode between custom and animation

  - e.g `m?1`

 - **`b?{BRIGHTNESS_VALUE}` **- The brightness level

   - e.g `b?150`

