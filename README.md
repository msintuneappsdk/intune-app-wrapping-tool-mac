# Microsoft Intune App Wrapping Tool for macOS
Use the Intune App Wrapping Tool for Mac to enable Mac apps to be managed by Microsoft Intune

Version 1.0

See release notes for more information.

Use the Microsoft Intune App Wrapping Tool for macOS to pre-process macOS line-of-business (LOB) apps. Once you use this tool on your apps, you will then be able to upload and assign the apps to the Microsoft Intune console. 

Before you install and use Microsoft Intune App Wrapping Tool for macOS you **must**:
* Review the [Microsoft License Terms for Microsoft Intune App Wrapping Tool for macOS](https://github.com/msintuneappsdk/intune-app-wrapping-tool-mac/blob/master/LicenseTerms/Microsoft%20Software%20License%20Terms%20Intune%20App%20Wrapping%20Tool%20for%20macOS%20-%20English.pdf). Print and retain a copy of the license terms for your records. By downloading and using Microsoft Intune App Wrapping Tool for macOS, you agree to such license terms. If you do not accept them, do not use the software.
* Review the [Microsoft Intune Privacy Statement](https://docs.microsoft.com/legal/intune/microsoft-intune-privacy-statement) for information on the privacy policy of the Intune App Wrapping Tool for macOS.

Instructions on using the Microsoft Intune App Wrapping Tool for macOS:
* IntuneAppUtil -h
* IntuneAppUtil -r <filename.intunemac> [-v]
* IntuneAppUtil -c <source_file> -o <output_file> [-v]

Description: The IntuneAppUtil utility enables conversion of application installation files into the intunemac format which is compatible with Microsoft Intune. During the conversion process the IntuneAppUtil utility detects the parameters required by the MDM agent to determine the application installation state.

* -h  Help
* -r  Outputs the detection.xml file of the provided .intunemac file to stdout. The output contains the detection parameters and version of IntuneAppUtil used to create the .intunemac file.
* -c  <source_file>
    Converts the provided input filename. Only pkg file is supported.
* -o  <output_file>    Used in conjunction with -c parameter to specify the output path
* -v  Verbose: Produces additional progress output and error diagnostics.

