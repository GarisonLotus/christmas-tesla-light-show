# **Tesla Light Show Christmas install Guide**

## Details on this presentation

### Song

Song from Candelight Reflections, Tokyo DisneySea. Modified from 5 minutes down to just over 2 minutes to not hit memory limits on the car.

###
Sample video show: https://youtu.be/7z8gpYP6hrE


## Running this custom show on a vehicle
A custom show can be run on a supported vehicle by loading it via a USB flash drive. Create and share your shows with others! A single show can be shared and run on any supported vehicle; they are not model-specific. The sequence data is stored in a .fseq file and the music comes from your choice of .mp3 or .wav.
### Supported Vehicles
- Model S (2021+)
- Model 3
- Model X (2021+)
- Model Y
- Running Software v11.0 (2021.44.25) or newer
### USB flash drive requirements
- Must contain a base-level folder called "LightShow" (without quotation marks and case sensitive - just copy the folder in this git repo).
- The LightShow folder must contain 2 files:
  - "lightshow.fseq"
  - "lightshow.mp3" or "lightshow.wav" (wav is recommended)
- Must be formatted as exFAT, FAT 32 (for Windows), MS-DOS FAT (for Mac), ext3, or ext4. NTFS is currently not supported.
- Must **not** contain a base-level TeslaCam folder.
- Must **not** contain any map update or firmware update files.
### Running the custom light show on a vehicle
- Insert the flash drive into one of the front USB or USB-C ports, or glovebox USB port, then wait a few seconds.
- In Toybox, select Light Show and tap Start The Show. If the files on the USB flash drive meet the requirements, then the custom show will be used instead of the built-in show.

- As the custom light show loads, the status at the bottom of the popup cycles through "Loading lightshow.fseq" and "Loading light show...". When the status becomes "Light show ready!", you can exit the vehicle and the custom show will start.

### Debug
- If the popup title is "Light Show" instead of "Custom Light Show", then the requirements are not being met for the USB flash drive formatting and/or required folder and files.
- Error messages will be provided if the required files exist but there is a problem with the light show sequence file.
