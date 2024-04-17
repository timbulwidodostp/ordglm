# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Generalized Linear Ordinal Regression Models Use Package gnlm (ordglm) With (In) R Software
# Ordinal Generalized Linear Models Use Package gnlm (ordglm) With (In) R Software
# Install Generalized Linear Ordinal Regression Models Use Package gnlm (ordglm) With (In) R Software
# Install Ordinal Generalized Linear Models Use Package gnlm (ordglm) With (In) R Software
install.packages("readxl")
install.packages("httr")
install.packages("glm")
install.packages("gnlm")
install.packages("nordr")
library("httr")
library("readxl")
library("glm")
library("gnlm")
library("nordr")
# Import Data Excel Into R From Github Olah Data Semarang (timbulwidodostp)
github_link <- "https://github.com/timbulwidodostp/ordglm/raw/main/ordglm/ordglm.xlsx"
temp_file <- tempfile(fileext = ".xlsx")
req <- GET(github_link, 
# authenticate using GITHUB_PAT
authenticate(Sys.getenv("GITHUB_PAT"), ""),
# write result to disk
write_disk(path = temp_file))
ordglm <- readxl::read_excel(temp_file)
# Estimate Generalized Linear Ordinal Regression Models Use Package gnlm (ordglm) With (In) R Software
ordglm(Test$y~Test$carrier, weights=Test$wt)
# Generalized Linear Ordinal Regression Models Use Package gnlm (ordglm) With (In) R Software
# Ordinal Generalized Linear Models Use Package gnlm (ordglm) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished