---
name: Carlos J Catota Valladares
Semester: Fall 23
Course: CIS 106 Linux Fundamentals
---

# Weekly Report 

## 1. cat
**Purpose:** Used for displaying the content of a file.
**Syntax:** `cat + [OPTION] + [file]`
**Examples:** 
- `cat file.txt` 
- `cat file1.txt file2.txt` 
        

## 2.tac

**Purpose:** Similar to cat but displays file content in reverse (last line first).
**Syntax:** `tac [OPTION] + [FILE]`
**Examples:** 
- `tac file.txt`
- `tac file1.txt file2.txt` 
## 3. head
**Purpose:** Outputs the first part of files.
**Syntax:** `head + [OPTION] + [FILE]`
**Examples:** 
- `head file.txt`
- `head -5 file.txt`

## 4. tail
**Purpose:** Outputs the last part of files.
**Syntax:** `tail + [OPTION] + [FILE]`
**Examples:** 
- `tail file.txt`
- `tail -5 file.txt`

## 5. cut
**Purpose:** Removes sections from each line of files.
**Syntax:** `cut + [OPTION] + [FILE]`
**Examples:** 
- `cut  -d':' -f1  file.txt`
- `cut -b 1-5 file.txt`

## 6. paste
**Purpose:** Merges lines of files.
**Syntax:** `paste + [OPTION] + [FILE]`
**Examples:** 
- `paste file1.txt file2.txt`
- `paste -d ',' file1.txt  file2.txt`

## 7. sort
**Purpose:** Sorts lines of text files.
**Syntax:** `sort + [OPTION] + [FILE]`
**Examples:** 
- `sort  file.txt`
- `sort -r file.txt`

## 8. wc
**Purpose:** Prints the number of lines characters and bytes in a file.
**Syntax:** `wc + [OPTION] + [FILE]`
**Examples:** 
- `wc -m file.txt`
- `wc -l file.txt`

## 9. tr
**Purpose:** Translates or deletes characters.
**Syntax:** `tr + [OPTION] + SET1 + [SET2]`
**Examples:** 
- `cat file.txt | tr 'a-z' 'A-Z'`
- `cat file.txt | tr ';' ','`

## 10. diff
**Purpose:** Compares files line by line.
**Syntax:** `diff + [OPTION] + FILES`
**Examples:** 
- `diff file1.txt file2.txt`
- `diff -y file1.txt + file2.txt`

## 11. grep
**Purpose:** Searches for patterns in files.
**Syntax:** `grep + [OPTION] + PATTERN + [FILE]`
**Examples:** 
- `grep + 'love' + file.txt`
- `grep + -i + 'mangu' + file.txt`

## 12. awk
**Purpose:** used for processing and displaying text .
**Syntax:** `awk + [OPTION] + [program] + [input-file]`
**Examples:** 
- `awk '{print $1}' file.txt`
- `awk + '/pattern/ {print $0}' + file.txt`
- `awk + -F: '{print $1, $3}' /etc/passwd`
- `awk + 'NR >1 {print}' + file.txt`
- `awk + '{print length($0)}' file.txt`

## 13. sed
**Purpose:** Stream editor for perform operations on files and standard output.
**Syntax:** `sed + [OPTION] + {script} + [file]`
**Examples:** 
- `sed + 's/cars/automobile/' + file.txt`
- `sed + 5d + file.txt`
- `sed + '12,$d' + file.txt`
- `sed + '/**.md/d' + file.txt`
- `sed + '1,5 s/future/tomorrow/' + file.txt`