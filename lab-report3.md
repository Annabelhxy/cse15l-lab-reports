# Lab Report 3
## Search files with pattern
This command will give all files which have ".txt" at the end. It's useful because it helps me find all ".txt" files in the directory.

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

source: [Link](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

## Search a file with specific name
This command will search for specific file in the directory. It's useful because it helps me find the specific file by using its name. 

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


## Search directories by type
This command will list all the directories. It's useful to help me know the catalog of the directory. 

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


## Search files greater than or less than specified size
This command will search all files which are greater than or less than the sepecific size. It's useful to find the files in the size range. 

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP
find . -size -10k 
```

output
```
.
./Berk
./Abernathy
./Rybczynski
./Kauffman
./Fletcher
./Castro
./Castro/chQ.txt
./Castro/chW.txt
./Castro/chZ.txt
./Castro/chN.txt
./Castro/chY.txt
./Castro/chO.txt
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
