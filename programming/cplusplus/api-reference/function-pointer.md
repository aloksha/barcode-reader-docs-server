---
layout: default-layout
title: Dynamsoft Barcode Reader C++ API Reference - Function Pointer
description: This page shows the callbacks of Dynamsoft Barcode Reader for C++ Language.
keywords: CB_Error, CB_IntermediateResult, CB_TextResult, callbacks, api reference, c++
needAutoGenerateSidebar: true
---


# Callbacks

  | Function | Description |
  |----------|-------------|
  | [`CB_Error`](#cb_error) | Represents the method that will handle the error code returned by the SDK. |
  | [`CB_IntermediateResult`](#cb_intermediateresult) | Represents the method that will handle the intermediate result array returned by the SDK. |
  | [`CB_TextResult`](#cb_textresult) | Represents the method that will handle the text result array returned by the SDK. | 

## CB_Error
Represents the method that will handle the error code returned by the SDK.

```c
typedef void(* CB_Error) (int frameId, int errorCode, void* pUser)
```   
   
**Parameters**  
`frameId` 	The ID of the frame.    
`errorCode` Error Code generated when decoding the frame.    
`pUser` Customized arguments passed to your function.   

**See Also**  
[Error Code]({{ site.enumerations }}error-code.html)







## CB_IntermediateResult
Represents the method that will handle the intermediate result array returned by the SDK.

```c
typedef void(* CB_IntermediateResult) (int frameId, IntermediateResultArray* pResults, void* pUser)
```   
   
**Parameters**  
`frameId` 	The ID of the frame.  
`pResults` The intermediate results of the frame.   
`pUser` Arguments passed to your function.   

**See Also**  
[IntermediateResultArray]({{ site.structs }}IntermediateResultArray.html)







## CB_TextResult
Represents the method that will handle the text result array returned by the SDK.

```c
typedef void(* CB_TextResult) (int frameId, TextResultArray *pResults, void *pUser)
```   
   
**Parameters**  
`frameId` 	The ID of the frame.  
`pResults` Recognized barcode results of the frame.   
`pUser` Arguments passed to your function.

**See Also**  
[TextResultArray]({{ site.structs }}TextResultArray.html)




