#githubber17-training-pr
A private (albeit public) repo for training purposes.

## MARKDOWN

### Numbered lists
When creating numbered lists, you must consider:
- The formatting style for the step labels
- The amount of indentation for the step contents

How step labels and content indentation are specified in markdown impacts how the list is rendered in Preview.

#### Create a numbered list
To create a numbered list in markdown, specify a number at the beginning of the step statement, such as 1, 1a, A, and so on.
When the file is rendered in Preview, the number of steps in the list is calculated and the steps are relabled as 1, 2, 3..., according to the label style that you specified. However, there is an exception to this behavior.

#### Specify the step labels
In markdown, steps can be labeled with the same numerical label, such as 1, 1, 1... or in numerical order, such as i, ii, iii, iv... However, how step labels are interpreted and subsequently rendered in Preview is impacted by how the indentation for the step contents  is specified in the markdown.

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
