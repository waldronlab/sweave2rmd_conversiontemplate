# Sweave to Rmd Converter
===========

To convert vignettes of a package from Rnw to Rmd, follow these steps:

1. Click on "Code" and select "Download Zip" above.
2. Extract the zip folder from the downloaded file.
3. Fork the new repository of the Bioconductor package containing the
   Rnw vignettes you wish to convert to Rmd.
4. Clone the repository of the Bioconductor package onto your local
   computer terminal.
5. Copy and paste the `.GitHub` folder from the conversion template
   into the cloned repository of the package you want to convert and
   then commit and push .Github file in the colned repository.
7. In the cloned repository, go to "Settings" and then "Actions - General." Under the "Workflow permissions" section, select:
    - "Read and write permissions"
    - "Allow GitHub Actions to create and approve pull requests"
8. Click on "Actions" and choose "Re-run all jobs."
9. Once the GitHub Action has finished (approximately 3 minutes), navigate to
   the "Pull requests" tab and merge the pull request it created.
   NOTE: Take note of the comments in the pull request, as they will provide information
   about which `.Rnw` files have been converted and which files need to be converted manually.
11.  After merging the pull request, create a new branch using the command `git switch -c file-Rmd`
     for the file you wish to create a pull request for. Follow the steps outlined in the [contribute](https://bioconductor.github.io/sweave2rmd/articles/contribute.html) document to make the pull request.
13. Make a pull request for the converted file and tag `@Bioconductor/sweave2rmd` and the maintainer of the package for review.
15. Optional: Activate GitHub Pages on the new repository. It will already have `pkgdown` running in its GitHub Action. (TODO: Add `pkgdown` Action and instructions).
