# Lab Report 3 - Researching Commands (Week 5)
**`grep` command:**

The `grep` command takes a string and a file, and print out all the lines in that file that match the string. (The command to search for a pattern in text files).

## First command: `grep -l`
The `grep -l` command is used to print only the names of the files that contain the specified search pattern, instead of printing the matching lines.
1. Example `grep -l "explore" written_2/*/*/*.txt` outputs this:
```
written_2/travel_guides/berlitz1/HandRJamaica.txt
written_2/travel_guides/berlitz1/HistoryEgypt.txt
written_2/travel_guides/berlitz1/HistoryFWI.txt
written_2/travel_guides/berlitz1/HistoryGreek.txt
written_2/travel_guides/berlitz1/HistoryHawaii.txt
written_2/travel_guides/berlitz1/HistoryIndia.txt
written_2/travel_guides/berlitz1/HistoryJapan.txt
written_2/travel_guides/berlitz1/HistoryLasVegas.txt
written_2/travel_guides/berlitz1/IntroEgypt.txt
written_2/travel_guides/berlitz1/IntroJamaica.txt
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt
written_2/travel_guides/berlitz1/WhatToGreek.txt
written_2/travel_guides/berlitz1/WhatToIbiza.txt
written_2/travel_guides/berlitz1/WhatToIsrael.txt
written_2/travel_guides/berlitz1/WhatToJamaica.txt
written_2/travel_guides/berlitz1/WhatToLasVegas.txt
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt
written_2/travel_guides/berlitz1/WhatToMadeira.txt
written_2/travel_guides/berlitz1/WhereToDublin.txt
written_2/travel_guides/berlitz1/WhereToEdinburgh.txt
written_2/travel_guides/berlitz1/WhereToEgypt.txt
written_2/travel_guides/berlitz1/WhereToFWI.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToGreek.txt
written_2/travel_guides/berlitz1/WhereToHongKong.txt
written_2/travel_guides/berlitz1/WhereToIbiza.txt
written_2/travel_guides/berlitz1/WhereToIsrael.txt
written_2/travel_guides/berlitz1/WhereToIstanbul.txt
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz1/WhereToJerusalem.txt
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
written_2/travel_guides/berlitz1/WhereToMadeira.txt
written_2/travel_guides/berlitz1/WhereToMadrid.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz1/WhereToMallorca.txt
written_2/travel_guides/berlitz2/Algarve-History.txt
written_2/travel_guides/berlitz2/Algarve-Intro.txt
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
written_2/travel_guides/berlitz2/California-History.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-History.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-History.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
written_2/travel_guides/berlitz2/Portugal-History.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/PuertoRico-History.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
```
This command is searching for the word "explore" in all `.txt` files in any immediate subdirectories of the `written_2/` directory, and 
printing the names of the files that contain the word "explore". This command is useful if you want to find all files that contain 
a particular word or phrase in a large project with many text files.
 
2. Example `grep -l "Lucayans" written_2/*/*/*.txt` outputs this:
```
written_2/travel_guides/berlitz2/Bahamas-History.txt
```
This command is searching for the word "Lucayans" in all `.txt` files in any immediate subdirectories of the `written_2/` directory, and 
printing the names of the files that contain the word "Lucayans". This command is useful if you want to find all files that contain 
a particular word or phrase in a large project with many text files.

## Second command: `grep -i`
The `grep -i` command is used to perform a case-insensitive search when searching for a pattern in text files.
1. Example `grep -i "pineapples" written_2/*/*/*.txt` outputs this:
```
written_2/travel_guides/berlitz1/HistoryHawaii.txt:        Pineapples and War
written_2/travel_guides/berlitz1/WhereToFWI.txt:        emporium you’ll have your pick of fresh Martinique pineapples, coconut
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        of rambutans, pineapples, and bananas, as well as locally made nougat
written_2/travel_guides/berlitz2/China-History.txt:Conservatism and hostility to foreign ideas, however, couldn’t be absolutely maintained. During the Ming era, China imported tobacco, pineapples, peanuts, and syphilis. Thanks to the emancipated Confucian tradition, Christian missionaries were usually welcomed, although they hardly achieved mass conversions. From the Jesuits the Chinese learned mathematics and astronomy; the old observatory still stands in downtown Beijing.
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:Ice cream, fruit, cheese, or flan (crème caramel) are the most popular desserts. In the summer and early autumn you will be spoiled with an enormous array of fruit. The weekly markets — the best place to buy — are full of strawberries, nísperos (a cousin of the lychee), grapes, figs, melons, peaches, apricots, raspberries, pomegranates, grapefruit, lemons, oranges, tangerines, apples, pears, and even locally grown bananas, pineapples, and dates.
```
This command is searching for the word "pineapples" in all `.txt` files in any immediate subdirectories of the `written_2/` directory, and printing all the lines that contain the word "pineapples", regardless if it is upper case or lower case. This command is useful if you want to perform a search that's not case-sensitive, and you do not want to have to search for all possible variations of the word.

