# Analyzing the Book: "The Fault in Our Stars"

## Project Overview
This project analyzes the text file 'faultinourstars.txt', which contains the complete text of "The Fault in Our Stars" by John Green. The primary objective of this analysis is to identify the main characters in the book.

## Steps in the Analysis
### 1. Reading in the File
<img width="374" alt="image" src="https://github.com/obinna-nweke/the-fault-in-our-stars-analysis/assets/152950827/1b9b1e0f-fd3a-40d4-b67f-883786752573">

### 2. Counting Word Frequency
Here, we count the frequency of each word line by line.
[('I', 2542),
 ('Augustus', 297),
 ('He', 253),
 ('The', 202),
 ('Gus', 146),
 ('It', 135),
 ('Isaac', 133),
 ('But', 131),
 ('Mom', 131),
 ('Van', 113),
 ('I’d', 111),
 ('And', 100),
 ('I’m', 97),
 ('Houten', 96),
 ('Hazel', 88),
 ('We', 87),
 ('She', 80),
 ('You', 76),
 ('My', 66),
 ('Peter', 61),
 ('A', 59),
 ('Waters', 57),
 ('Dad', 57),
 ('Lidewij', 57),
 ('CHAPTER', 50)]

### 3. Excluding Common Words
We exclude common sentence-starting words that are not character names.
[('Augustus', 297),
 ('Gus', 146),
 ('Isaac', 133),
 ('Mom', 131),
 ('Van', 113),
 ('Houten', 96),
 ('Hazel', 88),
 ('Peter', 61),
 ('Waters', 57),
 ('Dad', 57),
 ('Lidewij', 57),
 ('Gus’s', 46),
 ('After', 44),
 ('Amsterdam', 42),
 ('There', 41),
 ('Group', 40),
 ('Support', 37),
 ('Imperial', 35),
 ('God', 34),
 ('Dutch', 32),
 ('Patrick', 30),
 ('Grace', 30),
 ('Affliction', 29),
 ('When', 28),
 ('Kaitlyn', 26)]

### 4. Updating Excluded Words
We identify and exclude additional non-character words.
[('Augustus', 546),
 ('Van Houten', 209),
 ('Isaac', 133),
 ('Mom', 131),
 ('Hazel Grace', 118),
 ('Peter', 61),
 ('Dad', 57),
 ('Lidewij', 57),
 ('After', 44),
 ('Amsterdam', 42),
 ('There', 41),
 ('Group', 40),
 ('Support', 37),
 ('Imperial', 35),
 ('God', 34)]

### 5. Combined Count of First and Last Names of Characters
We also notice that the first and last names of the same individuals are counted separately, so we need to combine them and count them together:

name_mapping = {
    'Gus': 'Augustus',
    'Waters': 'Augustus',
    'Gus’s': 'Augustus',
    'Grace': 'Hazel Grace',
    'Hazel': 'Hazel Grace',
    'Van': 'Van Houten',
    'Houten': 'Van Houten',
}


### 6. Identifying Top Characters
We extract the top main characters from the filtered list.

{'Augustus': 546,
 'Van Houten': 209,
 'Isaac': 133,
 'Mom': 131,
 'Hazel Grace': 118}

### 6. Visualization Using Seaborn
![image](https://github.com/obinna-nweke/the-fault-in-our-stars-analysis/assets/152950827/beb2cd5d-a5e6-48f5-8a91-b2cce613f6fa)



### 7. Result Interpretation
The bar plot shows the top 10 most mentioned characters in "The Fault in Our Stars." Compare this list to the characters you recognize from the movie adaptation.
![image](https://github.com/obinna-nweke/the-fault-in-our-stars-analysis/assets/152950827/dcac1377-09c1-4015-9f41-69ee018a52c1)


## Conclusion
By following the above steps, we have successfully identified and visualized the top 10 main characters in "The Fault in Our Stars" based on their mention frequency.

## Files
- faultinourstars.txt: Contains the text of the book "The Fault in Our Stars" by John Green.
- Movie Cover Image: Poster of the movie adaptation of the book.

## Author
Obinna Nweke






