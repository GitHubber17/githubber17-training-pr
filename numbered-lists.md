
THIS TOPIC IS UNDER CONSTRUCTION

# Numbered lists in markdown
To create a numbered list, specify a number (with a period) at the beginning of the line:
```bash
10 1. This is step one.
11 2. This is step two.
12 3. This is step three.
```
Note that you do not need to specify the correct number for a step according to the total number of steps in the list. This is helpful when working with long lists or large amounts of content, where it is difficult to track your exact place in the list while authoring. At the beginning of the line, simply specify a number followed by a period and when the list is published, the build process will calculate the number to display next to each step. For example, if you accidentally misnumber steps during authoring:
```bash
10 1. This is step one.
11 2. This is step two.
12 3. This is step three.
13 3. This is step four.
14 4. This is step five.
15 6. This is step six.
16 7. This is step seven.
17 7. This is step eight.
18 8. This is step nine.
```
The steps are correctly numbered when the article is published:
1. This is step one.
2. This is step two.
3. This is step three.
3. This is step four.
4. This is step five.
6. This is step six.
7. This is step seven.
7. This is step eight.
8. This is step nine.

To create a nested list, at the beginning of the line, insert _4 spaces_ before you specify the number:
```bash
20 1. This is step one.
21     1. This is nested step one.
22     1. This is nested step two.
23 1. This is step two.
```
This is published as:
1. This is step one.
    1. This is nested step one.
    1. This is nested step two.
1. This is step two.

When a step contains content after the step statement, at the beginning of each line, insert _4 spaces_ before you specify the content. Otherwise, the steps will not be labeled in correct numerical order when the list is published.

```bash
30 1. This is step one.
31
32     More content for step one.
33     Even more content for step one.
34 1. This is step two.
35
36     More content for step two.
37     Even more content for step two.
38 1. This is step three.
```
This is published as:
1. This is step one.

    More content for step one.    
    Even more content for step one.
1. This is step two.

    More content for step two.    
    Even more content for step two.
1. This is step three.



In addition, a new line must be entered after each line of content to prevent the content lines from being appended together in the published view.

```bash
30 1. This is step one.
31
32     More content for step one.
33     Even more content for step one.
34 1. This is step two.
35
36     More content for step two.
37     1. This is nested step one.
38     1. This is nested step two.
39
40     Even more content for step two.
41 1. This is step three.
```
This is published as:
1. This is step one.

    More content for step one.    
    Even more content for step one.
1. This is step two.

    More content for step two.
    1. This is nested step one.
    1. This is nested step two.
    
    Even more content for step two.
1. This is step three.