2. Example `grep -i -l "pineapples" written_2/*/*/*.txt` outputs this:
```
written_2/travel_guides/berlitz1/HistoryHawaii.txt
written_2/travel_guides/berlitz1/WhereToFWI.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz2/China-History.txt
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
```
This command is searching for the word "pineapples" in all `.txt` files in any immediate subdirectories of the `written_2/` directory, and printing only the names of the files that contain the word "pineapples", regardless if it is upper case or lower case. This command is useful if you want to perform a search that's not case-sensitive and simply looking for the files containing the word or phrase without having to read the text along with it.

## Third command: `grep -n`
The `grep -n` command is used to display the line number of each matching line in the output when searching for a pattern in a file or a set of files
1. Example `grep -n "mango" written_2/*/*/*.txt` outputs this:
```
written_2/travel_guides/berlitz1/IntroMadeira.txt:33:        mangoes, passion fruit, watermelons, and avocados.
written_2/travel_guides/berlitz1/WhereToIndia.txt:1025:        terraced fields and mango groves over the deepest ravines to the
written_2/travel_guides/berlitz1/WhereToIndia.txt:1831:        branches of mangoes. The friezes are more sophisticated, showing
written_2/travel_guides/berlitz1/WhereToIndia.txt:2138:        streams of the Cauvery river, past groves of mango trees, sugar cane
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:687:        jungle fruit are mango, durian, rambutan, and wild banana. At over
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:76:Start your explorations by driving west on the autopista (highway) linking Havana with the province’s capital city of Pinar del Río. About 63 km (39 miles) along the highway, a turnoff leaves the level, palm-dotted plains for Soroa, where a richly endowed botanical garden nestles in the mountain foothills near a tired little tourist complex. A guided tour reveals an orchid garden, lychee and mango trees, coffee plants, and splendid specimens of jagüey and ceiba trees. A restaurant in the villa of Castillo de las Nubes on a nearby mountain has stunning views.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:41:Manzanillo has an enticingly tropical geography, comprised of vast groves of tall palms, abundant mango trees, and successive coves graced with smooth sand beaches. To the north, mountains blanketed with palms rise alongside the shoreline. And over it all lies the veneer of perfect weather — balmy temperatures and year-round sea breezes. Even the approach by plane into Manzanillo showcases the promise of a perfect vacation — you fly in over the beach and golf course.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:68:A countryside visit to Barra de Potosí, located 21 km (14 miles) south of Zihuatanejo offers a chance to see a small fishing village, coconut and mango plantations, and a lagoon known for the numerous tropical birds that inhabit it.
```
This command is searching for the word "mango" in all `.txt` files in any immediate subdirectories of the `written_2/` directory, and printing all the lines that contain the word "mango", along with their line numbers. This command is useful when you want to quickly find the line numbers for a particular search pattern in multiple files.

2. Example `grep -n -h "mango" written_2/*/*/*.txt` outputs this:
```
33:        mangoes, passion fruit, watermelons, and avocados.
1025:        terraced fields and mango groves over the deepest ravines to the
1831:        branches of mangoes. The friezes are more sophisticated, showing
2138:        streams of the Cauvery river, past groves of mango trees, sugar cane
687:        jungle fruit are mango, durian, rambutan, and wild banana. At over
76:Start your explorations by driving west on the autopista (highway) linking Havana with the province’s capital city of Pinar del Río. About 63 km (39 miles) along the highway, a turnoff leaves the level, palm-dotted plains for Soroa, where a richly endowed botanical garden nestles in the mountain foothills near a tired little tourist complex. A guided tour reveals an orchid garden, lychee and mango trees, coffee plants, and splendid specimens of jagüey and ceiba trees. A restaurant in the villa of Castillo de las Nubes on a nearby mountain has stunning views.
41:Manzanillo has an enticingly tropical geography, comprised of vast groves of tall palms, abundant mango trees, and successive coves graced with smooth sand beaches. To the north, mountains blanketed with palms rise alongside the shoreline. And over it all lies the veneer of perfect weather — balmy temperatures and year-round sea breezes. Even the approach by plane into Manzanillo showcases the promise of a perfect vacation — you fly in over the beach and golf course.
68:A countryside visit to Barra de Potosí, located 21 km (14 miles) south of Zihuatanejo offers a chance to see a small fishing village, coconut and mango plantations, and a lagoon known for the numerous tropical birds that inhabit it.
```
This command is searching for all files with a `.txt` extension inside any immediate subdirectories of the `written_2/` directory, and prints all the lines that contain the word "mango", along with their line numbers. The `-h` command tells grep not to print the file names in the output. This command is useful if you do not need to see the file names in the output, and just want to focus on the lines that match the search pattern.

## Fourth command: `grep -c`
The `grep -c` command is used to count the number of times a pattern appears in a file or a set of files.
1. Example `grep -c "tourist" written_2/*/*/*.txt` outputs this:
```
written_2/travel_guides/berlitz1/HandRHawaii.txt:0
written_2/travel_guides/berlitz1/HandRHongKong.txt:0
written_2/travel_guides/berlitz1/HandRIbiza.txt:0
written_2/travel_guides/berlitz1/HandRIsrael.txt:3
written_2/travel_guides/berlitz1/HandRIstanbul.txt:0
written_2/travel_guides/berlitz1/HandRJamaica.txt:0
written_2/travel_guides/berlitz1/HandRJerusalem.txt:0
written_2/travel_guides/berlitz1/HandRLakeDistrict.txt:0
written_2/travel_guides/berlitz1/HandRLasVegas.txt:0
written_2/travel_guides/berlitz1/HandRLisbon.txt:0
written_2/travel_guides/berlitz1/HandRLosAngeles.txt:0
written_2/travel_guides/berlitz1/HandRMadeira.txt:1
written_2/travel_guides/berlitz1/HandRMadrid.txt:1
written_2/travel_guides/berlitz1/HandRMallorca.txt:0
written_2/travel_guides/berlitz1/HistoryDublin.txt:0
written_2/travel_guides/berlitz1/HistoryEdinburgh.txt:1
written_2/travel_guides/berlitz1/HistoryEgypt.txt:1
written_2/travel_guides/berlitz1/HistoryFWI.txt:0
written_2/travel_guides/berlitz1/HistoryFrance.txt:0
written_2/travel_guides/berlitz1/HistoryGreek.txt:0
written_2/travel_guides/berlitz1/HistoryHawaii.txt:4
written_2/travel_guides/berlitz1/HistoryHongKong.txt:0
written_2/travel_guides/berlitz1/HistoryIbiza.txt:0
written_2/travel_guides/berlitz1/HistoryIndia.txt:0
written_2/travel_guides/berlitz1/HistoryIsrael.txt:0
written_2/travel_guides/berlitz1/HistoryIstanbul.txt:1
written_2/travel_guides/berlitz1/HistoryItaly.txt:2
written_2/travel_guides/berlitz1/HistoryJamaica.txt:3
written_2/travel_guides/berlitz1/HistoryJapan.txt:0
written_2/travel_guides/berlitz1/HistoryJerusalem.txt:0
written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt:0
written_2/travel_guides/berlitz1/HistoryLasVegas.txt:0
written_2/travel_guides/berlitz1/HistoryMadeira.txt:1
written_2/travel_guides/berlitz1/HistoryMadrid.txt:1
written_2/travel_guides/berlitz1/HistoryMalaysia.txt:0
written_2/travel_guides/berlitz1/HistoryMallorca.txt:1
written_2/travel_guides/berlitz1/IntroDublin.txt:0
written_2/travel_guides/berlitz1/IntroEdinburgh.txt:0
written_2/travel_guides/berlitz1/IntroEgypt.txt:1
written_2/travel_guides/berlitz1/IntroFWI.txt:4
written_2/travel_guides/berlitz1/IntroFrance.txt:1
written_2/travel_guides/berlitz1/IntroGreek.txt:4
written_2/travel_guides/berlitz1/IntroHongKong.txt:0
written_2/travel_guides/berlitz1/IntroIbiza.txt:4
written_2/travel_guides/berlitz1/IntroIndia.txt:0
written_2/travel_guides/berlitz1/IntroIsrael.txt:0
written_2/travel_guides/berlitz1/IntroIstanbul.txt:1
written_2/travel_guides/berlitz1/IntroItaly.txt:1
written_2/travel_guides/berlitz1/IntroJamaica.txt:0
written_2/travel_guides/berlitz1/IntroJapan.txt:0
written_2/travel_guides/berlitz1/IntroJerusalem.txt:0
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt:0
written_2/travel_guides/berlitz1/IntroLasVegas.txt:2
written_2/travel_guides/berlitz1/IntroLosAngeles.txt:0
written_2/travel_guides/berlitz1/IntroMadeira.txt:3
written_2/travel_guides/berlitz1/IntroMadrid.txt:1
written_2/travel_guides/berlitz1/IntroMalaysia.txt:0
written_2/travel_guides/berlitz1/IntroMallorca.txt:1
written_2/travel_guides/berlitz1/JungleMalaysia.txt:0
written_2/travel_guides/berlitz1/WhatToDublin.txt:4
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:1
written_2/travel_guides/berlitz1/WhatToEgypt.txt:5
written_2/travel_guides/berlitz1/WhatToFWI.txt:12
written_2/travel_guides/berlitz1/WhatToFrance.txt:0
written_2/travel_guides/berlitz1/WhatToGreek.txt:0
written_2/travel_guides/berlitz1/WhatToHawaii.txt:0
written_2/travel_guides/berlitz1/WhatToHongKong.txt:2
written_2/travel_guides/berlitz1/WhatToIbiza.txt:8
written_2/travel_guides/berlitz1/WhatToIndia.txt:2
written_2/travel_guides/berlitz1/WhatToIsrael.txt:8
written_2/travel_guides/berlitz1/WhatToIstanbul.txt:8
written_2/travel_guides/berlitz1/WhatToItaly.txt:3
written_2/travel_guides/berlitz1/WhatToJamaica.txt:13
written_2/travel_guides/berlitz1/WhatToJapan.txt:5
written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:10
written_2/travel_guides/berlitz1/WhatToLasVegas.txt:5
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:6
written_2/travel_guides/berlitz1/WhatToMadeira.txt:5
written_2/travel_guides/berlitz1/WhatToMalaysia.txt:3
written_2/travel_guides/berlitz1/WhatToMallorca.txt:3
written_2/travel_guides/berlitz1/WhereToDublin.txt:2
written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:2
written_2/travel_guides/berlitz1/WhereToEgypt.txt:8
written_2/travel_guides/berlitz1/WhereToFWI.txt:12
written_2/travel_guides/berlitz1/WhereToFrance.txt:24
written_2/travel_guides/berlitz1/WhereToGreek.txt:11
written_2/travel_guides/berlitz1/WhereToHawaii.txt:1
written_2/travel_guides/berlitz1/WhereToHongKong.txt:13
written_2/travel_guides/berlitz1/WhereToIbiza.txt:15
written_2/travel_guides/berlitz1/WhereToIndia.txt:2
written_2/travel_guides/berlitz1/WhereToIsrael.txt:9
written_2/travel_guides/berlitz1/WhereToIstanbul.txt:5
written_2/travel_guides/berlitz1/WhereToItaly.txt:25
written_2/travel_guides/berlitz1/WhereToJapan.txt:19
written_2/travel_guides/berlitz1/WhereToJerusalem.txt:2
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:2
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:16
written_2/travel_guides/berlitz1/WhereToMadeira.txt:8
written_2/travel_guides/berlitz1/WhereToMadrid.txt:1
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:5
written_2/travel_guides/berlitz1/WhereToMallorca.txt:13
written_2/travel_guides/berlitz2/Algarve-History.txt:1
written_2/travel_guides/berlitz2/Algarve-Intro.txt:4
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:12
written_2/travel_guides/berlitz2/Amsterdam-History.txt:1
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt:0
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:1
written_2/travel_guides/berlitz2/Athens-History.txt:0
written_2/travel_guides/berlitz2/Athens-Intro.txt:0
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt:4
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Bahamas-History.txt:3
written_2/travel_guides/berlitz2/Bahamas-Intro.txt:1
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:10
written_2/travel_guides/berlitz2/Bali-History.txt:1
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt:4
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:13
written_2/travel_guides/berlitz2/Barcelona-History.txt:0
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt:2
written_2/travel_guides/berlitz2/Beijing-History.txt:1
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt:8
written_2/travel_guides/berlitz2/Berlin-History.txt:0
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt:2
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:3
written_2/travel_guides/berlitz2/Bermuda-history.txt:2
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:5
written_2/travel_guides/berlitz2/Budapest-History.txt:0
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:5
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:7
written_2/travel_guides/berlitz2/California-History.txt:0
written_2/travel_guides/berlitz2/California-WhatToDo.txt:1
written_2/travel_guides/berlitz2/California-WhereToGo.txt:7
written_2/travel_guides/berlitz2/Canada-History.txt:0
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:24
written_2/travel_guides/berlitz2/CanaryIslands-History.txt:1
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:3
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:17
written_2/travel_guides/berlitz2/Cancun-History.txt:1
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:10
written_2/travel_guides/berlitz2/China-History.txt:2
written_2/travel_guides/berlitz2/China-WhatToDo.txt:5
written_2/travel_guides/berlitz2/China-WhereToGo.txt:48
written_2/travel_guides/berlitz2/Costa-History.txt:1
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt:5
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:7
written_2/travel_guides/berlitz2/CostaBlanca-History.txt:0
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:11
written_2/travel_guides/berlitz2/Crete-History.txt:0
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:11
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:3
written_2/travel_guides/berlitz2/Cuba-History.txt:0
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:5
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:26
written_2/travel_guides/berlitz2/Nepal-History.txt:0
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt:8
written_2/travel_guides/berlitz2/NewOrleans-History.txt:1
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt:5
written_2/travel_guides/berlitz2/Poland-History.txt:0
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Portugal-History.txt:0
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:24
written_2/travel_guides/berlitz2/PuertoRico-History.txt:0
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt:1
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt:5
written_2/travel_guides/berlitz2/Vallarta-History.txt:6
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:5
```
This command is searching for the word "tourist" in all `.txt` files in any immediate subdirectories of the `written_2/` directory, and printing the total number of lines that contain the word "tourist" across all the files. This command is useful if you want to quickly get a count of the number of occurrences of a particular pattern in a file or a set of files. 

