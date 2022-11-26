DayZ Chernarus Big Oil Rig By EZ Rich For Console and PC xml json Mod Instructions & Terms Of Use

These files spawn a large oil rig, with loot, in the sea 1.4km South of the Light-House on the Coast West of Chernogorsk.

Limited Testing on PC Chernaus Local Server DAYZ Version 1.15 Dec 2021.

Created by AND BIG THANKS TO: EZ Rich ( terrellerich91#2154 on Discord).

Many Thanks To Inclement Dab for his amazing DayZ Editor that makes this all possible: https://steamcommunity.com/sharedfiles/filedetails/?id=2250764298

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded xml / json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Ensure your DayZ Server has activated the cfggameplay.json. For console users on Nitrado Servers, go to "General Settings" on your server and tick "Enable cfggameplay.json".

On PC Servers add the following line to your serverDZ.cfg:

enableCfgGameplayFile = 1;

(On some PC servers, including Nitrado, the serverDZ.cfg is "hidden", so you need to enable "expert mode" in settings,
then go to "expert settings", which is the serverDZ.cfg. Stop the server before making changes this way.)

Upload "ez-rich-oil-rig.json" from the extracted files to inside the "custom" folder of the mission directory on your server. This file places the structures on your map.
(If you haven't got a "custom" folder, create one.)

Open the cfggameplay.json file in the correct mission file for your server and look for the "objectSpawnersArr" line.

This file tells your server to access your custom file.

Edit it to look like this: 

	"objectSpawnersArr": ["custom/ez-rich-oil-rig.json"],
	
If you already are calling custom jsons to spawn items, seperate the files like this:

	"objectSpawnersArr": ["custom/ez-rich-oil-rig.json","custom/anotherfile.json","custom/differentfile.json"],
	
Save your changes & upload if you need to.
	
Next we add loot to the structures by adding the following code snippet to the top of your mapgrouppos.xml file, after <map> 

	<!--big oil rig loot-->
	  <group name="Land_Construction_Building" pos="6030.310059 32.535400 553.257019" rpy="0.000000 0.000000 144.000000"/>
	<group name="Land_Construction_Building" pos="5991.520020 32.000000 514.164978" rpy="0.000000 0.000000 54.499996"/>
	<group name="Land_Container_1Aoh" pos="6058.689941 26.000000 554.330994" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="5999.470215 7.500000 526.145020" rpy="0.000000 0.000000 -34.000000"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="6025.870117 7.500000 541.375977" rpy="0.000000 0.000000 54.999992"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="6022.299805 7.500000 496.196991" rpy="0.000000 0.000000 145.999969"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="6049.520020 7.500000 520.278015" rpy="0.000000 0.000000 144.000000"/>
	<group name="Land_Construction_Building" pos="6041.709961 32.472599 518.786987" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Ship_Big_FrontA" pos="6045.930176 14.599500 583.523010" rpy="0.000000 0.000000 18.000000"/>
	<group name="Land_Ship_Big_FrontB" pos="6026.250000 13.000000 587.299988" rpy="0.000000 0.000000 18.000000"/>
	<group name="Land_Ship_Big_BackB" pos="5955.240234 11.100000 575.135986" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Ship_Big_BackA" pos="5971.350098 12.512600 586.206970" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Ship_Big_Castle" pos="5964.879883 20.986099 582.085999" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Construction_House2" pos="6036.709961 42.369801 518.234985" rpy="0.000000 0.000000 53.999996"/>
	<group name="Land_Container_1Aoh" pos="5989.240234 -0.434310 611.523987" rpy="0.000000 -11.499999 0.000000"/>
	<group name="Land_Mil_Tent_Big2_3" pos="6014.680176 27.400000 527.208008" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Mil_Tent_Big1_2" pos="5995.870117 25.299999 538.046997" rpy="0.000000 0.000000 -125.999992"/>
	<group name="Land_Mil_Tent_Big2_4" pos="6006.990234 27.400000 535.741028" rpy="0.000000 0.000000 53.999996"/>
	<group name="Land_Mil_Tent_Big4" pos="6047.549805 39.299999 560.872986" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Mil_Tent_Big2_5" pos="6022.629883 16.900000 500.329987" rpy="0.000000 0.000000 144.000000"/>
	<group name="Land_Mil_Tent_Big1_4" pos="6021.209961 14.800000 510.740997" rpy="0.000000 0.000000 53.999996"/>
	<group name="Land_Mil_Tent_Big1_5" pos="6009.979980 14.800000 503.756989" rpy="0.000000 0.000000 -125.999992"/>
	<group name="Land_Mil_Tent_Big1_3" pos="6002.379883 14.800000 512.286987" rpy="0.000000 0.000000 144.500000"/>
	<group name="Land_Mil_Tent_Big2_2" pos="6008.790039 16.799999 526.315979" rpy="0.000000 0.000000 53.999996"/>
	<group name="Land_Mil_Tent_Big1_1" pos="5992.370117 14.800000 523.978027" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Mil_Tent_Big2_1" pos="6020.109863 16.799999 546.382996" rpy="0.000000 0.000000 -27.000000"/>
	<group name="Land_Mil_Tent_Big4" pos="6016.850098 16.000000 531.806030" rpy="0.000000 0.000000 53.999996"/>
	<group name="Land_Mil_Tent_Big1_4" pos="6034.830078 14.800000 528.593994" rpy="0.000000 0.000000 -125.999992"/>
	<group name="Land_Mil_Tent_Big1_3" pos="6039.879883 14.973500 522.249023" rpy="0.000000 0.000000 -125.999992"/>
	<group name="Land_Mil_Tent_Big1_4" pos="6044.580078 14.800000 515.893005" rpy="0.000000 0.000000 -125.999992"/>
	<group name="Land_Mil_Tent_Big2_2" pos="6051.149902 16.799999 530.239014" rpy="0.000000 0.000000 53.999996"/>
	<group name="Land_Container_1Mo" pos="6043.939941 15.993400 537.916016" rpy="0.000000 0.000000 -125.999992"/>
	<group name="Land_Container_1Mo" pos="6035.799805 16.008301 545.013977" rpy="0.000000 0.000000 63.000000"/>
	<group name="Land_Container_1Mo" pos="6033.919922 15.993400 547.463989" rpy="0.000000 0.000000 53.999996 "/>
	<group name="Land_Container_1Mo" pos="5994.850098 15.993400 535.169983" rpy="0.000000 0.000000 -27.000000"/>
	<group name="Land_Container_1Mo" pos="6012.620117 15.993400 493.470001" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Container_1Aoh" pos="6020.990234 26.484501 503.264008" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Container_1Bo" pos="6021.100098 29.073000 503.309998" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Container_1Aoh" pos="6017.479980 26.714399 508.066010" rpy="0.000000 0.000000 144.000000"/>
	<group name="Land_Container_1Bo" pos="6039.979980 26.335300 534.659973" rpy="0.000000 0.000000 -125.999992"/>
	<group name="Land_Container_1Mo" pos="5984.540039 38.656502 510.105011" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Container_1Mo" pos="6026.549805 39.128601 501.199005" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Container_1Aoh" pos="6027.379883 39.088600 504.101990" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Mil_Tent_Big1_4" pos="6036.580078 37.990002 548.783997" rpy="0.000000 1.000000 144.000000"/>
	<group name="Land_Pier_Crane_A" pos="5955.640137 16.229799 556.620972" rpy="0.000000 0.000000 144.000000"/>
	<group name="Land_Container_1Mo" pos="6027.970215 39.201099 563.663025" rpy="0.000000 0.000000 53.999996"/>
	<group name="Land_Container_1Bo" pos="6010.419922 -0.714860 626.773010" rpy="0.000000 -15.499998 18.000002"/>
	<group name="Land_Container_1Moh" pos="6002.100098 0.009390 609.734009" rpy="0.000000 0.000000 45.000000"/>
	<group name="Land_Container_1Mo" pos="6000.450195 1.802210 612.924011" rpy="0.000000 -19.000000 -35.999996"/>
	<group name="Land_Container_1Bo" pos="5996.089844 -0.148810 614.643005" rpy="0.000000 0.000000 45.000000"/>
	<group name="Land_Container_1Mo" pos="5962.290039 12.074900 540.823975" rpy="0.000000 0.000000 -35.999996"/>
	<group name="Land_Container_1Mo" pos="5964.759766 12.074900 544.007996" rpy="0.000000 0.000000 -18.000000"/>
	<group name="Land_Container_1Mo" pos="5983.250000 12.074900 542.171997" rpy="0.000000 0.000000 0.000000"/>
	<group name="Land_Container_1Aoh" pos="5981.029785 14.615000 537.140015" rpy="0.000000 0.000000 -125.999992"/>
	
Save your changes & upload if you need to.

Restart your server and the new structures will appear immediatly, and then they will slowly stock with loot.

Org File Created by Your EZ Rich. For more help files for DayZ come visit us at http://bhaalshad.com 
If you upload this to another Discord or webpage, please leave filename intact and dont take credit
as your own. Thank you and enjoy :)  

Thanks, Rob.



