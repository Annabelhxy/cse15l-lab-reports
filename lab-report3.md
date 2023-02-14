# Lab Report 3
## Search files with pattern by using -name "*.txt"
This command will give all files which have ".txt" at the end. It's useful because it helps me find all ".txt" files in the directory. Source: [LINK](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP 
find ./Abernathy -name "*.txt"
```

output
```
./Abernathy/ch2.txt
./Abernathy/ch3.txt
./Abernathy/ch1.txt
./Abernathy/ch7.txt
./Abernathy/ch6.txt
./Abernathy/ch8.txt
./Abernathy/ch9.txt
./Abernathy/ch15.txt
./Abernathy/ch14.txt
```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP 
find ./Fletcher -name "*.txt
```

output
```
./Fletcher/ch2.txt
./Fletcher/ch1.txt
./Fletcher/ch5.txt
./Fletcher/ch6.txt
./Fletcher/ch9.txt
./Fletcher/ch10.txt
```


## Search a file with specific name by using -name ".txt"
This command will search for specific file in the directory. It's useful because it helps me find the specific file by using its name. Source: [LINK](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/travel_guides 
find ./berlitz1 -name "HandRHawaii.txt"
```

output
```
./berlitz1/HandRHawaii.txt
```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP 
find ./Abernathy -name "ch1.txt"
```

output
```
./Abernathy/ch1.txt
```


## Search directories by type by using -type d
This command will list all the directories. It's useful to help me know the catalog of the directory. Source: [LINK](https://www.redhat.com/sysadmin/linux-find-command)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2
find ./travel_guides -type d
```

output
```
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction 
find ./OUP -type d
```

output
```
./OUP
./OUP/Berk
./OUP/Abernathy
./OUP/Rybczynski
./OUP/Kauffman
./OUP/Fletcher
./OUP/Castro
```


## Search files greater than or less than specified size by using -size
This command will search all files which are greater than or less than the sepecific size. It's useful to find the files in the size range. Source: [LINK](https://linuxconfig.org/how-to-use-find-command-to-search-for-files-based-on-file-size)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP/Castro  
find . -size -10k 
```

output
```
.
./chQ.txt
./chW.txt
./chZ.txt
./chN.txt
./chY.txt
./chO.txt
```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/travel_guides/berlitz1
find . -size +100k
```

output
```
./WhereToIndia.txt
./WhereToItaly.txt
./WhereToMalaysia.txt
./WhereToJapan.txt
./WhereToFrance.txt
```
