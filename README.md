# stellae
dataset from exoplanets.org


Try this:
```
stellae %>% 
  ggplot(aes(x = TEFF, y =  MSTAR, color = TEFF)) + 
  geom_point() + 
  scale_x_reverse() + 
  scale_colour_gradient(
    low = "red",
    high = "yellow"
  ) + 
  theme_dark() + 
  labs(
    title = "Temperature and Mass of Stars",
    subtitle = "Stars with known exoplanets",
    x = "Effective Temperature", 
    y = "Solar Masses"
  ) + 
  guides(color = FALSE)
  ```
