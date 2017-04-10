
<!-- toc orderedList:0 depthFrom:1 depthTo:6 -->

* [Load data](#load-data)
* [Plot as regular time series](#plot-as-regular-time-series)
* [Default step chart](#default-step-chart)
* [Add labels](#add-labels)

<!-- tocstop -->


# Load data
```{r}
postage <- read.csv("data/us-postage.csv", sep=",", header=TRUE)

```
# Plot as regular time series
```{r}
plot(postage$Year, postage$Price, type="l")

```
# Default step chart
```{r}
plot(postage$Year, postage$Price, type="s")

```
# Add labels
```{r}
plot(postage$Year, postage$Price, type="s", main="US Postage Rates for Letters, First Ounce, 1991-2009", xlab="Year", ylab="Postage Rate (Dollars)")
```
