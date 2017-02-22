# model-dev-report
SWIM v2.5 Model Development Report

This repository contains the LaTeX code and data used to build the Model Development Report, as well as the current version of the document. It was built using TeXShop Version 3.77 running under macOS Sierra. It compiles using the [standard MacTeX-2016 distribution](https://tug.org/mactex/), and requires no special packages or additional utilities. It creates a single Acrobat Acrobat (.pdf) output file. To create the report follow these steps:

+ Compile `swim25mdr-v37.tex` (found in the root directory of this repository)
+ Find Table 6.8 in the output file `swim25mdr-v37.pdf`, and note the two consecutive page numbers it falls on. Note that there are placeholder graphics on these two pages to make them stand out.
+ Check that the page numbers on the placeholder pages match those in `oversized/oversized.pdf`. If the page numbers are wrong you will need to edit and compile `oversized/oversized.tex` with the correct page numbers set (note that a dummy page precedes the oversized Table 6.8, so `\setcounter{page}{131}` will need to be edited to point to the page before the placeholder begins).
+ Replace the placeholder pages with the second and third pages from `oversized/oversized.pdf` using Preview (macOS), Adobe Acrobat (any operating system), or comparable program. 
+ You can optionally compress the updated `swim25mdr-v37.pdf` using [PDF Compress](https://www.pdfcompress.com) or comparable utility. There is no loss in resolution of the output when using PDF Compress or Adobe Acrobat, but we have noticed that some other programs downgrade the embedded images, making smaller text unreadable. _Caveat emptor_.

The Model Development Report is considered a static document at this point, with the source code provided only for archival purposes. Please contact one of the [tlumip](https://github.com/tlumip) owners before committing changes to the documentation. Questions can be directed to [Rick Donnelly](mailto:rickdonnelly@gmail.com), who edited the submitted report.
