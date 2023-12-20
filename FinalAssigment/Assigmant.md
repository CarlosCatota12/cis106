---
name: Carlos J Catota Valladares
Semester: Fall 23
Course: CIS 106 Linux Fundamentals
---
# Question 1

## For every command in this list, include the following:

Description
formula/syntax
3 examples that you understand well


### awk
awk used for processing and displaying text 

*awk + options + {awk command} + file + file to save*
  
awk '{print $2,$3}' ~/Documents/Books/bible.txt

awk 'NR > 5 {print}' ~/Documents/Books?dracula.txt

awk '{print $NF}' ~/Documents/homework.txt 


### cat
cat is used fos displaying the content of a file

*cat + option + File to display*

cat -n bible.txt

cat -bn dracula.txt bible.txt

cat -s bible.txt

### cp

cp c0pies files/directories from a source to a destination 
*cp + files to copy + destination*

cp Downloads/cars.txt Documents/

cp -r cis106/ Documents/Linux/

cp Downloads/* ~/pictures/

### cut
cut extract a specific section of each line of a file and displaying it to the screen 

*cut + option + file*
  
cut -b 1-10 bible.txt

cut -d ':' -f1,7 --output-delimiter=',' /etc/passwd

cut -d ':' --complement -s -f5 /etc/passwd/


### grep

grep is used to search text in given file. 

*grep + option + search criteria + file*

grep -c bin/bash /etc/passwd

grep amen ~/Documents/Books/bible.txt

grep -in 'dracula' ~/Documents/Books/dracula.txt

### head
head displays the top N number of lines of a file
by default prints 10 lines
*head + option + file*

head ~/Documents/books/bible.txt

head -5 bible.txt 

head dracula.txt


### ls
-ls is used for listing the contend of a given directory.

*ls + option + directory to list*

ls -al /Downloads 

ls -Ggh

ls -l --time-style=iso


### man
mas describe commands, linux shell, executable programs, etc
 
*man + comman*

man ls

man pwd

man vim

### mkdir

*mkdir + name of the directory*

-mkdir is used for create directories

mkdir ~/Downloads/games

mkdir -p ~/Wallpapers/Principal/cars

mkdir downloads/games wallpapers/cars music/rap


### mv

-mv moves and renames directories 

*mv + source + destination*
*mv + file/directory to rename + new name*

mv Downloads/file1.txt Documents/

mv cars.txt toyota.txt

mv Downloads/file1.txt Downloads/file2.txt Documents/



### tac
tac is used for displaying the content of a file in reverse mode 

*tac + option + file*

tac -n bible.txt

tac -bn dracula.txt bible.txt

tac -s bible.txt


### tail
tail is used for displaying the last 10 lines of a file

*tail + option + file*

tail ~/Documents/books/bible.txt

tail -5 bible.txt 

tail dracula.txt


### touch

*touch + file name*

-touch is used for creating files

touch Downloads/cars.txt Music/rap.mp3

touch ~/Videos/carlos.mp4

touch "carlos 9.txt"


### tr

tr is used for translating or deleting characters from standard output 

*standard output | tr + option + set + set*

cat file.txt | tr '.' ','

cat /etc/passwd | tr ':' '/'

cat bible.txt | tr "[:space:]" '\t'



### tree

used for displaying the directory structure of a file system in a tree-like format.

*tree + option + Directory*

tree -a Documents/

tree -d Documents/

tree ~/Music/

### How to work with multiple terminals open?
Using tilix there is and option to add terminals 

### How to work with manual pages?
Use man [command] to access the manual page for a command.
for example *man ls*

### How to parse (search) for specific words in the manual page

first initiated man then press '/' and type the word that you are looking for.

### How to redirect output (> and |)

Using '>' will save the output of the command in a given file for example

ls > files.txt will write the output od ls inside od files.txt

Using '|' pass output as input to anoither command 
for example
 ls | grep "test" filters the output of ls for lines containig 'test'

### How to append the output of a command to a file

Using >> we can append output 
for example 
echo 'new line' >> file.txt  will add "new line" to the end of file.txt

### How to use wildcards 

cp ??*txt /destination/folder/
mv file[1-9]*.txt /destination/folder/ 

### How to use brace expansion 
Brace expansion is useful for creating complex directory structures efficiently. For example, mkdir -p project/{src,bin,docs/{html,pdf},tests} will create a project directory with subdirectories src, bin, docs (and further subdirectories html and pdf under docs), and tests

