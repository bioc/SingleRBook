all: compiled

compiled: 
	"${R_HOME}/bin/R" -e "work.dir <- rebook::bookCache('SingleRBook'); handle <- rebook::preCompileBook('../inst/book', work.dir=work.dir, desc='../DESCRIPTION'); old.dir <- setwd(work.dir); bookdown::render_book('index.Rmd'); setwd(old.dir); rebook::postCompileBook(work.dir=work.dir, final.dir='../inst/doc/book', handle=handle)"