2. Example `grep -c -v "tourist" written_2/*/*/*.txt` outputs this:
```
written_2/travel_guides/berlitz1/HandRHawaii.txt:248
written_2/travel_guides/berlitz1/HandRHongKong.txt:29
written_2/travel_guides/berlitz1/HandRIbiza.txt:20
written_2/travel_guides/berlitz1/HandRIsrael.txt:392
written_2/travel_guides/berlitz1/HandRIstanbul.txt:24
written_2/travel_guides/berlitz1/HandRJamaica.txt:379
written_2/travel_guides/berlitz1/HandRJerusalem.txt:31
written_2/travel_guides/berlitz1/HandRLakeDistrict.txt:34
written_2/travel_guides/berlitz1/HandRLasVegas.txt:34
written_2/travel_guides/berlitz1/HandRLisbon.txt:27
written_2/travel_guides/berlitz1/HandRLosAngeles.txt:28
written_2/travel_guides/berlitz1/HandRMadeira.txt:29
written_2/travel_guides/berlitz1/HandRMadrid.txt:213
written_2/travel_guides/berlitz1/HandRMallorca.txt:32
written_2/travel_guides/berlitz1/HistoryDublin.txt:238
written_2/travel_guides/berlitz1/HistoryEdinburgh.txt:305
written_2/travel_guides/berlitz1/HistoryEgypt.txt:263
written_2/travel_guides/berlitz1/HistoryFWI.txt:229
written_2/travel_guides/berlitz1/HistoryFrance.txt:552
written_2/travel_guides/berlitz1/HistoryGreek.txt:279
written_2/travel_guides/berlitz1/HistoryHawaii.txt:229
written_2/travel_guides/berlitz1/HistoryHongKong.txt:216
written_2/travel_guides/berlitz1/HistoryIbiza.txt:192
written_2/travel_guides/berlitz1/HistoryIndia.txt:792
written_2/travel_guides/berlitz1/HistoryIsrael.txt:244
written_2/travel_guides/berlitz1/HistoryIstanbul.txt:391
written_2/travel_guides/berlitz1/HistoryItaly.txt:717
written_2/travel_guides/berlitz1/HistoryJamaica.txt:248
written_2/travel_guides/berlitz1/HistoryJapan.txt:602
written_2/travel_guides/berlitz1/HistoryJerusalem.txt:264
written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt:197
written_2/travel_guides/berlitz1/HistoryLasVegas.txt:278
written_2/travel_guides/berlitz1/HistoryMadeira.txt:178
written_2/travel_guides/berlitz1/HistoryMadrid.txt:187
written_2/travel_guides/berlitz1/HistoryMalaysia.txt:516
written_2/travel_guides/berlitz1/HistoryMallorca.txt:202
written_2/travel_guides/berlitz1/IntroDublin.txt:119
written_2/travel_guides/berlitz1/IntroEdinburgh.txt:139
written_2/travel_guides/berlitz1/IntroEgypt.txt:117
written_2/travel_guides/berlitz1/IntroFWI.txt:114
written_2/travel_guides/berlitz1/IntroFrance.txt:160
written_2/travel_guides/berlitz1/IntroGreek.txt:122
written_2/travel_guides/berlitz1/IntroHongKong.txt:91
written_2/travel_guides/berlitz1/IntroIbiza.txt:93
written_2/travel_guides/berlitz1/IntroIndia.txt:385
written_2/travel_guides/berlitz1/IntroIsrael.txt:82
written_2/travel_guides/berlitz1/IntroIstanbul.txt:106
written_2/travel_guides/berlitz1/IntroItaly.txt:184
written_2/travel_guides/berlitz1/IntroJamaica.txt:153
written_2/travel_guides/berlitz1/IntroJapan.txt:278
written_2/travel_guides/berlitz1/IntroJerusalem.txt:145
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt:170
written_2/travel_guides/berlitz1/IntroLasVegas.txt:172
written_2/travel_guides/berlitz1/IntroLosAngeles.txt:96
written_2/travel_guides/berlitz1/IntroMadeira.txt:143
written_2/travel_guides/berlitz1/IntroMadrid.txt:165
written_2/travel_guides/berlitz1/IntroMalaysia.txt:131
written_2/travel_guides/berlitz1/IntroMallorca.txt:134
written_2/travel_guides/berlitz1/JungleMalaysia.txt:106
written_2/travel_guides/berlitz1/WhatToDublin.txt:315
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:331
written_2/travel_guides/berlitz1/WhatToEgypt.txt:326
written_2/travel_guides/berlitz1/WhatToFWI.txt:401
written_2/travel_guides/berlitz1/WhatToFrance.txt:46
written_2/travel_guides/berlitz1/WhatToGreek.txt:285
written_2/travel_guides/berlitz1/WhatToHawaii.txt:42
written_2/travel_guides/berlitz1/WhatToHongKong.txt:373
written_2/travel_guides/berlitz1/WhatToIbiza.txt:585
written_2/travel_guides/berlitz1/WhatToIndia.txt:281
written_2/travel_guides/berlitz1/WhatToIsrael.txt:326
written_2/travel_guides/berlitz1/WhatToIstanbul.txt:391
written_2/travel_guides/berlitz1/WhatToItaly.txt:339
written_2/travel_guides/berlitz1/WhatToJamaica.txt:1204
written_2/travel_guides/berlitz1/WhatToJapan.txt:510
written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:310
written_2/travel_guides/berlitz1/WhatToLasVegas.txt:711
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:363
written_2/travel_guides/berlitz1/WhatToMadeira.txt:414
written_2/travel_guides/berlitz1/WhatToMalaysia.txt:360
written_2/travel_guides/berlitz1/WhatToMallorca.txt:255
written_2/travel_guides/berlitz1/WhereToDublin.txt:1286
written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:1132
written_2/travel_guides/berlitz1/WhereToEgypt.txt:1205
written_2/travel_guides/berlitz1/WhereToFWI.txt:933
written_2/travel_guides/berlitz1/WhereToFrance.txt:3745
written_2/travel_guides/berlitz1/WhereToGreek.txt:1160
written_2/travel_guides/berlitz1/WhereToHawaii.txt:45
written_2/travel_guides/berlitz1/WhereToHongKong.txt:972
written_2/travel_guides/berlitz1/WhereToIbiza.txt:588
written_2/travel_guides/berlitz1/WhereToIndia.txt:2525
written_2/travel_guides/berlitz1/WhereToIsrael.txt:1232
written_2/travel_guides/berlitz1/WhereToIstanbul.txt:1268
written_2/travel_guides/berlitz1/WhereToItaly.txt:4141
written_2/travel_guides/berlitz1/WhereToJapan.txt:2666
written_2/travel_guides/berlitz1/WhereToJerusalem.txt:1080
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:1205
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:1116
written_2/travel_guides/berlitz1/WhereToMadeira.txt:928
written_2/travel_guides/berlitz1/WhereToMadrid.txt:1108
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:2597
written_2/travel_guides/berlitz1/WhereToMallorca.txt:1033
written_2/travel_guides/berlitz2/Algarve-History.txt:45
written_2/travel_guides/berlitz2/Algarve-Intro.txt:24
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt:69
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:159
written_2/travel_guides/berlitz2/Amsterdam-History.txt:50
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt:21
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt:69
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:138
written_2/travel_guides/berlitz2/Athens-History.txt:60
written_2/travel_guides/berlitz2/Athens-Intro.txt:22
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt:62
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:154
written_2/travel_guides/berlitz2/Bahamas-History.txt:40
written_2/travel_guides/berlitz2/Bahamas-Intro.txt:23
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt:65
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:159
written_2/travel_guides/berlitz2/Bali-History.txt:38
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt:56
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:197
written_2/travel_guides/berlitz2/Barcelona-History.txt:30
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt:48
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt:145
written_2/travel_guides/berlitz2/Beijing-History.txt:36
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt:61
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt:143
written_2/travel_guides/berlitz2/Berlin-History.txt:61
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt:61
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt:237
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt:93
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:115
written_2/travel_guides/berlitz2/Bermuda-history.txt:40
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:185
written_2/travel_guides/berlitz2/Budapest-History.txt:47
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:66
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:178
written_2/travel_guides/berlitz2/California-History.txt:59
written_2/travel_guides/berlitz2/California-WhatToDo.txt:73
written_2/travel_guides/berlitz2/California-WhereToGo.txt:176
written_2/travel_guides/berlitz2/Canada-History.txt:92
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:509
written_2/travel_guides/berlitz2/CanaryIslands-History.txt:42
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:74
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:143
written_2/travel_guides/berlitz2/Cancun-History.txt:32
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt:65
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:115
written_2/travel_guides/berlitz2/China-History.txt:75
written_2/travel_guides/berlitz2/China-WhatToDo.txt:56
written_2/travel_guides/berlitz2/China-WhereToGo.txt:461
written_2/travel_guides/berlitz2/Costa-History.txt:47
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt:57
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:168
written_2/travel_guides/berlitz2/CostaBlanca-History.txt:43
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:147
written_2/travel_guides/berlitz2/Crete-History.txt:49
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt:70
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:149
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:133
written_2/travel_guides/berlitz2/Cuba-History.txt:41
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:51
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:167
written_2/travel_guides/berlitz2/Nepal-History.txt:50
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt:103
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt:114
written_2/travel_guides/berlitz2/NewOrleans-History.txt:60
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt:42
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt:201
written_2/travel_guides/berlitz2/Poland-History.txt:51
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt:53
written_2/travel_guides/berlitz2/Portugal-History.txt:51
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt:89
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:316
written_2/travel_guides/berlitz2/PuertoRico-History.txt:34
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt:107
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt:128
written_2/travel_guides/berlitz2/Vallarta-History.txt:38
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:82
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:140
```
This command is searching for all files with a `.txt` extension inside any immediate subdirectories of `written_2/` directory, and counts the number of lines in those files that DO NOT contain the word "tourist" from the `-v` command which is used to invert the search and print all lines that do not match the search pattern. This command is useful if you want to count the number of lines that do not match a particular search pattern in multiple files.


## Sources Cited:
1. [grep(1) — Linux manual page](https://man7.org/linux/man-pages/man1/grep.1.html)
2. [grep command in Unix/Linux](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
3. [Grep Command in Linux/UNIX](https://www.digitalocean.com/community/tutorials/grep-command-in-linux-unix)
4. [15 Practical Grep Command Examples In Linux / UNIX](https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/)
5. [How To Use grep Command In Linux / UNIX With Practical Examples](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)
6. [Common Examples of the Grep Command in Linux [With Free Cheatsheet Download]](https://linuxhandbook.com/grep-command-cheatsheet/)
7. [How To Use grep Command In Linux/UNIX](https://phoenixnap.com/kb/grep-command-linux-unix-examples)
8. [ChatGPT](https://openai.com/blog/chatgpt/)
