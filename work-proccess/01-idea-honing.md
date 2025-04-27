# idea honing honing  (starting a new project)

 if you are starting a new project  you can use conversational LLMs like ChatGPT 4o/o3 to hone your idea. The AI will ask one question at a time to develop a thorough spec. Save the output as `spec.md` in the `docs` folder in this repository.


use this prompt to get started:
```
Ask me one question at a time 
so we can develop a thorough, step-by-step spec for this idea. 
Each question should build on my previous answers, 
and our end goal is to have a detailed specification I can hand off to a developer. 
Let's do this iteratively and dig into every relevant detail. 
Remember, only one question at a time.

Here's the idea:

<IDEA>
```
At the end of the brainstorm (it will come to a natural conclusion):
```
Now that we've wrapped up the brainstorming process, 
can you compile our findings into a comprehensive, developer-ready specification? 
Include all relevant requirements, architecture choices, 
data handling details, error handling strategies, 
and a testing plan so a developer can immediately begin implementation.
This will output a pretty solid and straightforward spec that can be handed off to the planning step. I like to save it as `spec.md` in the repo.
```

## Editing the Spec

Once the AI agent has created the spec, you can review and edit it as needed. Make sure to check for any errors or inconsistencies in the spec. You can also add any additional information or context that may be helpful for the developer who will be working on the project.

### Adding Additional Information
If you want to add additional information/ change things, you can use the following prompt:
```
Thank you! The spec is written well, but I would like to add some additional information. Please add the following information to the spec:
<additional information>
```

### Changing the Spec Description
If you want to change the spec description, you can use the following prompt:
```
Thank you! The spec is written well, but I would like to change the spec description. Please change the spec description to:
<change spec description/ additional information>
```