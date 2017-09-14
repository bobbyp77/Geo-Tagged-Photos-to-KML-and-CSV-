# Geo-Tagged-Photos-to-KML-and-CSV- (Windows 7 version)

This tool will take a directory of geo-tagged jpeg images (including images in any subdirectories) and it will create a KML file (and a CSV file) in that directory.  The output KML file can be opened in Google Earth and each image location will be marked by a Google Earth icon (a black and white target).  Each icon is labeled with the image name using a user defined text color.  Clicking on an icon in Google Earth will open a balloon box displaying the image, the image path relative to the kml, the image capture date, camera azimuth, GNSS elevation.

The KML stores relative paths to the images so the entire directory with the KML can be moved/shared without destroying the integrity of the KML.  This tool does not require cloud storage, third party software, and the original images resolutions remain in tack. 

To view the original image in Google Earth Pro click a placemark to open the balloon.  Mouse over the image, right-click and choose open, then use the magnifying glass to view the original image.

The CSV file can be imported into qGIS or ArcGIS with coordinates in WGS84.  The CSV file output is not limited or inhibited by the ArcGIS license level restricting camera to point output sizes.
Google Earth Pro is now free! Get a free Google Earth Pro license here: https://support.google.com/earth/answer/176160?hl=en

Use:

1.	Navigate to and run the exe file located at:..\GeotaggedImagesToKMLandCSV\dist\GeotaggedImage2KML_CSV.exe
2.	 Follow the prompts for user inputs.
3.	After code execution use Google Earth to open the KML file in the user defined directory. 

USER INPUTS

1. A directory of images.
2. A project name (will be used to name the output files).
3. A KML text color.





Troubleshooting

I don’t have a cellular connection: Your phone’s GNSS does not need a cellular connection to record positions.

Total tool failure?  This tool was written in Python 2.7 using several third-party dependencies.  The Python files (and dependencies) have been compiled to a Windows executable.    You can create a shortcut from the executable and move the shortcut file but do not alter the file structures in the directories.  If you have altered the file structure reinstall the application. 

Total tool failure?  You do not need to install Python to run this program but some Windows-Python conversion files may be required.  Run this file...\GeotaggedImagesToKMLandCSV\addin\vcredist_x86.exe and then retry running GeotaggedImage2KML_CSV.exe

No KML File?  Ensure that the device is saving files as jpegs, the jpegs have geo-tag information and that you have read/write privileges to the directory of images.

Image azimuth not accurate?  Consult your user guide and calibrate the compass on your device before capturing images.  Confirm your camera records angles from true north not magnetic north.

Image elevation not accurate? This tool displays the elevation recorded by your GNSS.  GNSS elevations are not very accurate.  Sorry, your phone is not a substitute for a professional GNSS unit.

Picture is not where it should be?  Ensure your device is recording locations in latitude and longitude using WGS 84.  Turn on the GNSS unit.  Check settings to allow geo-tagging on your device.

Picture is still not where it should be:  Position accuracy is affected by weather, terrain, atmosphere, satellite availability, and GNSS electronics.  Some devises will store and report their last known location even with the GNSS turned off or even with little or no satellite coverage. The positions recorded by this tool are extracted from the positions recorded by your device.  You can improve your location accuracy by letting your GNSS run prior to capturing images.  Confirm your location in a mapping app like Google Maps to ensure your GNSS is recording and displaying your correct location before capturing images.  Your GNSS does not need a cellular connection to record positions.

Problem not addressed by this troubleshooting guide?  Idunno?  Email sample photos to Gerry@gabrisch.us for help.

By using this software you have agreed to this user end agreement:
This software is provided AS-IS, without warranty of any kind, expressed or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringment.  In no event shall the authors of copyright holders be liable of any claim, damages, or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software of the use or other dealings in the software.  Gerry Gabrisch.

