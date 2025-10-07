## Certificate_generator
***Automatic Certificate Generator with Multiple Templates.***


# Automatic Certificate Generator

This project provides a comprehensive solution for automatically generating professional certificates from data. It is designed to be run in a Google Colab or Jupyter Notebook environment and supports multiple templates, data sources, and customization options.

## Overview

The notebook automates the creation of certificates for various purposes like course completion, achievement, or event participation. It can process data in bulk from Excel files or handle single, manual entries. The generated certificates can be saved as individual PNG files, compiled into a single PDF, and packaged in a downloadable ZIP archive.

## Features

*   **Multiple Templates**: Comes with pre-built templates for "Completion," "Achievement," and "Participation," plus functions to create your own custom designs [1].
*   **Flexible Data Input**:
    *   Manually enter data for a single certificate [1].
    *   Bulk-generate from Excel (`.xlsx`) or CSV (`.csv`) files [1].
    *   An interface to upload your own data files directly in the notebook [1].
*   **Customization**:
    *   Easily modify text fields, positions, fonts, and colors within the `CertificateGenerator` class [1].
    *   Programmatically create new certificate templates with unique layouts and color schemes [1].
*   **Output Formats**:
    *   Generates individual certificates in PNG format [1].
    *   Converts and compiles all generated PNGs into a single PDF document [1].
    *   Creates a downloadable ZIP archive containing all generated files (PNGs and PDF) [1].
*   **Environment**:
    *   Fully compatible with Google Colab, including Google Drive integration for file storage [1].
    *   Uses common Python libraries like Pillow, Pandas, and ReportLab [1].

## Installation and Setup

To run the notebook, you first need to install the required Python libraries. The following command is included in the notebook to handle the installation [1]:

```
pip install pillow pandas reportlab openpyxl xlrd
```

The script will also handle the creation of the necessary directory structure within your environment (e.g., in Google Drive) for templates, fonts, data, and output files [1].

## How to Use

The notebook is divided into sequential steps to guide you through the process:

1.  **Installation & Setup**: Run the initial cells to install libraries and mount Google Drive [1].
2.  **Choose a Generation Method**:
    *   **Manual Generation**: Modify the `manualdata` dictionary in the "Manual Certificate Generation" section and run the cell to create a few certificates on the fly [1].
    *   **Bulk Generation from Excel**: Use the sample Excel files provided or upload your own. The script will iterate through each row in the file to generate a certificate [1].
    *   **Upload Custom File**: Use the file upload interface to select your own data file. You will then need to run the processing cell and specify which certificate template to use [1].
3.  **Create PDF and ZIP Archive**: After generating the PNG certificates, run the corresponding cell to compile them into a PDF and create a downloadable ZIP archive [1].
4.  **Download Files**: The final cell provides the option to download the generated ZIP archive directly from the notebook environment [1].

## Customization Guide

You can customize the templates and fields to match your needs:

*   **Editing Existing Templates**: The `CertificateGenerator` class contains a `configs` dictionary where you can adjust the position, size, color, and font for each text field (`PARTICIPANTNAME`, `COURSENAME`, etc.) on the certificates [1].
*   **Creating New Templates**: Use the `createcustomtemplate` function to design new certificate layouts. You can define a name, titles, colors, and a layout style (`standard`, `modern`, `classic`) to generate a new template PNG file [1]. After creating it, you must add its configuration to the `configs` dictionary in the `CertificateGenerator` class to make it usable.
```

[1](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/76397965/90224736-875c-4cb9-b226-b1c0f741fb21/certificate_generator_colab-1.ipynb)
