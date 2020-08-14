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

### CLI Tools

#### Pandoc
*A 'swiss army knife' for document conversions, with some limitations on especially pdf (can only convert to and needs another program as engine) - the other CLI tools are all aimed at pdf due to this limitation*

The userguide is available [here](https://pandoc.org/MANUAL.html), due to frequent updates the local version is authorative

**Used For Creating**
* .docx
* .epub
* .html
* .odt
* .pptx
* .rtf
* .txt

~~.pdf~~ (only in specific circumstances, if the other tools don't cut it)

**from**
* .csv
* .docx
* .epub
* .html
* .odt

**Often used commands***

Create .docx fom website
> pandoc -f html -t docx https://google.com  -s -o test.docx

Create one filetype and filename fromt other filetype and filename
> pandoc -o output.html input.txt

Control the conversion
> pandoc -f html -t rtf hello.html

`-s` is needed to create full fledged "standalone" files (including the headers), otherwise only fragments are produced

####  wkhtmltox
Mainly used to directly create pdf from websites, also useful as pdfengine for pandoc. The documentation is available [here](https://wkhtmltopdf.org/docs.html)

**Often used commands**

> wkhtmltopdf http://google.com google.pdf
