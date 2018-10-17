States = rownames(US Arrests)
library(datasets)
View(USArrests)
States = rownames(USArrests)

Get states names with ‘w’.
grep(pattern = "w", States, value = TRUE)
[1] "Delaware"      "Hawaii"        "Iowa"          "New Hampshire" "New Jersey"    "New Mexico"   
[7] "New York"

Get states names with ‘W’.

> grep(pattern = "W", States, value = TRUE)
[1] "Washington"    "West Virginia" "Wisconsin"     "Wyoming"

2. Prepare a Histogram of the number of characters in each US state.
hist(nchar(States), main = paste("Number of characters in each US state"))
