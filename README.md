## Longest-Compound-Words
Impledge Technologies interview coding test 2025 


The problem statement can be found in the [Exercise_Fresher_Word_Problem.pdf](https://github.com/SoumadipDey/Longest-Compound-Words/blob/main/Exercise_Fresher_Word_Problem.pdf "Exercise_Fresher_Word_Problem.pdf") file.

### Problem Overview  
Compounded words are formed by combining valid words from the same file. Since the file is alphabetically sorted, valid components (prefixes/suffixes) of compounded words appear earlier. A compounded word must entirely consist of valid words without extra characters.

---

### Approach  
1. *Read Words:* Load words from the file into a list and a set for quick lookups.  
2. *Check Compounded Words:*  
   - For each word, split it into prefix and suffix.  
   - If the prefix exists in the set and the suffix can be recursively formed, the word is compounded.  
3. *Find Longest Words:*  
   - Collect all compounded words.  
   - Sort by length to identify the longest and second-longest words.  
4. *Measure Time:* Record the processing time.

---

### Algorithm Steps  
1. Load words from the file.  
2. Use a helper function to validate compounded words via prefix-suffix splitting.  
3. Track the longest and second-longest compounded words.  
4. Return the results along with the processing time.

---

### Example  
For Input_01.txt:
- Words: cat, cats, catsdogcats, dog, rat, ratcatdogcat  
- Longest: catsdogcats  
- Second-longest: ratcatdogcat  

Efficiently finds compounded words using recursion and set lookups
