# autocad-use-count
Powershell script that will output how many times a user used AutoCAD each month (with year)  

This script helps the company decide how many AutoCAD licenses it actually needs, based on how many times the employees use the software and if it's worth to buy (amount)

> Coding language: English | EN  
> User displayed language: Portuguese | PT

### To run this script you will need a .log file with the TIMESTAMPs (AutoCAD)
The script will then look for file named "autocad.log" located in the same folder as the script, after executing the script it save the output in a CSV file named "outfile.csv", that is also located in the root.

This filters the .log file from endian by removing double and empty TIMESTAMPs leaving only the important ones, then saves two lists, one is the filtered and the other is with unique words (names, dates, timestamps), as so to make comparisons for counting uses and then saving it in an array (name, uses, month). It also then converts the date from american to european.  

The last loop will ready up the output to be easy to read.
