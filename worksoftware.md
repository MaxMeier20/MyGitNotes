# Work Software

## CALC
## GRPH
## INET
## MLTM
## PACK
## PRJT
## SECR
## SYST
## WRDS
----
### CLI Tools

   <h4> &nbsp;&nbsp;&nbsp;&nbsp; :arrow_right: CPDF </h4>

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *Mainly unneeded - does all the things a full blown pdf editor does (encrypting, merging, resizing, splitting...) via the CLI*

  ####  Pandoc
   *A 'swiss army knife' for document conversions, with some limitations on especially pdf (can only convert to and needs another program as engine) - the other CLI tools are all   aimed at pdf due to this limitation*

   The userguide is available [here](https://pandoc.org/MANUAL.html), due to frequent updates the local version is authorative

   **Used For Creating / Converting**
   to    | from
   ----- | -----
   .docx |  .csv
   .epub | .docx
   .html | .epub
   .odt | .html
   .pptx | .odt
   .rtf | .txt
   .txt |
   .pdf\* | 

   \*(only in specific circumstances, if the other tools don't cut it)


   **Often used commands***

   Create .docx fom website
   > pandoc -f html -t docx https://google.com  -s -o test.docx

   Create one filetype and filename fromt other filetype and filename
   > pandoc -o output.html input.txt

   Control the conversion
   > pandoc -f html -t rtf hello.html

   `-s` is needed to create full fledged "standalone" files (including the headers), otherwise only fragments are produced

  
  #### :arrow_right: QPDF
   *Same as CPDF - Mainly unneeded, but has a nice "QDF" mode, which allows editing of .pdf files in an text editor*
  
  ####  :arrow_right: wkhtmltox
   Mainly used to directly create pdf from websites, also useful as pdfengine for pandoc. The documentation is available [here](https://wkhtmltopdf.org/docs.html)

  **Often used commands**

   > wkhtmltopdf http://google.com google.pdf

  #### :arrow_right: xpdftools
   *collection of simple CLI tools to convert pdf in other formats or stripping out information (attachments, images, fonts) from them*

----

### SumatraPDF
*just a simple pdf viewer with reduced functionality - very fast and helpful to checkout **questionable** pdfs*

----

### TexNet32
**TexNet32 provides users with special tools designed to assist in writing conventional abstracts. It is an hybrid abstracting system in which some tasks are performed by human abstractors and others by software**
  
*Kept for historical purposes [Resoomer](https://resoomer.com/en/),[SMMRY](https://smmry.com/) and related online services are preferred to process **public** information* 

