CSV Example

Class that provides parsing of comma-separated text files, along with an
example program that uses that class.

Requires Synergy/DE 9.1.3 or greater.

To build, use the batch file bldit.bat.

To run:

dbr CSVExample

On Windows, you may want to use dbs instead of dbr.

The contents of csvfile.txt will be parsed and output to the screen, with
"Next line" indicating the beginning of a new record.

Note that for an alpha field to contain a comma, it must be quoted.
Quoted strings are returned without their quotation marks.

To use the CSVFileParser in your own program, you must import the CSVParser
namespace.  Instantiate a CSVFileParser object, passing it the channel on
which the CSV file is opened.  Then you can call the methods NextLine and
NextWord to parse the data.

Chip Camden
November 14, 2008
