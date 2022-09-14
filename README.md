# Data-Restructure-for-Performance
Restructuring a very large dataset to work in Kaggle's memory strained environment. We change csv to parquet, we convert strings to int16, floats to int8 for categorical representation, and use multiprocessing to avoid the free list phenomenon and allow Kaggle to reallocate the memory of the 16gb dataset.
