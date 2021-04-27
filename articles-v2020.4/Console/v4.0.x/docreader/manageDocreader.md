# Manage Document Understanding Template

## View Document Understanding Template List

You can view all the document understanding templates under the current resource group in the template list by going to the "Document Understanding" page. The list mainly includes information such as the name of the template, the template release status, and the extraction tag of the current template. A template is mainly used to extract unstructured information from similar documents of that template.

![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader1.png)

## Create Document Understanding Template

New document understanding template click "New" button, in the dialog box to fill in the name of the template, comments, select the built-in model (including electronic PDF extraction model, OCR extraction model) to select the corresponding template file can be completed after the initial creation of template information.

![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader2.png)

## Document Understanding Template

### OCR Document Understanding Template Configuration

The configuration document comprehension template is mainly customized by the user through the visual interface to configure the extraction area of text information, and the user can determine the text area to be extracted by means of a pull box selection.

- **File anchor configuration**
  
  File anchors are used for template matching and skew correction of files, and are determined by clicking on the "gray text area" on the attachment. Anchors must be unchanging text, with no fewer than three anchors per page, the more the better.
  
  ![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader/ocr2.png)

- **Extraction Tag Configuration**
  
  The text area to be extracted can be selected in the attachment display area by pulling the box with the mouse, and a new label will be added automatically for each selected area. Each tag implies an unstructured text extraction area, and the batch extraction process will input the corresponding text content according to the tag.
  
  ![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader/ocr3.png)

- **Label Rendering**
  
  When a tab is clicked, the clicked item is highlighted and the boxed area in the attachment is highlighted. When a tag box is selected, the tag box is highlighted and the corresponding tag is highlighted.

### Electronic PDF Document Understanding Template Configuration

The configuration document comprehension template is mainly customized by the user through the visual interface to configure the extraction area of text information, and the user can determine the text area to be extracted by means of a pull box selection.

- **Extraction Tag Configuration**
  
  The text area to be extracted can be selected in the attachment display area by pulling the box with the mouse, and a new label will be added automatically for each selected area. Each tag implies an unstructured text extraction area, and the batch extraction process will input the corresponding text content according to the tag.
  
  ![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader3.png)

- **Reference Point Configuration**
  
  If the location of the label extraction area in the text is subject to some deviation, new reference points can be added to individual labels to assist in the positioning of the extraction frame when extracting information from new samples. Click the "Reference Point" button, fill in the content of the reference point in the expanded area and select the direction of the reference point
  
  - Up: The reference point is above the label box
  - Down: The reference point is below the label box
  - Left: The reference point is to the left of the label box
  - Right: The reference point is to the right of the label box
  
  ![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader4.png)

- **Label Rendering**
  
  When a tab is clicked, the clicked item is highlighted and the boxed area in the attachment is highlighted. When a tag box is selected, the tag box is highlighted and the corresponding tag is highlighted.

## Test Document Understanding Template

After completing the template configuration, we can check the effect of the template through the test function, click the "Test" button and then upload the files that need to be tested in the dialog box to view the information extraction results of the new sample, and display all the tag items and tag extraction contents in the extraction results page.

![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader5.png)

## Publish Document Understanding Template

If the current template passes the test, you can click the "Action" button on the template configuration page or action options to publish the current template. Once published, the current template service can be [called through the component](../../../Activities/Console/DocReader.md), thus enabling the RPA process to extract a large amount of unstructured text information.

![docreader](https://docimages.blob.core.chinacloudapi.cn/images/Console/docreader6.png)