# victron_ev_charger_in_home_assistant
Description and example of the MQTT code and dashboard to get the stats showing and having control of the EV charging.  

Firstly credits to SmartyVan, I had some basic Home Assistant MQTT integration setup but his video and code is next level..!  

https://www.youtube.com/watch?v=hx8UjOLD1tw

To get this working I thought would provide the steps as it wasn't straight forward  :-)

Steps

Physical install of the Victron EV Charger
Make sure that the firmware is updated, this has to be done either via the VRM portal or locally you will be best to ask the installer as the firmware is only available to those with a Victron professional account.
If you have any issues installing the firmware install it at least twice preferably locally.  Yes that sounds strange, but it worked for me.
https://community.victronenergy.com/t/ev-charging-station-hangs-after-firmware-update/8658/2

Configure GX
Firstly update the firmware on this via the VRM portal.  You need a relatively new version of Venus OS to work properly.
https://www.victronenergy.com/media/pg/EV_Charging_Station/en/setup,-configuration---operation.html#UUID-a5b3df40-5a60-184f-b5b4-a3465a6ad69b
My EV charger did not automatically appear and I had to search and manually update

Configure EV Charger
Follow the manual to connect the EV charger to your WIFI.  Make sure it's the same network as your GX device.
Configure the GX device comms and also include the GX in the whitelist.
Check comms if this doesn't pass you must resolve that first
https://www.victronenergy.com/media/pg/EV_Charging_Station/en/index-en.html

You should now be able to see the EV Charger in the GX (and VRM portal) and from the EV Charger see stats like solar, battery etc

Matt
