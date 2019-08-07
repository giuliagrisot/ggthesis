This is a Template for a PhD thesis inspired by [the CUED Latex template](https://github.com/kks32/phd-thesis-template) and based on the [Eisvogel template](https://github.com/Wandmalfarbe/pandoc-latex-template).

In order to use it, you will need to have installed:
- R
- Pandoc
- Latex
- MikTex console
- RStudio

# Procedure

1) download the latest version of the ggthesis template (ggthesis.latex) from the repository.
2) Move the template to your pandoc templates folder. The location of the templates folder depends on your operating system:
   - Unix, Linux, macOS: $XDG_DATA_HOME/pandoc/templates or ~/.pandoc/templates/
   - Windows XP: C:\Documents And Settings\USERNAME\Application Data\pandoc\templates
   - Windows Vista or later: C:\Users\USERNAME\AppData\Roaming\pandoc\templates
   
    (If there are no folders called templates or pandoc you need to create them and put the template ggthesis.latex inside.)

3) open your Rmd thesis file with RStudio. For details about the YAML, please see the example.Rmd file
4) Open the Terminal in RStudio (make sure to be inside your working directory, which is the place you want to have your Rmd file)
5) type the following code:

   (<mark>here I use example.Rmd/pdf, but remember to substitute it with YOUR_FILE.Rmd and YOUR_OUTPUT_FILE.pdf</mark>)
  
```
pandoc example.Rmd -s -o example.pdf --template ggthesis --number-sections --bibliography library.bib
```




