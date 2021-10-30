This is a bookdown template folked from demo (https://github.com/rstudio/bookdown-demo). The preview of this example can be found at https://bookdown.org/yihui/bookdown-demo/.

Please see the page "[Get Started](https://bookdown.org/yihui/bookdown/get-started.html)" at https://bookdown.org/yihui/bookdown/ for oringinal author's instruction on how to compile this example into **HTML**. 

More detailed instructions are available here https://bookdown.org/yihui/bookdown/build-the-book.html.

Here are the steps for compiling this bookdown template.  
1. Install R (latest version is preferred, I used R version 4.1.1 (2021-08-10) -- "Kick Things")
2. Install R studio (latest version is preferred, I used "Ghost Orchid" Release (077589bc, 2021-09-20) for macOS)   
3. Install the following R packages in R studio. 
   ```{r}
   install.packages("rmarkdown")
   install.packages("bookdown")
   tinytex::install_tinytex()    ## install tinytex package for LaTex
   install.packages("bslib")     ## need to install bslib, downlit, xlm2 for bs4_book() to work  
   install.packages("downlit") 
   install.packages("xml2")
   ```
4. Download the GitHub repository https://github.com/rstudio/bookdown-demo as a Zip file, then unzip it locally.
5. Open the bookdown-demo in RStudio - "File" - "Open Project..." and selecting **bookdown-demo.Rproj**. Then R studio will automatically load this R project. All files in this folder can be found in botton right panel of the R studio dashboard "Files".
6. Load required packages.
   ```{r}
   library(rmarkdown)
   library(bookdown)
   library(tinytex)
   library(bslib)
   library(downlit)
   library(xml2)
   ```
7. Open the R Markdown file **index.Rmd** and click the button **Build Book** on the **Build** tab of RStudio (top right panel)
   
Note:   
Set R studio "Tools" - "Global Options..." - "R Markdown" - "Show output preview in" - "Window", then after clicking **Build Book**, it will automatically open another window with the HTML format book output.   
To generate a copy of the book in **PDF** format, you may input `bookdown::render_book('index.Rmd', 'bookdown::pdf_book')` in R console. 

   
