# Data.gov Index Dump
I was wanting to map out, assess, and work with a variety of the government data indexed at data.gov. I didn't want to be hitting CKAN API behind the site to slice and dice the data I wanted, and wanted to establish a separate cached index of data.gov--for whatever might happen in the next administration

The quickest and most complete way to pull a copy of the data.gov index was to pull the list of all the tags (https://catalog.data.gov/api/3/action/tag_list), then slow drip the API calls for all the tags, pulling and saving the JSON for all available data packages. To be clear, I am not pulling the data at th emoment. This is just the data inventory index, each data resource has the details about where this data is located, and other meta data about the resource in each JSON file.

I put all 127,836 packages I pulled in the packages folder for this Github repository. All I did was pull the results and saved each package, using its unique id for the file name. I will be using this repo as a cached copy of data.gov, driving a variety of projects. I will re-run the pull scripts each month, keeping it as up to date as possible.

You can submit any questions, comments, and concerns via the Github issues for the project, or ping me @kinlane.com.
