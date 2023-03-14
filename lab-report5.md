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


## Count the number of lines that matches the given pattern by using -c
The -c option to grep finds the number of lines that matches the given pattern. It's useful when you want to get the number of lines with the given pattern. `-r` and `-l` search through the directories recursively and list the matched files. Source: [LINK](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

E.g.1
```
grep -r -c -l "California" written_2/non-fiction/OUP/Castro 
```

output
```
written_2/non-fiction/OUP/Castro/chR.txt:1
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chP.txt:1
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt:1
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chB.txt:1
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt:1
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chA.txt:1
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chV.txt:1
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt:1
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chM.txt:1
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chZ.txt:0
written_2/non-fiction/OUP/Castro/chL.txt:1
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chN.txt:0
written_2/non-fiction/OUP/Castro/chY.txt:0
written_2/non-fiction/OUP/Castro/chO.txt:0
```

E.g.2
```
grep -c "the" written_2/travel_guides/berlitz1/HistoryDublin.txt
```

output
```
141
```


## Show line number while displaying the output by using -n
The -n option to grep show the line number of file with the line matched. It's useful when we want to find the line with the pattern we want. Source: [LINK](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

E.g.1
```
grep -n "Northern and Southern California" written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

output
```
6:Many Californians would like to divide their state into two new states, Northern and Southern California — corresponding to what they believe to be two distinct frames of mind as represented by San Francisco and Los Angeles. In fact you will find a little bit of both — San Francisco’s sophistication and Los Angeles’ sunny craziness — all over the place.
```

E.g.2
```
grep -n "Disneyland" written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

output
```
131:Anaheim, 27 miles (43 km) southeast of downtown L.A. on the Santa Ana Freeway, is the home of Disneyland. It’s best to allow a full day for a visit, as the entrance fee is expensive and there is so much to see. You can buy a Passport for one, two, or three days, covering the entire Disneyland complex and valid for unlimited use on all the attractions. Food and drink are not included in the admission price.
134:Northwest of Disneyland you will find the Movieland Wax Museum (7711 Beach Boulevard, Buena Park), which displays wax figures of film stars in scenes from their best-known films. For film buffs, the most interesting display will be the collection of old nickelodeons, autoscopes, and movieola machines that projected the very first moving pictures.
```


## Search files with case-insensitive by using -i
The -i option to grep searches for a string case insensitively in the given file. It is useful when you want to search for files or directories that have similar words but different case variations. `-r` and `-l` search through the directories recursively and list the matched files. Source: [LINK](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

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
