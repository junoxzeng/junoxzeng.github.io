---
layout: essay
type: essay
title: "Smart Questions, Good or Bad?"
# All dates must be YYYY-MM-DD format!
date: 2025-09-11
published: true
labels:
  - Smart Questions
  - StackOverflow
---


## Smart Questions and Smart Engineers
When thinking of software engineering, the ability to code and problem solve is paramount to the success of a career. However, how do newcomers develop that skill? The ability to ask a well formed question is just as valuable as writing good code because it not only saves the time by being clear and efficient but will also help the community as a whole. The quality of a question is often linked to the quality of response that it will receive and this especially holds true in a community like Stack Overflow who is volunteer based and can have a wide variety of skill levels and personalities.

## Simple, Direct, Fast
One example of a smart question that was asked by a user on StackOverflow was "Can I use comments inside a JSON  file? If so, How?" The question is very direct and gets to the problem. It specifies the specific language, JSON, and clearly lets you the reader know what the user wants to ask. It was especially relevant as well towards the public as a whole since during the time it was published which was almost 17 years ago, there wasn't the convenience of being able to lookup the answer which made learning a new coding language especially difficult. This in turn allowed the question to become more universal as anyone learning JSON might have this question.

```
No.

JSON is data-only. If you include a comment, then it must be data too.

You could have a designated data element called "_comment" (or something) that should be ignored by apps that use the JSON data.

You would probably be better having the comment in the processes that generates/receives the JSON, as they are supposed to know what the JSON data will be in advance, or at least the structure of it.

```
By being so direct and concise, the user received responses that were direct, clear, and concise. The top response which is shown above explained the problem simply and also offered a solution or alternative that could be used. This was one of the earliest examples of a smart question being asked being especially relevant as it is still one of the most viewed questions on stack overflow till this day.

Here is a link to [StackOverflow](https://stackoverflow.com/questions/244777/can-comments-be-used-in-json)


## How to get Ignored

While there is no such thing as a "dumb" question, there is a way to ask questions that will be unproductive and frustrating for others to answer. In this example, the user asked the question shown down below.

```
This question is analogous to How to keep Visual Studio autocomplete from overwriting the next word, but targeted at Visual Studio Code instead of Visual Studio.

When a completion suggestion is selected from the list, it is inserted, but all characters from the word after the cursor are deleted. (So, nothing happens if there is a whitespace after the cursor. But if autocompletion is triggered while the cursor is placed at the beginning of a word, said word will be deleted).

Is there a way to disable this deletion behavior and get it to add the selected suggestion without deleting text to the right of the caret?
```
While this is still a relatively great question to ask and it is asked in a great way, there is still some missing elements that keep it from being a great question. It firstly lacked some detail such as the specific VS code version and language that they were having problems with. Second of all is that the question is too broad, is it only on certain languages they are having with? Is it a question about IntelliSense generally or is it a problem with VS Code? As a result, the responses that they received were more general and not as focused. The top upvoted response could only help by suggesting they go into the settings and to turn off the default behavior and that they might need to check certain languages whether the default is changed which makes the response to the question more broad. The insufficient detail leads to a reponse that isn't as clear cut of a solution to the question at hand

Here is a link to [StackOverflow](https://stackoverflow.com/questions/75448674/how-to-prevent-vs-code-from-deleting-the-next-word-characters-on-intellisense-au)

##

## Conclusion

When we rely on others’ generosity and expertise to provide answers to our questions, it should hold that the question we ask should be one that leads to efficient and effective help that not only benefits us, but also the people we ask and others who might ask the same question in the future. Thus, if you have a question… make it a smart one! Asking questions may not always get you the best answer, but asking them in a way that will make others want to answer them will increase the success of finding a good solution and make it a positive experience on all sides.
