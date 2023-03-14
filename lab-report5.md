# Lab Report 5
## Search files with pattern by using -name
This command will give all files and directories which contain with the letters inside the double quotations marks and in front of the star. It's useful because it helps me find all files with specific patterns ("_*") in the directory. Source: [LINK](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP 
find ./ -name "ch*"   
```

output
```

```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2                
find ./ -name "P*"
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
