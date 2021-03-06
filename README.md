# BIS 305 Assignment 4 - Case Problem 1.

This repo is for use to code and debug the BIS 305 Assignment 4 - Case Problem 1.

### Use Case 1

The inputs in the console could be like:
```html
Enter number of contestants last year >> 6
Enter number of contestants this year >> 14
```

The output from the console should be:
```html
Last year's competition had 6 contestants, and this year's has 14 contestants
Revenue expected this year is $350.00
The competition is more than twice as big this year!
```

### Use Case 2

The inputs in the console could be like:
```html
Enter number of contestants last year >> 39
Enter number of contestants this year >> 47
```

The output from the console should be:
```html
Last year's competition had 39 contestants, and this year's has 47 contestants
Revenue expected this year is $1,175.00
The competition is bigger than ever!
```

### Use Case 3

The inputs in the console could be like:
```html
Enter number of contestants last year >> 55
Enter number of contestants this year >> 54
```

The output from the console should be:
```html
Last year's competition had 55 contestants, and this year's has 54 contestants
Revenue expected this year is $1,350.00
A tighter race this year! Come out and cast your vote!
```

### Here is a flowchart for the logic:  
<!-- below from https://github.com/mermaid-js/mermaid -->
```mermaid
flowchart TB
A["Display  #quot;Enter number of contestants last year >>  #quot;\n in the console"] --> B[Get input from the user.];
B --> C["Display  #quot;Enter number of contestants this year >> #quot;\n in the console"] --> D[Get input from the user.];
D --> E["Display  #quot;Last year's competition had {LastYearEntry} contestants,\n and this year's has {ThisYearEntry} contestants #quot;\n in the console"];
E --> F{Is this year's entry more than\n twice as many contestants as last year?};
F --> |Yes| G["Display  #quot;The competition is more than twice as big this year! #quot; "];
F --> |No| H{Is this year's entry is more than\n contestants than last year,\n but not more than twice as big?};
H --> |Yes| I["Display  #quot;The competition is bigger than ever! #quot;"];
H --> |No| J{Is this year's entry\n smaller than last year's?};
J --> |Yes| K["Display  #quot;A tighter race this year! Come out and cast your vote! #quot;"];
```
