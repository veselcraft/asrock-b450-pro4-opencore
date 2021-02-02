![Screenshot](/screen.png?raw=true)

This is OpenCore configuration that can be applied to Asrock B450 Pro4. Tested on macOS 10.13.6, 10.15

## Installation
  1. Create directory "EFI" in your EFI partition (e.g. pendrive or hard drive)
  2. Clone this repo and paste directiories "BOOT" and "OC" onto created directory
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select 
  4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB  (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.

## Known issues
* NVMe drives are detected as external
* USB 2.0 ports does not work (seems like it is problem of DSDT that i tooked from [here](https://github.com/misifiksi/ryzentosh-highsierra))