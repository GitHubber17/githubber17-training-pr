THIS TOPIC IS UNDER CONSTRUCTION

# Numbered lists in markdown
To create a numbered list in markdown, specify a number (with a period) at the beginning of the line:
```bash
 9 // In markdown, create a numbered list:
10 1. This is step one.
11 2. This is step two.
12 3. This is step three.
```
To create a nested list in markdown, at the beginning of the line, insert 4 spaces before you specify a number (with a period):
```bash
19 // In markdown, create a nested numbered list:
20 1. This is step one.
21    1. This is sub-step one.
22    2. This is sub-step two.
23    3. This is sub-step three.
24    4. This is sub-step four.
25 2. This is step two.
```
This is published as:
1. One
    i. one
    ii. two
    iii. three
    iv. four
2. Two
    
How you label your steps impacts how the list is numbered and displayed when published.

How you label your steps and specify indentation for step content in markdown impacts how the list is numbered and displayed when published.

When the file is published, the number of steps in the list is calculated and the steps are labled using the label style that you specified in the markdown.
1)
2)
3)

When a step contains content in addition to the step statement, then the manner in which the step content is indented in markdown impacts whether the steps are labeled in correct numerical order when the list is published.
```bash 9
10
11 i. This is step 1.
12    This is additional content for step 1.
13 ii. This is step 2.
14    This is additional content for step 2.
15 iii. This is step 3.
```

#### Specify the step labels
In markdown, steps can be labeled with the same numerical label, such as 1, 1, 1... or they can be labeled in numerical order, such as i, ii, iii, iv... However, how step labels are interpreted and subsequently published is impacted by how the indentation for the step contents is specified in the markdown.

#### Specify indentation for the step contents
In markdown, step contents are indented underneath the step statement by inserting <space> characters before each line of step content. The presence of the <space> characters causes correct numerical ordering and labeling of the steps in Preview.

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
