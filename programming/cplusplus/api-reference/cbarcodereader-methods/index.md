---
layout: default-layout
title: CBarcodeReader Methods - Dynamsoft Barcode Reader SDK C++ Edition API Reference
description: This page shows CBarcodeReader methods of Dynamsoft Barcode Reader SDK C++ Edition.
keywords: methods, CBarcodeReader, api reference, c++
needAutoGenerateSidebar: true
---

# class dynamsoft::dbr::CBarcodeReader

## Constructor and Destructor
   
  | Method               | Description |
  |----------------------|-------------|
  | [`CBarcodeReader`](constructor-and-destructor.md#cbarcodereader) | Default constructor of `CBarcodeReader` object.|
  | [`~CBarcodeReader`](constructor-and-destructor.md#~cbarcodereader) | Destructor of `CBarcodeReader` object.|
  | [`GetInstance`](constructor-and-destructor.md#getinstance) | Gets an idle Dynamsoft Barcode Reader instance running on concurrent instance mode. |
  | [`Recycle`](constructor-and-destructor.md#recycle) | Recycles a Dynamsoft Barcode Reader instance running on concurrent instance mode. |
   
   
## License
  
  | Method               | Description |
  |----------------------|-------------|
  | [`InitLicense`](license.md#initlicense) | Initializes license key and activate the SDK. |
  | [`GetDeviceUUID`](license.md#getdeviceuuid) | Gets the device uuid used for license activating. |
  | [`IsInstanceValid`](license.md#isinstancevalid) | Gets whether the instance is valid when charging by concurrent instances count. |
  | [`SetDeviceFriendlyName`](license.md#setdevicefriendlyname) | Sets a human-readable name that identifies the device. |
  | [`SetLicenseCachePath`](license.md#setlicensecachepath) | Sets a directory path for saving the license cache. |
  | [`SetMaxConcurrentInstanceCount`](license.md#setmaxconcurrentinstancecount) | Sets the max concurrent instance count used for current device and process. |
  | [`GetIdleInstancesCount`](license.md#getidleinstancescount) | `Deprecated` |
  | [`InitLicenseFromServer`](license.md#initlicensefromserver) | `Deprecated` |
  | [`InitLicenseFromLicenseContent`](license.md#initlicensefromlicensecontent) | `Deprecated` |
  | [`OutputLicenseToString`](license.md#outputlicensetostring) | `Deprecated` |
  | [`OutputLicenseToStringPtr`](license.md#outputlicensetostringptr) | `Deprecated` |
  | [`FreeLicenseString`](license.md#freelicensestring) | `Deprecated` |
  | [`InitDLSConnectionParameters`](license.md#initdlsconnectionparameters) | `Deprecated` |
  | [`InitLicenseFromDLS`](license.md#initlicensefromdls) | `Deprecated` |
  | [`InitLTSConnectionParameters`](license.md#initltsconnectionparameters) | `Deprecated` |
  | [`InitLicenseFromLTS`](license.md#initlicensefromlts) | `Deprecated` |

   
   
## Decode
   
  | Method               | Description |
  |----------------------|-------------|
  | [`DecodeFile`](decode.md#decodefile) | Decode barcodes from a specified image file. |
  | [`DecodeFileInMemory`](decode.md#decodefileinmemory) | Decode barcodes from an image file in memory. |
  | [`DecodeBuffer`](decode.md#decodebuffer) | Decode barcodes from raw buffer. |
  | [`DecodeBase64String`](decode.md#decodebase64string) | Decode barcodes from a base64 encoded string. |
  | [`DecodeDIB`](decode.md#decodedib) | Decode barcode from a handle of device-independent bitmap (DIB). |
  | [`InitIntermediateResult`](decode.md#initintermediateresult) | Inits an intermediateResult struct with default values. |
  | [`DecodeIntermediateResults`](decode.md#decodeintermediateresults) | Decodes barcode from intermediate results. |
   
   
   
 
## Basic Settings Functions
   
  | Method               | Description |
  |----------------------|-------------|
  | [`SetModeArgument`](parameter-and-runtime-settings-basic.md#setmodeargument) | Set argument value for the specified mode parameter. |
  | [`GetModeArgument`](parameter-and-runtime-settings-basic.md#getmodeargument) | Get argument value for the specified mode parameter. |
  | [`GetRuntimeSettings`](parameter-and-runtime-settings-basic.md#getruntimesettings) | Get current runtime settings. |
  | [`UpdateRuntimeSettings`](parameter-and-runtime-settings-basic.md#updateruntimesettings) | Modify and update the current runtime settings. |
  | [`ResetRuntimeSettings`](parameter-and-runtime-settings-basic.md#resetruntimesettings) | Reset runtime settings to default. |

## Advanced Settings Functions
  
  | Method               | Description |
  |----------------------|-------------|
  | [`InitRuntimeSettingsWithFile`](parameter-and-runtime-settings-advanced.md#initruntimesettingswithfile)  | Initialize runtime settings with the settings in a given JSON file. |
  | [`InitRuntimeSettingsWithString`](parameter-and-runtime-settings-advanced.md#initruntimesettingswithstring) | Initialize runtime settings with the settings in a given JSON string. |
  | [`AppendTplFileToRuntimeSettings`](parameter-and-runtime-settings-advanced.md#appendtplfiletoruntimesettings) | Append a new template file to the current runtime settings. |
  | [`AppendTplStringToRuntimeSettings`](parameter-and-runtime-settings-advanced.md#appendtplstringtoruntimesettings) | Append a new template string to the current runtime settings. |
  | [`GetParameterTemplateCount`](parameter-and-runtime-settings-advanced.md#getparametertemplatecount) | Get the count of the parameter templates. |
  | [`GetParameterTemplateName`](parameter-and-runtime-settings-advanced.md#getparametertemplatename) | Get the parameter template name by index. |
  | [`OutputSettingsToFile`](parameter-and-runtime-settings-advanced.md#outputsettingstofile) | Output runtime settings to a settings file (JSON file). |
  | [`OutputSettingsToString`](parameter-and-runtime-settings-advanced.md#outputsettingstostring) | Output runtime settings to a string. |
  | [`OutputSettingsToStringPtr`](parameter-and-runtime-settings-advanced.md#outputsettingstostringptr) | Output runtime settings to a string. |
  | [`FreeSettingsString`](parameter-and-runtime-settings-advanced.md#freesettingsstring) | Free memory allocated for runtime settings string. |
      
   

   
   
## Result
   
  | Method               | Description |
  |----------------------|-------------|
  | [`GetAllTextResults`](result.md#getalltextresults) | Get all recognized barcode results. |
  | [`FreeTextResults`](result.md#freetextresults) | Free memory allocated for text results. |
  | [`GetIntermediateResults`](result.md#getintermediateresults) | Get intermediate results. |
  | [`FreeIntermediateResults`](result.md#freeintermediateresults) | Free memory allocated for the intermediate results. |
   
      


   
## General
   
  | Method               | Description |
  |----------------------|-------------|
  | [`GetErrorString`](general.md#geterrorstring) | Get error message by error code.|
  | [`GetVersion`](general.md#getversion) | Get version information of SDK.|
  | [`TransformCoordinates`](general.md#transformcoordinates) | Transform the coordinates of a point based on the given transformation matrix. |
  | [`FreeString`](general.md#freestring) | Free memory allocated for string. |
   
      


   
## Video

### Decode
    
   | Method               | Description |
   |----------------------|-------------|
   | [`StartFrameDecoding`](video.md#startframedecoding) | Decode barcodes from inner frame queue. |
   | [`StartFrameDecodingEx`](video.md#startframedecodingex) | Decode barcodes from inner frame queue. |
   | [`AppendFrame`](video.md#appendframe) | Append a frame image buffer to the inner frame queue. |
   | [`StopFrameDecoding`](video.md#stopframedecoding) | Stop thread used for frame decoding. |

### Parameter
   
   | Method               | Description |
   |----------------------|-------------|
   | [`InitFrameDecodingParameters`](video.md#initframedecodingparameters) | Initialize frame decoding parameter. |

### Callback
   
   | Method               | Description |
   |----------------------|-------------|
   | [`SetErrorCallback`](video.md#seterrorcallback) | Set callback function to process errors which is triggered when the library finishes decoding a frame. |
   | [`SetTextResultCallback`](video.md#settextresultcallback) | Set callback function to process text results which is triggered when the library finishes decoding a frame. |
  | [`SetUniqueBarcodeCallback`](video.md#setuniquebarcodecallback) | Set callback function to process text results which is triggered when the library finishes decoding a frame and finds unique barcodes. |
   | [`SetIntermediateResultCallback`](video.md#setintermediateresultcallback) | Set callback function to process intermediate results which is triggered when the library finishes decoding a frame. |

### Status retrieval
   
   | Method               | Description |
   |----------------------|-------------|
   | [`GetLengthOfFrameQueue`](video.md#getlengthofframequeue) | Get length of current inner frame queue. |
 


