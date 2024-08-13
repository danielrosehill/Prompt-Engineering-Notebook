# Prompts For Developing & Optimising Prompt-Recording System

*13-08-24*

One of the truly outstanding facets of ChatGPT is its ability to provide outputs on how to use it (ie itself!) more effectively. To the best of my knowledge, no *"name"* has been invented yet to describe the phenomenon of ChatGPT instructing humans on how to use it most effectively (I could be wrong about this!). In the abscence of a better descriptor, I have begun to call it *"self guidance"*."

One particularly helpful ability of ChatGPT in this respect is its ability to provide suggestions on how to work with it most effectively. ChatGPT can advise upon:

- Developing workflows involving third-party APIs and custom scripting
- Systems for storing prompt outputs and creating prompt libraries
- Workflows for validating prompt outputs and prompt engineering
- Developing taxonomies for organising GPT output

## ChatGPT, Please Help Me To Build A ChatGPT System!

A prompting strategy I have used successfully involves asking ChatGPT to help develop the system I am building on top of NocoDB for logging outputs. 

While this could probably be achieved with a custom GPT, prompt engineering has an advantage when it comes to commonly changing contexts (like the constituion of my 'system'). Either strategy could work well. 

Fundamental to the design of data-logging systems is capturing the right data, which is why developing taxonomies is so important. 

## Model Prompts

Here are some model prompts which use ChatGPT to suggest a more comprehensive structure for a data table. The focus is on providing a detailed overview of the system and then asking specifically for new data to capture:

### Suggest New Fields To Capture

```
I am currently using NocoDB to develop a system for logging and recording details of my work with ChatGPT. Help me to make my workflow for capturing prompt outputs as effective as possible. Please suggest 10 fields about prompt outputs that I should be capturing in my database. For every field you suggest capturing, please explain why it would be helpful.
```
### Suggest New Fields To Capture With The Recommended Format

A variation might entail adding a request to suggest the appropriate data field type for your particular database (for example, MySQL):

```
I am currently using NocoDB to develop a system for logging and recording details of my work with ChatGPT. It's a MySQL database. Help me to make my workflow for capturing prompt outputs as effective as possible. Please suggest 10 fields about prompt outputs that I should be capturing in my database. For every field you suggest capturing, please explain why it would be helpful. Please also recommend the most appropriate data type for that field in MySQL.
```

###  Here's What I'm Capturing. What Could I Be Missing?

Finally, you could consider providing ChatGPT with your current schema and ask it to "fill in the gaps":

```
My dearest ChatGPT,

I'm currently using NocoDB to log and capture my ChatGPT prompts and outputs. As you know, NocoDB is a management interface for a relational database. 

Here are the fields which I am currently capturing for logging ChatGPT outputs:

- Date of output
- Unique ID for output
- Output text

Please suggest 5 additional fields which I could be capturing in my database. For every new field that you suggest, please explain why it would be useful to add it. 
```

Etc, etc. 
