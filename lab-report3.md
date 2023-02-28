# Lab Report 3
## Search files with pattern by using -name
This command will give all files and directories which contain with the letters inside the double quotations marks and in front of the star. It's useful because it helps me find all files with specific patterns ("_*") in the directory. Source: [LINK](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2/non-fiction/OUP 
find ./ -name "ch*"   
```

output
```
.//Berk/ch2.txt
.//Berk/ch1.txt
.//Berk/ch7.txt
.//Abernathy/ch2.txt
.//Abernathy/ch3.txt
.//Abernathy/ch1.txt
.//Abernathy/ch7.txt
.//Abernathy/ch6.txt
.//Abernathy/ch8.txt
.//Abernathy/ch9.txt
.//Abernathy/ch15.txt
.//Abernathy/ch14.txt
.//Rybczynski/ch2.txt
.//Rybczynski/ch3.txt
.//Rybczynski/ch1.txt
.//Kauffman/ch3.txt
.//Kauffman/ch1.txt
.//Kauffman/ch4.txt
.//Kauffman/ch5.txt
.//Kauffman/ch7.txt
.//Kauffman/ch6.txt
.//Kauffman/ch8.txt
.//Kauffman/ch9.txt
.//Kauffman/ch10.txt
.//Fletcher/ch2.txt
.//Fletcher/ch1.txt
.//Fletcher/ch5.txt
.//Fletcher/ch6.txt
.//Fletcher/ch9.txt
.//Fletcher/ch10.txt
.//Castro/chR.txt
.//Castro/chP.txt
.//Castro/chQ.txt
.//Castro/chB.txt
.//Castro/chC.txt
.//Castro/chA.txt
.//Castro/chV.txt
.//Castro/chW.txt
.//Castro/chM.txt
.//Castro/chZ.txt
.//Castro/chL.txt
.//Castro/chN.txt
.//Castro/chY.txt
.//Castro/chO.txt
```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2                
find ./ -name "P*"
```

output
```
.//travel_guides/berlitz2/Portugal-History.txt
.//travel_guides/berlitz2/Portugal-WhereToGo.txt
.//travel_guides/berlitz2/Poland-WhatToDo.txt
.//travel_guides/berlitz2/Paris-WhereToGo.txt
.//travel_guides/berlitz2/PuertoRico-WhatToDo.txt
.//travel_guides/berlitz2/PuertoRico-History.txt
.//travel_guides/berlitz2/Portugal-WhatToDo.txt
.//travel_guides/berlitz2/PuertoRico-WhereToGo.txt
.//travel_guides/berlitz2/Poland-History.txt
.//travel_guides/berlitz2/Paris-WhatToDo.txt
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
This command will search all files which are greater than or less than the sepecific size. It depends on the sign in front of the words size. i.e. If it is "-", it will search for all files greater than the specific size; if it is "+", it will search for all files less than the specific size. The specific size is behind the sign. It's useful to find the files in the specific size range. Source: [LINK](https://linuxconfig.org/how-to-use-find-command-to-search-for-files-based-on-file-size)

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


## Search files with case-insensitive by using -size
This command will search all files name with case-insensitive. It is useful when you want to search for files or directories that have similar names but different case variations. Source: [LINK](https://chat.openai.com/chat)

E.g.1
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2
find ./ -iname "ch2.txt"
```

output
```
.//non-fiction/OUP/Berk/ch2.txt
.//non-fiction/OUP/Abernathy/ch2.txt
.//non-fiction/OUP/Rybczynski/ch2.txt
.//non-fiction/OUP/Fletcher/ch2.txt
```

E.g.2
```
cd /Users/huxinyu/Documents/GitHub/docsearch/written_2
find ./ -iname "cha.txt"
```

output
```
.//non-fiction/OUP/Castro/chA.txt
```
