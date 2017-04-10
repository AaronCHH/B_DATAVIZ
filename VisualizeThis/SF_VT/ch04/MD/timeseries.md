
<!-- toc orderedList:0 depthFrom:1 depthTo:6 -->

* [Load data](#load-data)
* [Default plot](#default-plot)
* [Adjust axis](#adjust-axis)

<!-- tocstop -->


# Load data
```{r}
population <- read.csv("data/world-population.csv", sep=",", header=TRUE)
```
# Default plot
```{r}
plot(population$Year, population$Population, type="l")
```
# Adjust axis
```{r}
plot(population$Year, population$Population, type="l", ylim=c(0, 7000000000), xlab="Year", ylab="Population")
```
