
![](https://i.imgur.com/iywjz8s.png)


# Collaborative Document Day 3

2024-09-24-ds-intermediate-python.

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: https://tinyurl.com/intermediate-day-3

Collaborative Document day 1: https://tinyurl.com/intermediate-day-1
Collaborative Document day 2: https://tinyurl.com/intermediate-day-2
Collaborative Document day 3: https://tinyurl.com/intermediate-day-3
Collaborative Document day 4: https://tinyurl.com/intermediate-day-4
Collaborative Document day 5: https://tinyurl.com/intermediate-day-5

[Zoom link](https://us02web.zoom.us/meeting/register/tZMvc-2hqjMuHNNKA5ygPA3adR6Q9IkA6ZPP)

##  🫱🏽‍🫲🏻 Code of Conduct

Participants are expected to follow these guidelines:
* Use welcoming and inclusive language.
* Be respectful of different viewpoints and experiences.
* Gracefully accept constructive criticism.
* Focus on what is best for the community.
* Show courtesy and respect towards other community members.
 
## ⚖️ License

All content is publicly available under the Creative Commons Attribution License: [creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/).


## 🙋Getting help
### In the main room
To ask a question, raise your hand in zoom. Click on the icon labeled "Reactions" in the toolbar on the bottom center of your screen, then click the button 'Raise Hand ✋'. For urgent questions, just unmute and speak up!

You can also ask questions or type 'I need help' in the chat window and helpers will try to help you. Please note it is not necessary to monitor the chat - the helpers will make sure that relevant questions are addressed in a plenary way. (By the way, off-topic questions will still be answered in the chat)

### In the breakout room
If you click Ask for Help, it will notify the meeting host that you need assistance and they will be asked to join your breakout room.

Click Ask for Help  in the meeting controls.
Confirm that you would like assistance by clicking Invite Host.
![](https://codimd.carpentries.org/uploads/upload_5b7ea076277616bd16fd9af8ebdb3705.png)


## 🖥 Workshop website

[link](https://esciencecenter-digital-skills.github.io/2024-09-24-ds-intermediate-python)

🛠 Setup

[link](https://esciencecenter-digital-skills.github.io/2024-09-24-ds-intermediate-python#setup.html)

📖 Course Material

[Link](https://carpentries-incubator.github.io/python-intermediate-development/00-setting-the-scene/index.html)


## 👩‍🏫👩‍💻🎓 Instructors

Sven van der Burg, Dani Bodor, Jaro Camphuijsen

## 🧑‍🙋 Helpers
Claire Donnelly, Sander van Rijn

## 🗓️ Agenda day 3
09:00	Welcome + feedback from last week
09:05   Icebreaker in breakout rooms
09:15   Introduction to section 3 (Sven)
09:15	Section 3: Software Development as a Process
10:15	Coffee break
10:30	Section 3: Software Development as a Process
11:30	Coffee break
11:45	Section 3: Software Development as a Process
12:45	Wrap-up
13:00	END


## 🎓 Certificate of attendance
If you attend the full workshop you can request a certificate of attendance by emailing to training@esciencecenter.nl.
Please request your certificate within 8 months after the workshop, as we will delete all personal identifyable information after this period.

## :snowflake: Icebreaker
In breakout rooms:
1. What is something you are proud of?
2. Thinking back about what you learned last time. What are things that were useful? What were things you learned that are overkill for your current work? What questions do you still have?
3. If you have any remaining questions, please 'Call for help?'

## 🧠 Collaborative Notes
* Dead link: 'MVC architecture' & 'software architectural patterns' in the section 'Software Architecture and Design', fixed link: https://carpentries-incubator.github.io/python-intermediate-development/software-architecture-extra/index.html

* Dead link: 'extra episode on functional programming' in section 'Code Refactoring'. Many dead links under the header 'Programming Paradigms' in the section 'Code Refactoring'.
* Typo in solution. The solution for 'Exercise: Testing a Pure Function' refers to the function `compute_standard_deviation_by_data`, this should be `compute_standard_deviation_by_day`
* First link in https://carpentries-incubator.github.io/python-intermediate-development/32-software-architecture-design/index.html#reusable-patterns-of-architecture, should point to: https://www.redhat.com/architect/14-software-architecture-patterns

### The exercise "Add an additional datasource" is broken: 

https://carpentries-incubator.github.io/python-intermediate-development/33-code-decoupling-abstractions/index.html#exercise-add-an-additional-datasource

It refers to a function `load_json` that is missing from the `models.py`. This is the function:

```python
def load_json(filename):
    """Load a numpy array from a JSON document.

    Expected format:
    [
        {
            observations: [0, 1]
        },
        {
            observations: [0, 2]
        }
    ]

    :param filename: Filename of CSV to load

    """
    with open(filename, 'r', encoding='utf-8') as file:
        data_as_json = json.load(file)
        return [np.array(entry['observations']) for entry in data_as_json]

```

### Mocking data source for analyse_data

The analyse_data function is not fully refactored yet:
https://github.com/carpentries-incubator/python-intermediate-development/issues/367
    - The test should fail and the following section should deal with the problem. 

## 🗒 Optional exercises
Here follow some optional exercises for section 3 if you are done early or need some extra practice.
The exercises have an explorative nature, so feel free to go off in any direction that interests you.
You will be looking at some tools that either complement or are alternatives to those already introduced.
Even if you find something that you really like,
we still recommend sticking with the tools that were introduced prior to this episode when you move onto other sections of the course.

### Exercise: Apply to your own project(s)
Apply what you learned in this section to your own project(s). 
This is the time to ask any questions to your instructors or helpers.
Everyone has different preferences for tooling, so getting the input of experienced developers is a great opportunity.

### Exercise: 'advanced object-oriented programming for persistence' and 'databases'
There are two optional extra episodes which you may find interesting.

Both episodes cover the persistence layer of software architectures and methods of persistently storing data, but take different approaches. The episode on [persistence with JSON](https://carpentries-incubator.github.io/python-intermediate-development/persistence/) covers some more advanced concepts in Object Oriented Programming, while the [episode on databases](https://carpentries-incubator.github.io/python-intermediate-development/databases) starts to build towards a true multilayer architecture, which would allow our software to handle much larger quantities of data.


## 💬 Feedback
Please write down one thing that went well and one thing that can be improved.

### 👍 What went well?
- Much of this section is directly applicable to my project, so I took a lot of notes and am going to start applying these today!
- I finally understand what I can use classes for :) x4
- Everything was new for me, it was very very nice, I learnt a lot!x2
- This section really makes you think about how you can rewrite your own code in smaller, more understandable segments. Making it more intuitive for yourself and the eventual user.
- I enjoyed learning about how functions can be broken down into pure functions and why we do this; when I started to applying testing from last weeks lesson to my own code, I quickly saw how "inpure" my functions were, but since this wasn't introduced until this week, I didn't know how to describe this.
- The content is really relevant :) x4
-
- I already have quite some code, and this lesson has taught many ways on improving it (as opposed to writing new 'good' code from scratch).


### 👎 What can be improved?
- Part of this section required implementing tests which would automatically fail, as the functions they apply to were deliberately left unfinished or imperfect. This is not a problem by itself, but it caused some confusion as this was not mentioned in the course.
- Today's lesson was much harder. Almost feels like two weeks/sessions worth of content in one lesson.
- If you try running the analyse_data function it freezes. I guess this is part of a later excerise but it confused me a bit when i was trying to run it
- First URL in the [https://carpentries-incubator.github.io/python-intermediate-development/32-software-architecture-design/index.html#reusable-patterns-of-architecture](https://carpentries-incubator.github.io/python-intermediate-development/32-software-architecture-design/index.html#reusable-patterns-of-architecture) section doesn't work
- I feel like the learning curve skyrocketed today... many things were not clear but that should of course be fixable by studying more this week x2
- Quite a few typos and mistakes in today's lesson, which detracts from the learning experience x3
- It would be great to have some examples of research projects that have a Git repo that we can look at to understand how architecture design can be implemented in real-life examples that are closer to our work.
- A lot of reading in today's lesson, and not so many exercises - especially in the beginning x2
- Maybe not relevant, but I'm not really sure what the code in the main controller is doing with the args Parser and stuff like that, although it's becoming relevant as we're writing code that gets called there. So might be nice to have a small explanation at some point as to what's going on in there.
- I feel like this section made quite some jumps in reasoning, explanation or steps. For example not mentioning the expected error when running the test on analyse_data, not explaining inflammation-analysis a bit more, not telling how you could run inflammation-analysis through the terminal with the new command line parameter --full-data-analysis, etc. For me it caused more confusion than I anticipated.
- The section "Test Using a Mock Implementation" in the "Code Decoupling & Abstractions" chapter is a bit confusing and felt out of place. Especially since the chapter right after goes deeper into testing. For example, I wasn't sure where to put the test function for this, ended up adding it to the test_models.py file (next chapter we are instructed to make a test_compute_data.py file, which makes more sense, why not guide us to make that earlier?) 
- Sometimes the code snippets require us to import specific packages, eg. pathlib.Path in excercise "Write Regression Tests". Only the solution code will show you the package. If you aren't familiar with common python packages it might be hard to know from the skeleton code what packages need to be imported.
- The links for extra episodes on procedural programming, functional programming and object-oriented programming are broken

### Sven's summary
- Last week's material was much harder and longer than week 1 and 2. 
    - This week will likely be easier for most people
    - If there is anything still unclear from last week, ask one of us to explain it to you!
- In section 3 there were many broken links and 'bugs', also the material should give more guidance. It's annoying and we will fix it. We are happy that content-wise you like it.
- Example git repos in resources of today's collab doc (day 4)
- Confusion about command line interface (I will demo it before going into today's section)


### For next time:
* Finish section 3, we will start collaboration in section 4 so you need to be in sync with your group. If you really don't have time it is OK if you do not fully finish section 3, just make sure you merge everything cleanly.


## ❓ Homework questions:
Put any questions that come up during homework here: We try to check this document for questions daily:
- Q: I am having trouble merging full-data-analysis into develop. It's giving conflicts because there is new code in both. I forgot I was supposed to rebase on develop in the beginning.. What to do?
- A: You have to resolve the conflicts. You can do that manually by editing the files. Then commit if you are happy. This is a bit cumbersome though and I prefer using PyCharm's tool for it: https://www.jetbrains.com/help/pycharm/resolve-conflicts.html Can you try if this solves your problem? 
- Q: I think the solution in the "Benefits of Pure Functions" section contradicts a previous solution that changed the analyse_data() function to work with classes, as suddenly the function does not use classess anymore.
- A: Yes you are right [this solution](https://carpentries-incubator.github.io/python-intermediate-development/33-code-decoupling-abstractions/index.html#solution-1) indeed comes before that and uses the `CSVDataSource` class. We will make sure the lesson material will be updated. See [this issue](https://github.com/carpentries-incubator/python-intermediate-development/issues/394)
-
-



## 📚 Resources
Books that teach you little advanced Python tricks one at a time. The nice thing is that you can read a few pages on a specific trick once in a while.
- [Book: 'Effective Python: 90 specific ways to write better Python](https://www.goodreads.com/book/show/48566725-effective-python)
- [Book: Python tricks: A buffet of awesome Python features](https://www.goodreads.com/book/show/36990732-python-tricks)
