### clear R startup message
cat("\014")

### modify options
options(repos = c(CRAN = "https://cran.rstudio.org"))
options(prompt = "R> ")

### load required packages
if (!require("usethis", quietly = TRUE)) {
  install.packages("usethis") 
}
if (!require("devtools", quietly = TRUE)) {
  install.packages("devtools") 
}

### greeting
cat("Hi Lennart! :-)\n")

### Session infos
cat("R version", paste(R.version[c("major", "minor")], collapse = "."), "\n")
