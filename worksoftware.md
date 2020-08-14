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

  <h4> &nbsp;&nbsp;&nbsp;&nbsp; :arrow_right: Pandoc </h4>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *A 'swiss army knife' for document conversions, with some limitations on especially pdf (can only convert to and needs another program as engine) - the other CLI tools are all   aimed at pdf due to this limitation*

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The userguide is available [here](https://pandoc.org/MANUAL.html), due to frequent updates the local version is authorative

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Used For Creating / Converting**
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

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  \*(only in specific circumstances, if the other tools don't cut it)


  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Often used commands***

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Create .docx fom website
   > pandoc -f html -t docx https://google.com  -s -o test.docx

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Create one filetype and filename fromt other filetype and filename
   > pandoc -o output.html input.txt

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Control the conversion
   > pandoc -f html -t rtf hello.html

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `-s` is needed to create full fledged "standalone" files (including the headers), otherwise only fragments are produced

  
 <h4> &nbsp;&nbsp;&nbsp;&nbsp; :arrow_right: QPDF </h4>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *Same as CPDF - Mainly unneeded, but has a nice "QDF" mode, which allows editing of .pdf files in an text editor*
  
  <h4> &nbsp;&nbsp;&nbsp;&nbsp; :arrow_right: wkhtmltox </h4>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Mainly used to directly create pdf from websites, also useful as pdfengine for pandoc. The documentation is available [here](https://wkhtmltopdf.org/docs.html)

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Often used commands**

   > wkhtmltopdf http://google.com google.pdf

  <h4> &nbsp;&nbsp;&nbsp;&nbsp; :arrow_right: xpdftools </h4>
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *collection of simple CLI tools to convert pdf in other formats or stripping out information (attachments, images, fonts) from them*

----

### SumatraPDF
*just a simple pdf viewer with reduced functionality - very fast and helpful to checkout **questionable** pdfs*

----

### TexNet32
**TexNet32 provides users with special tools designed to assist in writing conventional abstracts. It is an hybrid abstracting system in which some tasks are performed by human abstractors and others by software**
  
*Kept for historical purposes [Resoomer](https://resoomer.com/en/),[SMMRY](https://smmry.com/) and related online services are preferred to process **public** information* 

