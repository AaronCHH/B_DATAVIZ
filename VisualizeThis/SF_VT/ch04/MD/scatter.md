
<!-- toc orderedList:0 depthFrom:1 depthTo:6 -->

* [Load data](#load-data)
* [Default plot with points](#default-plot-with-points)
* [Default plot with type explicity specified](#default-plot-with-type-explicity-specified)
* [Draw vertical lines](#draw-vertical-lines)
* [Draw points with above lines](#draw-points-with-above-lines)
* [Edits with colors and labels](#edits-with-colors-and-labels)

<!-- tocstop -->


# Load data
```{r}
subscribers <- read.csv("data/flowingdata_subscribers.csv", sep=",", header=TRUE)

```
# Default plot with points
```{r}
plot(subscribers$Subscribers)

```
# Default plot with type explicity specified
```{r}
plot(subscribers$Subscribers, type="p", ylim=c(0, 30000))

```
# Draw vertical lines
```{r}
plot(subscribers$Subscribers, type="h", ylim=c(0, 30000))

```
# Draw points with above lines
```{r}
plot(subscribers$Subscribers, type="h", ylim=c(0, 30000))
points(subscribers$Subscribers)
```
# Edits with colors and labels
```{r}
plot(subscribers$Subscribers, type="h", ylim=c(0, 30000), xlab="Day", ylab="Subscribers")
points(subscribers$Subscribers, pch=19, col="black")
```
