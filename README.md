# AirMediaAPI_ConfigTool
This is a script for simplifying Crestron AirMedia configuration for The University of Alabama's Audio Visual Solutions classroom deployments.
If your preferred configuration differs, you can customize this tool by editing the iterator variable in the python script, referencing the Crestron AirMedia API documentation:

	https://sdkcon78221.crestron.com/sdk/AM3K-API/Content/Topics/Objects/AirMedia.htm

To install this tool, follow instructions in the included AirMediaAPI_Instructions.txt.

The intended way to use this tool is to invoke it from the command line:
	
	cd ~/Downloads
	python AirMediaAPI.py

This tool will pull am_api_template.csv from your downloads folder, update AirMedias at the IP addresses listed in the file, and update firmware, if needed.
The current firmware file should also be saved in your downloads folder.
If you want to upgrade to a firmware version newer than 3.0600.0079, you will need to download the new .puf file, and update the puf_filepath variable in the python script.
