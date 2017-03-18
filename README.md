# splitcsv #
Split a CSV file, or any text file, e.g. tab delimited file, that contains column headings as the first line into multiple smaller files with the first line being the column headings.

This script can be useful in importing a subset of a large dataset, or breaking an input into smaller batches.

## Usage ##
	Usage: splitcsv [path] [max lines] [optional prefix]
	
	Arguments:
		path      : the path to the CSV file with the first line being column headings
		max lines : Max number of lines per split file, e.g. 1000
		prefix    : Optional prefix for output files, default value is split_
	
	Split a CSV file that contains column headings as the first line
	into multiple smaller files with the first line being the column headings.
	This script can be useful in importing a subset of a large dataset, or breaking
	an input into smaller batches.
	
	Examples:
	
	splitcsv input.csv 1000
	   Split input.csv into multiple smaller csv files, each no longer
	   than 1000 lines
	
	splitcsv input.csv 200 sub_
	   Split input.csv into multiple smaller csv files, each no longer
	   than 200 lines in length, prefixed with sub_