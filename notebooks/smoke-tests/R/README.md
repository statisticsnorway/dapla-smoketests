# R Notebooks

This folder contains notebooks written for the R kernel. Note that **nbval** is unaware of R kernel spesifics such as the the environment variable **R_PROFILE_USER**.
Therefore, this folder contains the file **.Rprofile**, which is automatically picked up by the R environment at startup. This ensures that the SparkR library is loaded and that spark speific functions such as **read.parquet** are available.



