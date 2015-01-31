## Clean Names

Script takes a csv file with column 'Name' and returns all the columns of the original csv file + 'uniqid', 'FirstName', 'MiddleInitial/Name', 'LastName', 'RomanNumeral', 'Title', 'Suffix'. By default, it takes out duplicate names.  

# License

Scripts are released under the [MIT License](https://github.com/soodoku/Clean-Names/License%20for%20Scripts.md).


# Usage

Main: process_names.py
process_names.py calls names.py

COMMAND LINE OPTIONS
---------------------

Usage: process_names.py [options] <input file>  

Options:
  -h, --help            show this help message and exit  
  -o OUTFILE, --out=OUTFILE  
                        Output file in CSV (default: cfscores_output.csv)  
  -c COLUMN, --column=COLUMN  
                        Column name in CSV that contains Names (default:  
                        Name)  
  -a, --all             Export all names (do not take duplicate names out)  
                        (default: False)  
  
EXAMPLES
--------
   chdir WhereTheScriptsAre  
   python process_names.py -a sample_input.csv   

NOTE
------
   Use the script to fix names in CF-Scores from [Database on Ideology, Money in Politics, and Elections](http://data.stanford.edu/dime).  