---
layout: default-layout
title: FrameDecodingParameters Struct - Dynamsoft Barcode Reader SDK C & C++ Edition
description: This page shows the FrameDecodingParameters struct of Dynamsoft Barcode Reader SDK C & C++ Edition.
keywords: FrameDecodingParameters, struct, c, c++
needAutoGenerateSidebar: false
---


# FrameDecodingParameters
Defines a struct to configure the frame decoding Parameters.  

## Typedefs

```cpp
typedef struct tagFrameDecodingParameters  FrameDecodingParameters
```

---

## Attributes
    
| Attribute | Type |
|---------- | ---- |
| [`maxQueueLength`](#maxqueuelength) | *int* |
| [`maxResultQueueLength`](#maxresultqueuelength) | *int* |
| [`width`](#width) | *int* |
| [`height`](#height) | *int* |
| [`stride`](#stride) | *int* |
| [`imagePixelFormat`](#imagepixelformat) | [`ImagePixelFormat`]({{ site.enumerations }}other-enums.html#imagepixelformat) |
| [`region`](#region) | [`RegionDefinition`](RegionDefinition.md) |
| [`threshold`](#threshold) | *float* |
| [`fps`](#fps) | *int* |
| [`autoFilter`](#autofilter) | *int* |
| [`clarityCalculationMethod`](#claritycalculationmethod) | [`ClarityCalculationMethod`]({{ site.enumerations }}frame-decoding-enums.html#claritycalculationmethod) |
| [`clarityFilterMode`](#clarityfiltermode) | [`ClarityFilterMode`]({{ site.enumerations }}frame-decoding-enums.html#clarityfiltermode) |
| [`reserved`](#reserved) | *char\[20\]* |


### maxQueueLength
The maximum number of frames waiting for decoding.
```cpp
int tagFrameDecodingParameters::maxQueueLength
```
- **Value range**   
    [0,0x7fffffff]   
      
- **Default value**   
    3

### maxResultQueueLength
The maximum number of frames whose results (text result/localization result) will be kept for further reference.  
```cpp
int tagFrameDecodingParameters::maxResultQueueLength
```
- **Value range**   
    [0,0x7fffffff]   
      
- **Default value**   
    10  

### width
The width of the frame image in pixels. 
```cpp
int tagFrameDecodingParameters::width
```
- **Value range**   
    [0,0x7fffffff]   
      
- **Default value**   
    0  

### height
The height of the frame image in pixels.
```cpp
int tagFrameDecodingParameters::height
```
- **Value range**   
    [0,0x7fffffff]   
      
- **Default value**   
    0  

### stride
The stride (or scan width) of the frame image.
```cpp
int tagFrameDecodingParameters::stride
```
- **Value range**   
    [0,0x7fffffff]   
      
- **Default value**   
    0 
      
### imagePixelFormat
The image pixel format used in the image byte array.
```cpp
ImagePixelFormat tagFrameDecodingParameters::imagePixelFormat
```
- **Value range**   
    A value of [`ImagePixelFormat`]({{ site.enumerations }}other-enums.html#imagepixelformat) Enumeration items.
      
- **Default value**   
    `IPF_GRAYSCALED`
    
- **See also**  
    [`ImagePixelFormat`]({{ site.enumerations }}other-enums.html#imagepixelformat)
      
### region
The region definition of the frame to calculate the internal indicator.  
```cpp
RegionDefinition tagFrameDecodingParameters::region
```
- **Default value**  
    `{ regionLeft = 0, regionRight = 100, regionTop = 0, regionBottom = 100, regionMeasuredByPercentage = 1 }`
      
- **See also**   
    [`RegionDefinition`](RegionDefinition.md)
     
### threshold
The threshold used for filtering frames.
```cpp
float tagFrameDecodingParameters::threshold
```
- **Value range**   
    [0, 1]
      
- **Default value**   
    0.01
    
- **Remark**  
    The SDK will calculate an inner indicator for each frame from [`AppendFrame`]({{ site.cpp_methods }}video.html#appendframe) or  [`DBR_AppendFrame`]({{ site.c_methods }}video.html#dbr_appendframe), if the change rate of the indicators between the current frame and the history frames is larger than the given threshold, the current frame will not be added to the inner frame queue waiting for decoding.

### fps
The frequency of calling [`AppendFrame`]({{ site.cpp_methods }}video.html#appendframe) or  [`DBR_AppendFrame`]({{ site.c_methods }}video.html#dbr_appendframe) per second.
```cpp
int tagFrameDecodingParameters::fps
```
- **Value range**   
    [0,0x7fffffff]
      
- **Default value**   
    0  
    
- **Remark**  
    0 means the frequency will be calculated automatically by the SDK.

### autoFilter
Sets whether to filter frames automatically.
```cpp
int tagFrameDecodingParameters::autoFilter
```
- **Value range**   
    [0,1]
      
- **Default value**   
    1  
    
- **Remark**  
    0: Diable filtering frames automatically. 1: Enable filtering frames automatically. 
    

### clarityCalculationMethod
Sets the method used for calculating the clarity of the frames.
```cpp
ClarityCalculationMethod tagFrameDecodingParameters::clarityCalculationMethod
```
- **Value range**   
    Any one of the [`ClarityCalculationMethod`]({{ site.enumerations }}frame-decoding-enums.html#claritycalculationmethod) Enumeration items.   
      
- **Default value**   
    ECCM_CONTRAST   
    
- **See also**  
    [`ClarityCalculationMethod`]({{ site.enumerations }}frame-decoding-enums.html#claritycalculationmethod)    
    

### clarityFilterMode
Sets the mode used for filtering frames by calculated clarity.
```cpp
ClarityFilterMode tagFrameDecodingParameters::clarityFilterMode
```
- **Value range**   
    Any one of the [`ClarityFilterMode`]({{ site.enumerations }}frame-decoding-enums.html#clarityfiltermode) Enumeration items.   
      
- **Default value**   
    CFM_GENERAL   
    
- **See also**  
    [`ClarityFilterMode`]({{ site.enumerations }}frame-decoding-enums.html#clarityfiltermode)    
    

### reserved
Reserved memory for the struct. The length of this array indicates the size of the memory reserved for this struct.
```cpp
char tagFrameDecodingParameters::reserved[28]
```
