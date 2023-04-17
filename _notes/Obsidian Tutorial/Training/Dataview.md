---
title: A New Hope 
year: 1977 
favorite: true 
cast: 
 - Mark Hamill 
 - Harrison Ford 
 - Carrie Fisher
Rating: ⭐⭐⭐⭐⭐
---

```dataview
LIST 
```

```dataview
LIST FROM #test OR #another 
```
![[cover.png]]
```dataview
LIST FROM "That's a folder"
```

```dataview
LIST Where file.name = "Test"
```

```dataview
LIST Where contains(file.name, "Test")
```

```dataview
Table author AS autor, about AS sobre
FROM "Test"
```


==HIGH LIGHT==

```dataview  
List  
From ""  
Sort file.mtime DESC  
Limit 5  
```

```dataview  
Table file.ctime as created  
sort ASCE  
Limit 20  
```


```dataview  
Table
From [[Test]]
```



```dataview  
Table author as Author
From outgoing([[Another]])
```

```dataview  
Table author as Author,category as Category, rating as Rating, status as Status, cast  
From #test  
```

```dataview  
Table author as Author,category as Category, rating as Rating, status as Status  
From #test AND -"Another"  
```

```dataview  
Table WITHOUT ID author as Author,category as Category, rating as Rating, status as Status  
From #test AND -"Another"  
```

```dataview  
Table WITHOUT ID Cover, Rating
From "Another"
```

```dataview
Table
Where contains(favorite,true)
```

![[Drawing 2023-04-07 20.08.53.excalidraw]]

```mermaid
flowchart LR 
A --- B
```