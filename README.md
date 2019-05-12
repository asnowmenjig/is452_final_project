
## About
My final project for IS452 is a Python program that evaluates the number of Shakespeare citations in each alphabet section of Samuel Johnson's *A Dictionary of the English Language* (1775) (Google-digitized text retrieved from HathiTrust, [catalog record 009310086](<https://catalog.hathitrust.org/Record/009310086>))


## About Johnson's Dictionary
*A Dictionary of the English Language* (1775) is an English-language dictionary written by Samuel Johnson. Johnson sought to produce an evidence-based dictionary by citing literary language use from the writers of his time. Of the cited authors, William Shakespeare is featured most prominently.


## How to Run
First, download the following files from the **is452_Project_FinalVersion** folder or the Moodle submission page:
* johnson\_volume1.txt
* johnson\_volume2.txt

Next, download the following files from the Moodle submission page:
* jmwong5_finalproject_volume1.py (also available as "is452_Project_Final_volume1.ipynb" in the **is452_Project_FinalVersion** folder)
* jmwong5_finalproject_volume2.py (also available as "is452_Project_Final_volume2.ipynb" the **is452_Project_FinalVersion** folder)

Make sure that each .py file is paired together with its corresponding .txt file in the same folder, then execute each program in your preferred interpreter.


## How it Works
This program is split into two files, which correspond with the dictionary's two volumes. Each program takes the Google-digitized text from a volume of Johnson's dictionary and cleans each line of text. The cleaned lines are then split into lists of individual words.

Each unique word and its frequency of occurrence in the text are recorded in a CSV file. The program also keeps count of the number of pages in the current alphabet section as it loops through the text.

When the program detects that the current alphabet section has ended, it evaluates how many times William Shakespeare was cited in the completed section and writes the number of Shakespeare citations and the page count for the section in the volume's respective "counts.txt" file. The program then creates a new CSV file and restarts its count of unique words and pages.

When all the alphabet sections in the given volume have been recorded, the program prints "Complete!" and exits.


## Program Output

The program for Volume 1 (jmwong5_finalproject_volume1.py) should output the following:
* 10 CSV files (Letter\_*\_counts.csv)
  * CSV files containing word counts for their respective letter sections of the dictionary.
* volume\_1\_counts.txt
  * A text file detailing the total page counts and Shakespeare citation counts for volume 1 (letter sections A-K).<sup>1</sup>

The program for Volume 2 (jmwong5_finalproject_volume2.py) should output the following:
* 14 CSV files (Letter\_*\_counts.csv)
  * CSV files containing word counts for their respective letter sections of the dictionary.
* volume\_2\_counts.txt
  * A text file detailing the total page counts and Shakespeare citation counts for volume 2 (letter sections L-Z).<sup>2</sup>


***

#### Notes:

<sup>1</sup> There is no J section count because the I & J sections are combined as one letter section in the original manuscript.

<sup>2</sup> There is no V section count because the U & V sections are combined as one letter section in the original manuscript.
