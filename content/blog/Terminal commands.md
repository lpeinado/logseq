---

description: Initial description.

author: "@Luigi"
---

- pwd, cd, ls
- whoami
- mkdir another folder
- echo "some content" > file1.txt
- ls -la, cat file1.txt
- cat file1 file2
- less long.txt (quits with q)
- uniq command to output uniq lines
- sort command sorts the file output alf
- wc comand is a wordcount that shows lines, words and chars
- combine the above with pipes ie
	- sort file3 | uniq | wc -c
	- displays the number of unique words in file 3 (sorted, unneeded)
- cat file.txt | grep "b" | wc -l
	- shows the number of lines that contain "b" string
	- cat file.txt | grep "l" | wc -l
- Grep: global search regex and print
	- grep "linu" * | wc -c
	  returns number of words containing "linu" substr in all files of the current directory
- date, uptime, w (dates, users connected, and who is connected)