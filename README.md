Sweave --> Rmd converter
===========

To do an initial conversion of vignettes of a package from Rnw to Rmd:

1. Click "Use this template" - "Create a new repository" above
2. Give the new repository the name of the Bioconductor package whose Rnw 
vignettes you would like to convert to Rmd
3. In the new repository, under settings go to "Actions - General" then the section "Workflow permissions"  to select "Allow GitHub Actions to create and approve pull requests"
4. Wait for the GitHub Action of the new repository to finish. If it had already finished before you changed the workflow permissions in step 3, you may have to click on "Actions", click on the failed workflow run, then select re-run failed jobs. 
5. Click on the "Pull requests" tab to merge the pull request created by the GitHub Action. 
6. Check and edit the Rmd vignettes of the new repository until they work
7. Optional: activate GitHub Pages on the new repository; it will already have
pkgdown running in its GitHub Action. (TODO: add details to this step)
