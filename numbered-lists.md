# Numbered lists in markdown

When creating numbered lists in markdown, several things must be considered:
- The formatting style to use for the step labels
- Whether steps will contain content in addition to the step statement
- The amount of indentation to apply to the step contents

How you label your steps and specify indentation for step content in markdown will impact how the list is numebred and displayed when published.

To create a numbered list in markdown, you specify a number at the beginning of the step statement, such as 1, 1a, A, and so on.
```bash 9
10
11 1. This is step one.
12 2. This is step two.
13 3. This is step three.
```
When the file is published, the number of steps in the list is calculated and the steps are labled using the label style that you specified in the markdown.
```bash 9
10
11 1) This is step one.
12   1a) This is step 1a.
13   1b) This is step 1b.
14 2) This is step two.
15   2a) This is step 2a.
```
When a step contains content in addition to the step statement, then the manner in which the step content is indented in markdown impacts whether the steps are labeled in correct numerical order when the list is published.
```bash 9
10
11 A. This is step A.
12    This is additional content for step A.
13 B. This is step B.
14    This is additional content for step B.
15 C. This is step C.
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
1. Statement sentence for step number one.
    ```bash
       step content: fist and last lines indented 4 <space>s, middle line indented 7 <space>s
    ```
1. Statement sentence for step number two.
    ```bash
step content: fist and last lines indented 4 <space>s, middle line not indented
    ```
1. Statement sentence for step number three.
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

### Hope you enjoyed this tutorial!
