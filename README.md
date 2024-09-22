# ABE_detector
ABE detector

<img width="1213" alt="1" src="https://github.com/user-attachments/assets/e5cc0ce8-0d74-487c-a6d9-e84339254def">

This Python script is designed to facilitate the analysis of A-to-G conversion efficiency in NGS data when using ABE and ABE-related tools. You can modify the target_list.txt file to adjust the NGS files to be analyzed and the parameters used.

The first line of target_list.txt includes four parameters:



Minimum_frequency: Sets the minimum offset for each read.

Comparison_range: Sets the indicator distance to pull matching reads.

Indicator_range: Sets the length of the indicator.

Window: Sets the window range displayed in the output file.



Each value is separated by tabs.


From the second line onward, you input the regions you want to analyze. A total of five inputs are required, and each element is separated by tabs:



WT amplicon sequence: Input the WT sequence, excluding the primer binding site (recommended).

Spacer (20nt): Input a 20nt spacer sequence.

NGS folder path: Create a folder within the path and place the NGS files inside it. Then, specify the name of that folder.

Fastqjoin (NGS) file name: This is the name of the NGS file, typically a number determined by the index.

Notes you want to include for the analysis: Leave a note to make the output file easier to distinguish.




The analysis file will be presented as an Excel sheet, with the data displayed on the second sheet (Sheet1).
