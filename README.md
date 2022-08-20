# nordic-freetube <br>
## Overview & Credits
A custom theme for the FreeTube YouTube Client that is based on the [Nord Color Palette](https://www.nordtheme.com/)

Updated and working version of Marc Llorca's [freetube-nord](https://github.com/llorca-mfs/freetube-nord) with a linux tutorial added

![alt text](https://github.com/zecm/nordic-freetube/blob/c1788341a7364fc5bd39b315eca0b2692060ee37/screenshots/screenshot1.png)
![alt text](https://github.com/zecm/nordic-freetube/blob/c1788341a7364fc5bd39b315eca0b2692060ee37/screenshots/screenshot2.png)



# Windows: <br>

## Pre-requisites:

1. [7-Zip](https://www.7-zip.org/download.html)
2. [Asar7z Plugin](https://www.tc4shell.com/en/7zip/asar/)

<br>

## How to install:

1. Install the Asar7z plugin for 7-Zip
2. Go to to the directory where you installed the FreeTube Desktop Client
3. Go to resources
4. Right-click on the "app.asar" file, hover on 7-Zip, then click on "Open Archive"
5. Once the archive has opened, in 7-Zip, open the "dist" folder
6. Look for the "renderer.f754525d9b3da96424e4.css" and delete it
8. Replace it with the "renderer.f754525d9b3da96424e4.css" file of this repository
9. Open FreeTube, then go to Settings
10. Scroll down to "Theme Settings", then change into the following parameters:
    * Base Theme: Black
    * Main Color Theme: Cyan
    * Secondary Color Theme: Cyan


If all works correctly, then you should have applied the Nord theme by now. Enjoy!


<br><br>

# Linux: <br>

## Pre-requisites:

1. asar      &nbsp;  `sudo npm install -g asar`

<br>

## How to install:

1. Go to the resources directory  <br> `cd /opt/FreeTube/resources` <br><br>


2. Extract the app.asar archive     <br> `sudo asar extract app.asar app_extract` <br><br>

3. Go to the dist directory   <br> `cd app_extracted/dist/` <br><br>

4. Remove the "renderer.f754525d9b3da96424e4.css" file and replace it with the one on my repository

<br>

5. Go back to the resources directory   <br> `cd ../..` <br><br>

6. Replace the old app.asar <br> `sudo rm -f app.asar && sudo asar pack app_extracted app.asar && sudo rm -rf app_extracted` <br><br>

7. Open FreeTube, then go to Settings
<br><br>

8. Scroll down to "Theme Settings", then change into the following parameters:
    * Base Theme: Black
    * Main Color Theme: Cyan
    * Secondary Color Theme: Cyan
    

If all works correctly, then you should have applied the Nord theme by now. Enjoy!

