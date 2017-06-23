---
layout: minimal
---

| Link  | Cat Comment  | Location  |  Max's Comments |
|---|---|---|---|
| [Heart of Stowe](https://www.airbnb.com/rooms/2480930)  | `Hey Max... I've had a couple dogs up there in the last few months... Probably 4-5 since January. I don't think I've ever had a cat but I wouldn't want to bet my... Or your friends.... Life on it.`|[Stowe](https://www.google.com/maps/dir//44.4662509,-72.6879696/@44.3541189,-73.0026969,10z)| Best Location<br>Slightly Pricy ($56 each)<br>In a (albeit small) city <br> --------- |
|[Green Mtns](https://www.airbnb.com/rooms/18729679)   |`There was a cat in the apartment in November. Since then we've put in all new carpet and generally re-did the whole place. So, in July it will have been 8 months - - your call. `   | [Hancock](https://www.google.com/maps/dir//Hancock/@44.1886678,-72.9579775,10.07z/data=!4m8!4m7!1m0!1m5!1m1!1s0x89e03f23305a1645:0xfd6f031415eb1195!2m2!1d-72.8412292!2d43.9261192)  | Hour south of the towns<br>Relatively inexpensive<br>Closer to nature (mountains) <br> --------- |



```{r, echo=TRUE}
library(ggplot2)
ggplot(mpg, aes(displ, hwy)) +
  geom_point(aes(color = class)) +
  geom_smooth(se = FALSE, method = "loess") +
  labs(
    title = "Fuel efficiency generally decreases with engine size",
    subtitle = "Two seaters (sports cars) are an exception because of their light weight",
    caption = "Data from fueleconomy.gov"
  )
```