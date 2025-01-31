---
layout: default-layout
title: FurtherModes Struct - Dynamsoft Barcode Reader SDK .NET Edition API Reference
description: This page shows the FurtherModes Struct of Dynamsoft Barcode Reader SDK .NET Edition.
keywords: FurtherModes, struct, api reference, .Net
needAutoGenerateSidebar: false
---


# FurtherModes
Stores the FurtherModes. 

```csharp
public struct FurtherModes
```  

## Attributes
  
| Attribute | Type |
|---------- | ---- |
| [`ColourClusteringModes`](#colourclusteringmodes) | [`EnumColourClusteringMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#colourclusteringmode)[ ] |
| [`ColourConversionModes`](#colourconversionmodes) | [`EnumColourConversionMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#colourconversionmode)[ ] |
| [`GrayscaleTransformationModes`](#grayscaletransformationmodes) | [`EnumGrayscaleTransformationMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#grayscaletransformationmode)[ ] |
| [`RegionPredetectionModes`](#regionpredetectionmodes) | [`EnumRegionPredetectionMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#regionpredetectionmode)[ ] |
| [`ImagePreprocessingModes`](#imagepreprocessingmodes) | [`EnumImagePreprocessingMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#imagepreprocessingmode)[ ] |
| [`TextureDetectionModes`](#texturedetectionmodes) | [`EnumTextureDetectionMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#texturedetectionmode)[ ] |
| [`TextFilterModes`](#textfiltermodes) | [`EnumTextFilterMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#textfiltermode)[ ] |
| [`DPMCodeReadingModes`](#dpmcodereadingmodes) | [`EnumDPMCodeReadingMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#dpmcodereadingmode)[ ] |
| [`DeformationResistingModes`](#deformationresistingmodes) | [`EnumDeformationResistingMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#deformationresistingmode)[ ] |
| [`BarcodeComplementModes`](#barcodecomplementmodes) | [`EnumBarcodeComplementMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#barcodecomplementmode)[ ] |
| [`BarcodeColourModes`](#barcodecolourmodes) | [`EnumBarcodeColourMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#barcodecolourmode)[ ] |
| [`AccompanyingTextRecognitionModes`](#accompanyingtextrecognitionmodes) | [`EnumAccompanyingTextRecognitionMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#accompanyingtextrecognitionmode)[ ] |

### ColourClusteringModes
Sets the mode and priority for colour categorization. Not supported yet.  

```csharp
EnumColourClusteringMode[] Dynamsoft.DBR.FurtherModes.ColourClusteringModes
```

**Value Range**    
   Each array item can be any one of the [`ColourClusteringMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#colourclusteringmode) Enumeration items.  
     
**Default Value**    
   `[EnumColourClusteringMode.CCM_SKIP, EnumColourClusteringMode.CCM_SKIP, EnumColourClusteringMode.CCM_SKIP, EnumColourClusteringMode.CCM_SKIP, EnumColourClusteringMode.CCM_SKIP, EnumColourClusteringMode.CCM_SKIP, EnumColourClusteringMode.CCM_SKIP, EnumColourClusteringMode.CCM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is. 

### ColourConversionModes
Sets the mode and priority for converting a colour image to a grayscale image.

```csharp
EnumColourConversionMode[] Dynamsoft.DBR.FurtherModes.ColourConversionModes
```

**Value Range**    
   Each array item can be any one of the [`ColourConversionMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#colourconversionmode) Enumeration items. 
     
**Default Value**    
   `[EnumColourConversionMode.CICM_GENERAL, EnumColourConversionMode.CICM_SKIP, EnumColourConversionMode.CICM_SKIP, EnumColourConversionMode.CICM_SKIP, EnumColourConversionMode.CICM_SKIP, EnumColourConversionMode.CICM_SKIP, EnumColourConversionMode.CICM_SKIP, EnumColourConversionMode.CICM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.  

### GrayscaleTransformationModes
Sets the mode and priority for the grayscale image conversion.

```csharp
EnumGrayscaleTransformationMode[] Dynamsoft.DBR.FurtherModes.GrayscaleTransformationModes
```

**Value Range**    
   Each array item can be any one of the [`GrayscaleTransformationMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#grayscaletransformationmode) Enumeration items. 
     
**Default Value**    
   `[EnumGrayscaleTransformationMode.GTM_ORIGINAL, EnumGrayscaleTransformationMode.GTM_SKIP, EnumGrayscaleTransformationMode.GTM_SKIP, EnumGrayscaleTransformationMode.GTM_SKIP, EnumGrayscaleTransformationMode.GTM_SKIP, EnumGrayscaleTransformationMode.GTM_SKIP, EnumGrayscaleTransformationMode.GTM_SKIP, EnumGrayscaleTransformationMode.GTM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.  

### RegionPredetectionModes
Sets the region pre-detection mode for barcodes search.

```csharp
EnumRegionPredetectionMode[] Dynamsoft.DBR.FurtherModes.RegionPredetectionModes
```

**Value Range**    
   Each array item can be any one of the [`RegionPredetectionMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#regionpredetectionmode) Enumeration items.  
     
**Default Value**    
   `[EnumRegionPredetectionMode.RPM_GENERAL, EnumRegionPredetectionMode.RPM_SKIP, EnumRegionPredetectionMode.RPM_SKIP, EnumRegionPredetectionMode.RPM_SKIP, EnumRegionPredetectionMode.RPM_SKIP, EnumRegionPredetectionMode.RPM_SKIP, EnumRegionPredetectionMode.RPM_SKIP, EnumRegionPredetectionMode.RPM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is. If the image is large and the barcode on the image is very small, it is recommended to enable region predetection to speed up the localization process and recognition accuracy.

### ImagePreprocessingModes
Sets the mode and priority for image preprocessing algorithms.

```csharp
EnumImagePreprocessingMode[] Dynamsoft.DBR.FurtherModes.ImagePreprocessingModes
```

**Value Range**    
   Each array item can be any one of the [`ImagePreprocessingMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#imagepreprocessingmode) Enumeration items.  
     
**Default Value**    
   `[EnumImagePreprocessingMode.IPM_GENERAL, EnumImagePreprocessingMode.IPM_SKIP, EnumImagePreprocessingMode.IPM_SKIP, EnumImagePreprocessingMode.IPM_SKIP, EnumImagePreprocessingMode.IPM_SKIP, EnumImagePreprocessingMode.IPM_SKIP, EnumImagePreprocessingMode.IPM_SKIP, EnumImagePreprocessingMode.IPM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.

### TextureDetectionModes
Sets the mode and priority for texture detection. 

```csharp
EnumTextureDetectionMode[] Dynamsoft.DBR.FurtherModes.TextureDetectionModes
```

**Value Range**    
   Each array item can be any one of the [`TextureDetectionMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#texturedetectionmode) Enumeration items.  
     
**Default Value**    
   `[EnumTextureDetectionMode.TDM_GENERAL_WIDTH_CONCENTRATION, EnumTextureDetectionMode.TDM_SKIP, EnumTextureDetectionMode.TDM_SKIP, EnumTextureDetectionMode.TDM_SKIP, EnumTextureDetectionMode.TDM_SKIP, EnumTextureDetectionMode.TDM_SKIP, EnumTextureDetectionMode.TDM_SKIP, EnumTextureDetectionMode.TDM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.

### TextFilterModes
Sets the mode and priority for text filter.

```csharp
EnumTextFilterMode[] Dynamsoft.DBR.FurtherModes.TextFilterModes
```

**Value Range**    
   Each array item can be any one of the [`TextFilterMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#textfiltermode) Enumeration items.  
     
**Default Value**    
   `[EnumTextFilterMode.TFM_GENERAL_CONTOUR, EnumTextFilterMode.TFM_SKIP, EnumTextFilterMode.TFM_SKIP, EnumTextFilterMode.TFM_SKIP, EnumTextFilterMode.TFM_SKIP, EnumTextFilterMode.TFM_SKIP, EnumTextFilterMode.TFM_SKIP, EnumTextFilterMode.TFM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is. If the image contains a lot of text, you can enable text filter to speed up the localization process.


### DPMCodeReadingModes
Sets the mode and priority for DPM code reading.

```csharp
EnumDPMCodeReadingMode[] Dynamsoft.DBR.FurtherModes.DPMCodeReadingModes
```

**Value Range**    
   Each array item can be any one of the [`DPMCodeReadingMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#dpmcodereadingmode) Enumeration items.  
     
**Default Value**    
   `[EnumDPMCodeReadingMode.DPMCRM_SKIP, EnumDPMCodeReadingMode.DPMCRM_SKIP, EnumDPMCodeReadingMode.DPMCRM_SKIP, EnumDPMCodeReadingMode.DPMCRM_SKIP, EnumDPMCodeReadingMode.DPMCRM_SKIP, EnumDPMCodeReadingMode.DPMCRM_SKIP, EnumDPMCodeReadingMode.DPMCRM_SKIP, EnumDPMCodeReadingMode.DPMCRM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.  

### DeformationResistingModes
Sets the mode and priority for deformation resisting.

```csharp
EnumDeformationResistingMode[] Dynamsoft.DBR.FurtherModes.DeformationResistingModes
```

**Value Range**    
   Each array item can be any one of the [`DeformationResistingMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#deformationresistingmode) Enumeration items.  
     
**Default Value**    
   `[EnumDeformationResistingMode.DRM_SKIP, EnumDeformationResistingMode.DRM_SKIP, EnumDeformationResistingMode.DRM_SKIP, EnumDeformationResistingMode.DRM_SKIP, EnumDeformationResistingMode.DRM_SKIP, EnumDeformationResistingMode.DRM_SKIP, EnumDeformationResistingMode.DRM_SKIP, EnumDeformationResistingMode.DRM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.  

### BarcodeComplementModes
Sets the mode and priority to complement the missing parts in the barcode.

```csharp
EnumColourConversionMode[] Dynamsoft.DBR.FurtherModes.ColourConversionModes
```

**Value Range**    
   Each array item can be any one of the [`BarcodeComplementMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#barcodecomplementmode) Enumeration items.  
     
**Default Value**    
   `[EnumColourConversionMode.BCM_SKIP, EnumColourConversionMode.BCM_SKIP, EnumColourConversionMode.BCM_SKIP, EnumColourConversionMode.BCM_SKIP, EnumColourConversionMode.BCM_SKIP, EnumColourConversionMode.BCM_SKIP, EnumColourConversionMode.BCM_SKIP, EnumColourConversionMode.BCM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.  

### BarcodeColourModes
Sets the mode and priority for the barcode colour mode used to process the barcode zone.

```csharp
EnumBarcodeColourMode[] Dynamsoft.DBR.FurtherModes.BarcodeColourModes
```

**Value Range**    
   Each array item can be any one of the [`BarcodeColourMode`]({{ site.dotnet_enumerations }}parameter-mode-enums.html#barcodecolourmode) Enumeration items.  
     
**Default Value**    
   `[EnumBarcodeColourMode.BICM_DARK_ON_LIGHT, EnumBarcodeColourMode.BICM_SKIP, EnumBarcodeColourMode.BICM_SKIP, EnumBarcodeColourMode.BICM_SKIP, EnumBarcodeColourMode.BICM_SKIP, EnumBarcodeColourMode.BICM_SKIP, EnumBarcodeColourMode.BICM_SKIP, EnumBarcodeColourMode.BICM_SKIP]`  
     
**Remarks**      
   The array index represents the priority of the item. The smaller index is, the higher priority is.  

### AccompanyingTextRecognitionModes
[`Deprecated`]Sets the mode and priority to recognize accompanying text.

```csharp
EnumAccompanyingTextRecognitionMode[] Dynamsoft.DBR.FurtherModes.AccompanyingTextRecognitionModes
```
