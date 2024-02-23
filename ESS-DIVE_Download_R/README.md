# Function: `download_and_read_data()`
## Objective
The `download_and_read_data()` function downloads data from [ESS-DIVE](https://data.ess-dive.lbl.gov/data) to a local directory on your computer and then reads the downloaded csv files into R's global environment as a list.
## Directions
1. Source in the function by pasting the following code at the top of your script.

``` R
# Load devtools package
library(devtools)

# Specify the GitHub URL of the script
github_url <- "https://raw.githubusercontent.com/river-corridors-sfa/rcsfa-essdive-api/main/ESS-DIVE_Download_R/script_ess_dive_file_download_function.R"

# Source the script from GitHub
source_url(github_url)
```

2. The `download_and_read_data()` function takes five arguments (3 required, 2 optional):
	- `target_url` = the URL of a specific file you want to download from ESS-DIVE
	- `filename` = the filename of the file you want to download from ESS-DIVE
	- `downloads_folder` = target folder to store the downloaded file
	- `rm_zip` = whether to remove the downloaded zip file after unzipped the file, default is FALSE
	- `rm_unzip_folder`: whether to remove the unzip_folder after reading data into R, default is FALSE

3. See [script_ess_dive_file_download_example.R](https://github.com/river-corridors-sfa/rcsfa-essdive-api/blob/main/ESS-DIVE_Download_R/script_ess_dive_file_download_example.R) for examples on how to use the function.
