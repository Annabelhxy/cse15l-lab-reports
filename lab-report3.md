# Lab Report 3
## Search a file with pattern

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


## Search a file with specific name

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


## find directory by type

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


## search for all files greater than or lower than specified size

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
