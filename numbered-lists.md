THIS TOPIC IS UNDER CONSTRUCTION

# Numbered lists in markdown
To create a numbered list, specify a number (with a period) at the beginning of the line:
```bash
10 1. This is step one.
11 2. This is step two.
12 3. This is step three.
```
To create a nested list, at the beginning of the line, insert _4 spaces_ before you specify the number:
```bash
20 1. This is step one.21     1. This is nested step one.
22     2. This is nested step two.
23 2. This is step two.
```
This is published as:
1. This is step one.
    1. This is nested step one.
    2. This is nested step two.
2. This is step two.


When a step contains content after the step statement, at the beginning of each line, insert _4 spaces_ before you specify the content. Otherwise, the steps will not be labeled in correct numerical order when the list is published.
```bash
30 1. This is step one.
31     More content for step one.
32     Even more content for step one.
33 2. This is step two.
34     More content for step two.
35     1. This is nested step one.
36     2. This is nested step two.
37     Even more content for step two.
38 3. This is step three.
```
This is published as:
1. This is step one.

    More content for step one.
    
    Even more content for step one.
2. This is step two.

    More content for step two.
    
    1. This is nested step one.
    2. This is nested step two.
    
    Even more content for step two.
3. This is step three.

##### Example: INCORRECT, missing all indentation
In the markdown, no <space> characters are inserted before the lines of step content.
As a result, the step numbering is not correctly calculated and the steps are all labeled as "1" in Preview.
1. Statement sentence for step number one.
```bash
step content: no indentation applied
```
1. Statement sentence for step number two.
```bash
step content: ...
```
1. Statement sentence for step number three.
```bash
step content: ...
```

##### Example: INCORRECT, missing some indentation
In the markdown, <space> characters are inserted before some lines of step content, but not all lines of step content.
As a result, the step numbering is not fully calculated and there are multiple steps labeled as "1" in Preview.
A) Statement sentence for step number one.
    ```bash
       step content: fist and last lines indented 4 <space>s, middle line indented 7 <space>s
    ```
A) Statement sentence for step number two.
    ```bash
step content: fist and last lines indented 4 <space>s, middle line not indented
    ```
A) Statement sentence for step number three.
```bash
   step content: fist and last lines not indented, middle line indented 3 <space>s
```

##### Example: CORRECT, all indentation applied
In the markdown, all steps are labeled as "1", <space> characters are inserted before each line of step content.
As a result, the step numbering is correctly calculated and the steps are labeled as "1, 2, 3" in Preview.
1. Statement sentence for step number one.
    ```bash
       step content: fist and last lines indented 4 <space>s, middle line indented 7 <space>s
    ```
1. Statement sentence for step number two.
    ```bash
       step content: ...
    ```
1. Statement sentence for step number three.
    ```bash
       step content: ...
    ```
