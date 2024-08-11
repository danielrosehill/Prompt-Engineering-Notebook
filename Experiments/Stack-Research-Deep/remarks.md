# Stack Research "Deep"

Date: 11-08-24
GPT: 4o, ChatGPT, Web UI

## Notes

The purpose of this prompting experiment was to see how ChatGPT would do with an "evaluation list" prompt that requested many variables. In this case, 12. 

The next objective was to see whether the same prompt could be used to build a "shortlist" based on very specific criteria - in this case a list of tools meeting the 3 "hard requirements" of having a native Android app, supporting backup (somehow), and with support for markdown. 

Finally, the prompt asked that GPT whittle the shortlist down into an actionable "bottom line" selection of the 3 best tools. 

GPT inferred that they should be ordered by order of preference although the output was a little unclear. 

## Results

At first glance impressive (without verifying too carefully the various details returned).

The output maintained a consistent format for each record it iterated. 

Attempting to re-engineer the prompt to output more results (e.g. "please output 30 suggestions") caused the generation to stop at 11 and throw this:

```
(Additional tools would be listed similarly, providing details as above)
```

But the output could be manually continued by prompting:

```
Add 10 more tools to the evaluation
```

After forcing the additional updates, the `Shortlist` section was regenerated to include the new additions, although the GPT failed to transition to the third section of prompt intended to pick the decisive "winner":

```
Shortlist
Tools that meet the criteria of having an Android app, supporting Markdown, and offering data backup:

Notion
Confluence
Document360
Guru
Slite
Obsidian
Tettra
BookStack
Zendesk Guide
Kipwise
```

## Iterative Improvement 

The final section of the prompt needs improvement:

```
Finally, provide a section called Top 3 GPT Recommendations

Recommend 3 solutions from the shortlist and pick whichever one you think is best and offers the best scalability
```

It should be reworked to be more explicit. An idea for V2 is:

```
Finally, provide a section called Winner, Runner Up

Identify the best solution from those listed in the previous section. Judge the "best" solution by the tool with the best ability to scale. List this under a heading called "The Winner."

Next, identify the second best solution from those listed in the previous section. Use the same criteria as before to make this determination. List this under a heading called "Runner Up"

```