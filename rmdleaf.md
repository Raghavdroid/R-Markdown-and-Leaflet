---
  title: "R Markdown and Leaflet"
date: "September 9th 2020"
output: html_document
---
  
  ```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```
#R Markdown and Leaflet
```{r}
library(leaflet)
my_map <- leaflet() %>% addTiles() 
my_map <- my_map %>% addMarkers(lat=11.127123, lng= 78.656891, popup="State")
my_map
```