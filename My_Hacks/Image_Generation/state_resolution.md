# State The Resolution

Getting DALLE to adhere to requests to generate at specific resolutions is still (in my experience, at least) hit and miss.

Knowing the output resolution is very useful, however. 

You may have pseudotext or other imperfections that you wish to clean up. 

While it's trivially easy to determine the output resolution by opening the generated image in a browser, you can save time by having GPT tell you this parameter up front in the chat. 

## Prompt Snippet

I've found that you can append this to the image generation prompt:

```
After generating the image, please state its resolution in pixels.
```
And GPT will output the parameter after generating the image. 

## Example

![Instructing GPT to output the resolution after generating the image](../../images/resinstructions.png)