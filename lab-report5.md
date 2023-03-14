# Lab Report 5
## Search files containing the whole pattern by using -w
The -w option to grep makes it match only the exactly whole words. It's useful because it helps me search files with exact words. `-r` and `-l` search through the directories recursively and list the matched files. Source: [LINK](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

E.g.1 This example searches the files that match exactly whole word.
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
This command will list all the directories. It's useful when you want to get a list of all directories in a particular directory. It's also useful when you want to perform a bulk action, such as deleting or moving, on all directories in a particular directory. Source: [LINK](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

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
This command will search all files which are greater than or less than the sepecific size. It depends on the sign in front of the words size. i.e. If it is "-", it will search for all files less than the specific size; if it is "+", it will search for all files greater than the specific size. The specific size is behind the sign. For instance, example 1 searches files with size less than 10k and example 2 searches files with size greater than 100k. It's useful to find the files in the specific size range. Source: [LINK]([https://linuxconfig.org/how-to-use-find-command-to-search-for-files-based-on-file-size](https://www.geeksforgeeks.org/grep-command-in-unixlinux/))

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
The -i option to grep searches for a string case insensitively in the given file. It is useful when you want to search for files or directories that have similar words but different case variations. `-r` and `-l` search through the directories recursively and list the matched files. Source: [LINK]([https://chat.openai.com/chat](https://www.geeksforgeeks.org/grep-command-in-unixlinux/))

E.g.1
```
grep -r -i -l "california" written_2/non-fiction/OUP/
```

output
```
written_2/non-fiction/OUP//Berk/ch1.txt
written_2/non-fiction/OUP//Abernathy/ch2.txt
written_2/non-fiction/OUP//Abernathy/ch15.txt
written_2/non-fiction/OUP//Rybczynski/ch2.txt
written_2/non-fiction/OUP//Rybczynski/ch1.txt
written_2/non-fiction/OUP//Kauffman/ch1.txt
written_2/non-fiction/OUP//Kauffman/ch9.txt
written_2/non-fiction/OUP//Fletcher/ch9.txt
written_2/non-fiction/OUP//Castro/chR.txt
written_2/non-fiction/OUP//Castro/chP.txt
written_2/non-fiction/OUP//Castro/chQ.txt
written_2/non-fiction/OUP//Castro/chB.txt
written_2/non-fiction/OUP//Castro/chC.txt
written_2/non-fiction/OUP//Castro/chA.txt
written_2/non-fiction/OUP//Castro/chV.txt
written_2/non-fiction/OUP//Castro/chW.txt
written_2/non-fiction/OUP//Castro/chM.txt
written_2/non-fiction/OUP//Castro/chL.txt
```

E.g.2
```
grep -r -i -l "Hotel" written_2/travel_guides/berlitz2
```

output
```
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-History.txt
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
written_2/travel_guides/berlitz2/Berlin-History.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
written_2/travel_guides/berlitz2/Bali-History.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-History.txt
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2/travel_guides/berlitz2/Algarve-Intro.txt
written_2/travel_guides/berlitz2/Nepal-History.txt
written_2/travel_guides/berlitz2/Canada-History.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt
written_2/travel_guides/berlitz2/Beijing-History.txt
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-history.txt
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/China-WhatToDo.txt
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
```
