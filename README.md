This repo contains my RStudio setup.

## .Renviron and .Rprofile

Global options and environment variables settings. Can be edited easily via
```{r}
usethis::edit_r_environ()
usethis::edit_r_profile()
```

## oeli.rstheme

The RStudio appearance I like to work with, based on the [Tomorrow Night ](https://github.com/rstudio/rstudio/blob/master/src/cpp/session/resources/themes/tomorrow_night.rstheme) theme. To setup it up, run:

```{r}
oeli <- "https://raw.githubusercontent.com/loelschlaeger/rstudio_setup/main/oeli.rstheme"
rstudioapi::addTheme(oeli, apply = TRUE, force = TRUE)
```

To remove it, run:

```{r}
rstudioapi::removeTheme("oeli")
```

