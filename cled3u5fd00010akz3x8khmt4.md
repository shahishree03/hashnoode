---
title: "OCR-Optical Character Recognition"
datePublished: Mon Feb 20 2023 17:41:44 GMT+0000 (Coordinated Universal Time)
cuid: cled3u5fd00010akz3x8khmt4
slug: ocr-optical-character-recognition
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1676913392658/fd34aaea-aec5-42ce-b237-321dc16dab92.jpeg
tags: machine-learning, ocr, textrecognition

---

OCR (optical character recognition) is a technology to distinguish printed or handwritten text characters inside digital images of physical documents, such as scanned documents. The basic process of OCR involves examining the text of a document and translating the characters into code that can be used for data processing. It is also called text recognition.

### **Why OCR is used?**

Most businesses involve receiving a bulk amount of information from print media such as paper forms, invoices, scanned legal documents, and printed contracts. These large volumes of paperwork take a lot of time and space to store and manage. Though paperless document management is the way to go, scanning the document into an image creates challenges. The process requires manual intervention and can be tedious and slow.

Moreover, digitizing this document content creates image files with the text hidden within them. Text in images cannot be processed by word processing software in the same way as text documents. OCR technology solves the problem by converting text images into text data that can be analyzed by other business software. We can use the data to conduct analytics, streamline operations, automate processes, and improve productivity.

OCR systems are made up of hardware and software that is used to convert physical documents into machine-readable text. Hardware, such as an optical scanner or specialized circuit board, is used to copy or read text while software typically handles the advanced processing. With the help of AI, Software can implement more advanced methods of intelligent character recognition (ICR), like identifying languages or styles of handwriting.

### **How optical character recognition works**

The first step of OCR is **Image acquisition** where it uses a scanner to process the physical form of a document. Once all pages are copied, OCR software converts the document into a two-color, or black and white, version. The scanned-in image is analyzed for light and dark areas, where the dark areas are identified as characters that need to be recognized and light areas are identified as background.

### **Pre-processing:**

Different fonts and ways to write a single character make this issue a challenge to solve. Before selecting an OCR algorithm, the image must be preprocessed for the image to be ready to be “read”.

**1\. De-skew**  
If the document was not correctly aligned when scanned, it may need to be tilted a few degrees clockwise or anticlockwise to create text lines completely horizontal or vertical.

**2\. Despeckle**  
Remove positive and negative spots, smoothing edges

**3\. Binarization**  
Convert an image to black-and-white (called a “binary image” because there are two colors). The binarization task is conducted as an easy and accurate way to distinguish text (or any other required image element) from the background.

**4\. Line removal**  
Cleans up non-glyph boxes and lines.

**5\. Layout analysis or “zoning”**  
Identifies columns, paragraphs, captions, etc., as blocks. Particularly useful in multi-column layouts and tables.

**6\. Line and word detection**  
Establish word and character shape baseline, and divides words when required.

**7\. Script Recognition**  
In multiple language documents, the script may transform at the word level and therefore script identification is vital before the relevant OCR can be utilized to manage the particular script.

**8\. Character isolation or “segmentation”**  
For OCR characters, various characters linked by image artifacts should be divided, and single characters broken into several artifact-based pieces should be linked.

**9\. Normalization**  
Normalize aspect ratio and scale

### **Text Recognition:**

The two main types of OCR algorithms or software processes that OCR software uses for text recognition are called pattern recognition and feature extraction.

**Pattern recognition**

OCR programs are fed examples of text in various fonts and formats which are then used to compare and recognize, characters in the scanned document.

**Feature detection**

OCR programs apply rules regarding the features of a specific letter or number to recognize characters in the scanned document. When a character is identified, it is converted into an ASCII code that can be used by computer systems to handle further manipulations. Users should correct basic errors, proofread and make sure complex layouts were handled properly before saving the document for future use.

## Post-processing

OCR accuracy can be improved if the output is limited by a lexicon (a list of words permitted in a document). For instance, this could be all the words in English or a more technical lexicon for a particular field.

This method can be less efficient if the document contains words that are not in the lexicon, like proper nouns.

Fortunately, to improve accuracy, there are OCR libraries available online for free. The Tesseract library is using its dictionary to control the segmentation of characters.

The output stream can be a single string or a character file, but more advanced OCR systems retain the original page structure and, for example, create a PDF containing both the original image pages and a searchable textual image.

### **Optical character recognition use cases**

OCR can be used for a variety of applications, including the following:

* Scanning printed documents into versions that can be edited with word processors, like Microsoft Word or Google Docs.
    
* Indexing print material for search engines.
    
* Automating data entry, extraction and processing.
    
* Deciphering documents into text that can be read aloud to visually-impaired or blind users.
    
* Archiving historic information, such as newspapers, magazines or phonebooks, into searchable formats.
    
* Electronically deposit checks without the need for a bank teller.
    
* Placing important, signed legal documents into an electronic database.
    
* Recognizing text, such as license plates, with a camera or software.
    
* Sorting letters for mail delivery.
    
* Translating words within an image into a specified language.
    

### **Benefits of optical character recognition**

The main advantages of OCR technology are the following:

* saves time;
    
* decreases errors;
    
* minimizes effort; and
    
* enables actions that are not possible with physical copies, such as compressing into ZIP files, highlighting keywords, incorporating into a website and attaching to an email.
    

While taking images of documents enables them to be digitally archived, OCR provides the added functionality of being able to edit and search those documents.