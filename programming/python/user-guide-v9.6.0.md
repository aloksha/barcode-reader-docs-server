---
layout: default-layout
title: User Guide - Dynamsoft Barcode Reader SDK Python Edition
description: This is the user guide of Dynamsoft Barcode Reader SDK Python Edition.
keywords: user guide, python
needAutoGenerateSidebar: true
needGenerateH3Content: true
noTitleIndex: true
---

# Getting Started with Dynamsoft Barcode Reader Python Edition

In this guide, you will learn step by step on how to build a barcode reading application with Dynamsoft Barcode Reader (DBR) SDK using Python.

## System Requirements

- Operating Systems:
  - Windows x64
  - Linux (x64, ARM32, ARM64)
  - macOS (10.15+)

- Python Versions:
  - Python 3.10
  - Python 3.9
  - Python 3.8
  - Python 3.7
  - Python 3.6
  - Python 3.5 (for versions below DBR 7.5)
  - Python 2.7 (for versions below DBR 7.2.2.3)

>Note:
>Dynamsoft Barcode Reader provides both online and offline license options. The online license option might not work in an environment that doesn't have network connection or some environments like AWS Lambda. In such case, you can get an offline trial license key via <a href="https://www.dynamsoft.com/customer/license/trialLicense?utm_source=guide&product=dbr&package=desktop" target="_blank">Customer Portal</a> or by <a href="https://www.dynamsoft.com/company/contact/" target="_blank">contacting us</a>.

<iframe width="400" height="225" src="https://www.youtube.com/embed/6uPP3siJJlU" title="How to Use Dynamsoft Barcode Reader Python SDK | Dynamsoft Tutorial" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Installation

Start terminal or command prompt to run the following command:

```
pip install dbr
```

## Build Your First Application

Let's start by creating a console application which demonstrates how to use the minimum code to read barcodes from an image file.  
> You can <a href="https://github.com/Dynamsoft/barcode-reader-python-samples/blob/master/samples/general-settings.py" target="_blank">download the entire source code here</a>.

### Create a New Project

Create a new source file named `DBRPythonSample.py`.

### Include the Library

Import dbr package in the source file.

   ```python
   from dbr import *
   ```

### Initialize a Barcode Reader Instance

1. Initialize the license key.

   ```python
   BarcodeReader.init_license("<insert DBR license key here>")
   ```

    > Please replace `<insert DBR license key here>` with a valid DBR license key. You can request a free trial from <a href="https://www.dynamsoft.com/customer/license/trialLicense?utm_source=guide&product=dbr&package=desktop" target="_blank">Customer Portal</a>.

2. Create an instance of Dynamsoft Barcode Reader.

   ```python
   reader = BarcodeReader()
   ```

### Configure the Barcode Scanning Behavior

DBR provides multiple APIs for you to customize the barcode scanning behavior. Here we set the barcode format and barcode count to read.

   ```python
   settings = reader.get_runtime_settings()
   settings.barcode_format_ids = EnumBarcodeFormat.BF_ALL
   settings.barcode_format_ids_2 = EnumBarcodeFormat_2.BF2_POSTALCODE | EnumBarcodeFormat_2.BF2_DOTCODE
   settings.excepted_barcodes_count = 10
   reader.update_runtime_settings(settings)
   ```

> For better performance, we recommend that you only enable the barcode formats your application requires. Check out [Barcode Format Enumeration]({{ site.python_enumerations }}format-enums.html) for fully supported barcode formats.

> If you know exactly the count of barcodes you want to read, specify `excepted_barcodes_count` to speed up the process and improve the accuracy. 

### Decode and Output Results

1. Decode barcodes from an image file.
2. Get and output barcode results.

   ```python
   try:
      image_path = r"[INSTALLATION FOLDER]/Images/AllSupportedBarcodeTypes.png"
      results = reader.decode_file(image_path)
      if results != None:
         i = 0
         for text_result in results:
            print("Barcode " + str(i))
            print("Barcode Format : " + text_result.barcode_format_string)
            print("Barcode Text : " + text_result.barcode_text)
            i = i+1
   except BarcodeReaderError as bre:
      print(bre)
   ```

   > For the error handling mechanism, the SDK throws [BarcodeReaderError]({{site.python_class}}BarcodeReaderError.html) for each function. You can add code for exception handling based on your needs. 

   > The SDK returns multiple barcode information items, including barcode count, barcode format, barcode text, location, barcode raw data, etc. Check out [TextResult]({{ site.python_class }}TextResult.html) for fully supported result data.

### Release Resource

Destroy the instance to release all resources.

```python
del reader
```

### Build and Run the Project

1. Start terminal or command prompt and change to the target directory where `DBRPythonSample.py` located in.
2. Run the sample

```
python DBRPythonSample.py
```

> You can <a href="https://github.com/Dynamsoft/barcode-reader-python-samples/blob/master/samples/general-settings.py" target="_blank">download the entire source code here</a>.

## Next Steps

- Learn [How to Upgrade to Latest Version](upgrade-instruction.md)
- [Explore SDK Features](user-guide/explore-features/index.md)
- See how the SDK works in [Popular Use Cases](user-guide/use-cases/index.md)
- Check out the [Official Samples and Demo](samples/index.md)