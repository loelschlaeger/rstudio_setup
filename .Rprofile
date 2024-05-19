### clear R startup message
cat("\014")

### modify options
options(repos = c(CRAN = "https://cran.rstudio.org"))
options(prompt = "R> ")

### greeting
message("Hi Lennart! :-)")
message("Your path is ", getwd(), ".")
message("You use R version ", paste(R.version[c("major", "minor")], collapse = "."), ".")

### packages
if (interactive()) {
  if (suppressWarnings(!require("utils", quietly = TRUE))) {
    install.packages("utils")
  }
  if (file.exists("renv/activate.R")) {
    message("You use renv. Activate it?")
    if (utils::menu(c("yes", "no")) == 1) {
      source('renv/activate.R')
    }
  }
  if (suppressWarnings(!require("usethis", quietly = TRUE))) {
    message("You want to install usethis?")
    if (utils::menu(c("yes", "no")) == 1) {
      renv::install("usethis", prompt = FALSE)
    }
  }
  if (suppressWarnings(!require("devtools", quietly = TRUE))) {
    message("You want to install devtools?")
    if (utils::menu(c("yes", "no")) == 1) {
      renv::install("devtools", prompt = FALSE)
    }
  }
}

