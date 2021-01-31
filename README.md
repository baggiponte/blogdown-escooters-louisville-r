# Static Website for [`escooters-louisville-r`](https://github.com/baggiponte/escooters-louisville-r)

[![Netlify Status](https://api.netlify.com/api/v1/badges/fbe5de82-c0d4-446a-99dd-630e67a67441/deploy-status)](https://app.netlify.com/sites/louisville-dockless-vehicles/deploys)

This is the repo connected to `netlify` with the source material for the static website create with `blogdown` and `hugo` for the content in the omonimous repo [escooters-louisville-r](https://github.com/baggiponte/escooters-louisville-r).

The `.Rmarkdown` notebooks are published is in the directory [`/content/post`](https://github.com/baggiponte/blogdown-escooters-louisville-r/tree/main/content/post).

## Libraries for Machine Learning

I have almost relied entirely on [`tidymodels`](https://github.com/tidymodels/tidymodels).
I have also made a [repository](https://github.com/baggiponte/learn-tidymodels) to reproduce some basic tutorials with this framework:
you can find the originals [here](https://www.tidymodels.org/start/).

## The data

The original raw data can be obtained from [here](https://data.louisvilleky.gov/dataset/dockless-vehicles).

I did some preprocessing in Python, which you can find [here](https://github.com/baggiponte/escooters-louisville-python). I basically used it for two things:
a starting data cleaning to get deal with mislabelled observations and then used [`geopandas`](https://geopandas.org/) to intersect the data with a shapefile of the city.

## Quick Table of Contents

The articles are presented as follows:

1. **Exploratory Data Analysis**.
2. **Some Advanced Visualisations** using `{circlize}` and `{ggalluvial}`.
3. **Final Feature Engineering**: creating the final dataset that will be used.
3. **Multinomial Logistic Regression**.
4. **Decision Tree**.
5. **K-means and Hierarchical Clustering**.
6. **Final Considerations** on what is missing and how I felt using Tidymodels.

## Credits

The theme used is the elegant [`PaperMod`](https://github.com/adityatelange/hugo-PaperMod).

Please make sure to check out [`blogdown`](https://bookdown.org/yihui/blogdown/) and [`tidymodels`](https://www.tidymodels.org)!
