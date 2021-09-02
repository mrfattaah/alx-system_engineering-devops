0.echo Hello, World: prints "Hello, World" followed by a new line to the standard output
1.echo "\"(Ôo)'": display a confused smiley "(Ôo)'
2.cat /etc/passwd: display the content of the /etc/passwd
3.cat /etc/passwd /etc/hosts: display the contents of /etc/passwd and /etc/hosts
4.tail -n 10 /etc/passwd: display the last ten lines of /etc/passwd
5.head -n 10 /etc/passwd: display the first ten lines of /etc/passwd
6.head -n 3 iacta | tail -n 1: displays the third line of the file iacta
7.echo "Best School" > \*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:): creates a file \*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:) with Best School is inside
8.ls -la > ls_cwd_content: writes  into the file ls_cwd_content. it also creates a file
9.echo -en "" | tail --lines=1 iacta >> iacta: duplicates the last line of the file iacta
10.find . -name '*.js' -type f -delete: deletes all the regular files (not the directories) with a js extension that are present in the current directory and all its subfolders
11.find -mindepth 1 -type d | wc -l: writes script that counts the number of directories and sub directories in the current directory
12.ls -t | head: create a script that displays the 10 newest files in the current directory, one file per file and sorted from the newest to the oldest
13.sort | uniq -u: creates a script that takes a list of words as input and prints only words that appear exactly once
14.grep -i root /etc/passwd: display lines containing the pattern "root" from the file /etc/passwd
15.grep -c bin /etc/passwd: display the number of lines that contain the pattern "bin" in the file /etc/passwd
16.grep -iA 3 root /etc/passwd: displays the lines containing the pattern root and 3 lines after them in the file /etc/passwd
17.grep -iv bin /etc/passwd: displays all the line in the file /etc/passwd that do not contain the pattern "bin"
18.grep -i "^[a-z]" /etc/ssh/sshd_config: displays all lines of the file /etc/ssh/sshd_config
19.tr Ac Ze: replaces all characters A and c from input Z and e respectively
20.tr -d cC: creates a script that removes all letters c and C from input
21.rev: reverses its input
22.cut -d: -f 1,6 /etc/passwd | sort: displays all users and their home directories sorted by users
23.find . -empty -printf "%f\n": finds all empty files and directories in the current directories and all subdirectories
24.find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f: writes script that lists all the files with a .gif extension in the current directory and all its sub directories
25.cut -c 1 | paste -s -d ' ': creates a script that decodes acrostic that use the first letter of each line
26.tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev: writes script that parses web servers logs in TSV format as input and displays the 11 hostsor IP addresses which did the most requests