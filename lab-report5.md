# Lab Report 5
## Search files containing the whole pattern by using -w
The -w option to grep makes it match only the exactly whole words. It's useful because it helps me search files with exact words. '-r' and `-l` search through the directories recursively and list the matched files. Source: [LINK](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

E.g.1 This example searches the texts that match exactly whole word.
```
grep -r -w -l "California" written_2/non-fiction/OUP 
```

output
```
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chL.txt
```

E.g.2 This example demonstrates -w can't search texts with pattern as substring.
```
grep -r -w -l "Cal" written_2/non-fiction/OUP 
```

output
```

```


## Search directories by type by using -type d
This command will list all the directories. It's useful when you want to get a list of all directories in a particular directory. It's also useful when you want to perform a bulk action, such as deleting or moving, on all directories in a particular directory. Source: [LINK](https://www.redhat.com/sysadmin/linux-find-command)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2
find ./travel_guides -type d
```

output
```

```

E.g.2
```

```

output
```

```


## Search files greater than or less than specified size by using -size
This command will search all files which are greater than or less than the sepecific size. It depends on the sign in front of the words size. i.e. If it is "-", it will search for all files less than the specific size; if it is "+", it will search for all files greater than the specific size. The specific size is behind the sign. For instance, example 1 searches files with size less than 10k and example 2 searches files with size greater than 100k. It's useful to find the files in the specific size range. Source: [LINK](https://linuxconfig.org/how-to-use-find-command-to-search-for-files-based-on-file-size)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP/Castro  
find . -size -10k 
```

output
```

```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/travel_guides/berlitz1
find . -size +100k
```

output
```

```


## Search files with case-insensitive by using -i
This command will search all files name with case-insensitive. It is useful when you want to search for files or directories that have similar names but different case variations. Source: [LINK](https://chat.openai.com/chat)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2
find ./ -iname "ch4.txt"
```

output
```

```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2
find ./ -iname "cha.txt"
```

output
```

```
