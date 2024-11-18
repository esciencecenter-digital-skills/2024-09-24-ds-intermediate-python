
![](https://i.imgur.com/iywjz8s.png)


# Collaborative Document Day 4

2024-09-24-ds-intermediate-python.

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: https://tinyurl.com/intermediate-day-4

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

[link](https://esciencecenter-digital-skills.github.io/2024-09-24-ds-intermediate-python#setup)

📖 Course Material

[Link](https://carpentries-incubator.github.io/python-intermediate-development/00-setting-the-scene/index.html)


## 👩‍🏫👩‍💻🎓 Instructors

Sven van der Burg, Dani Bodor, Jaro Camphuijsen

## 🧑‍🙋 Helpers
Claire Donnely, Sander van Rijn, Ewan Cahen

## 🥶 Icebreaker
1. What is the thing you like the most about your work?
2. Thinking back about what you learned last time. What are things that were useful? What were things you learned that are overkill for your current work? What questions do you still have?
3. If you have any remaining questions, please 'Call for help'


## 🗓️ Agenda day 4
09:00	Welcome and icebreaker
09:15	Section 4: Collaborative Software Development for Reuse
10:15	Coffee break
10:30	Section 4: Collaborative Software Development for Reuse
11:30	Coffee break
11:45	Section 4: Collaborative Software Development for Reuse
12:45	Wrap-up
13:00	END


## 🎓 Certificate of attendance
If you attend the full workshop you can request a certificate of attendance by emailing to training@esciencecenter.nl.
Please request your certificate within 8 months after the workshop, as we will delete all personal identifyable information after this period.


## 🧠 Collaborative Notes

Example of pull request: https://github.com/carpentries-incubator/python-intermediate-development/pull/375

### Patient class
You can use below code it you want to add the missing `Patient` class. For example if you want to work on the `persistence` or `databases` extra episodes.

```python
class Observation:
    def __init__(self, day, value):
        self.day = day
        self.value = value

    def __str__(self):
        return str(self.value)

class Patient:
    """A patient in an inflammation study."""
    def __init__(self, name):
        self.name = name
        self.observations = []

    def add_observation(self, value, day=None):
        if day is None:
            try:
                day = self.observations[-1].day + 1

            except IndexError:
                day = 0

        new_observation = Observation(day, value)

        self.observations.append(new_observation)
        return new_observation

    def __str__(self):
        return self.name


alice = Patient('Alice')
obs = alice.add_observation(3)
```

### Teaching material bugs

- In section "Developing Software In a Team: Code Review", [solution to first exercise](https://carpentries-incubator.github.io/python-intermediate-development/41-code-review/index.html#exercise-review-some-code): "Not clear what variable `number` contains - better option is a business-logic name like mean or mean_of_data." - there is no variable `number`, but `mmm`.


## 🗒 Optional exercises
Here follow some optional exercises for section 1 if you are done early or need some extra practice.
The exercises have an explorative nature, so feel free to go off in any direction that interests you.
You will be looking at some tools that either complement or are alternatives to those already introduced.
Even if you find something that you really like,
we still recommend sticking with the tools that were introduced prior to this episode when you move onto other sections of the course.

### Exercise: Apply to your own project(s)
Apply what you learned in this section to your own project(s). 
This is the time to ask any questions to your instructors or helpers.
Everyone has different preferences for tooling, so getting the input of experienced developers is a great opportunity.

### Exercise: GitHub collaboration
- As you've now seen, Pull Requests are a helpful way to keep new features separate until they've been reviewed. To force this behavior, even for yourself, you can [**protect**](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule#creating-a-branch-protection-rule) a branch in GitHub. Try this for yourself, and see what happens if you still commit to main locally and try to push it. How would you fix this when it happens?

### Exercise: Packaging
- Have a look at the [Python Packaging Guide](https://packaging.python.org/en/latest/)
- Try actually publishing your code to [test.pypi.org](https://test.pypi.org) based on the above guide

## 💬 Feedback
Can you provide is with feedback of todays session? Can you write down one thing that went well and one thing that can be improved?

### 👍 What went well:
- It was very helpful to learn about how pull requests work because, even if you don't use them in your own work, you often encounter them when searching for solutions to errors online. The part on packaging was also nice to demistify packages and see that it is actually relatively easy to get started with them.
- Great to demystify many github features related to collaboration. Learned a lot!(x2)
- Appreciate the emphasis on the human aspect of collaboration. Not just technically 'how does a code review work', but also what your tone should be and focus on empathy and constructive attitude. x4
- Really want to state that I appreciate how feedback to the workshop is handled; ending each day with writing some stuff down and starting the next session with reviewing what things went well and what could improve for a next time. Amazing! :) 
- Great to start working together with other students in the group x2
- Great tips and feedback from the instructors
- I actually appreciated that it used a somewhat outdated branch and was not a straightforward merge. Often in courses you get these kind of ideal situations and then irl you run into a bunch of issues that you have not seen before. So I appreciated getting a bit more practice with this. x2

### 👎 Can be improved:
- I was a bit confused by the feature-std branch that we had to use today for the pull requests because the branch is outdated relative to what we covered in previous weeks, at least in my repository, so when we merge it into develop to resolve the pull request I lost a sizeable amount of functions and tests. This may be my fault though :)
    - +3 on the confusion about using an outdated branch as a starting point
- The heading of section 4.3 "Software release" is broken.
- Sometimes it is not immediately clear from the exercise in which branch we should be working at a given time; often this becomes clear a little later in the section, but it can cause some confusion. (x2)
- I think the introduction to the code review/pull-request workflow can be improved by providing a full overview (maybe with a diagram) what the entire flow looks like. 
- Maybe it is just lack of prior knowledge, but it took a bit of time to figure out how merge conflicts, specifically the complicated ones, could be resolved. As in; how do you read the feedback git gives when trying to resolve. It might be nice to elaborate a bit on that somewhere in the course. 
- Clear instruction not to create your pull request from the python-incubator main repository as a base, but instead the main branch of your own repository.
- It wasn't super clear what the function s_dev() we were working on was supposed to do, calculate a daily standard deviation or one across the whole data - This caused some confusion in our group's code review since we both understood it differently. x2

### Sven's summary
- Happy to see that you liked last weeks topics! Some of you even speak about demystification, wow! 👍
- There was quite some confusion around creating the pull request and the merge conflicts that arose. Although some people liked it because it felt more like the real world :) 
    - We think the material should give more guidance here so we wrote down what to improve
    - If we have time we will go a bit deeper in merge conflict resolution
- Remember you can use the breakout rooms to clear up anything that you still think is unclear from last week


## Next week:
No strong dependencies on what you did the first 4 weeks (apart from knowing the project and having it forked). So up to you if you want to finish section 4 (but we recommend doing so because you can still ask questions).

Same zoom link, starting at 9:00 sharp (you can join from 8:45). See you next week! 

## Questions regarding homework after week 4.
- Q:
- A:
- Q:
- A:
- Q:
- A:

## 📚 Resources
Example projects (please add if you have good examples):
- [ESMValTool: A community diagnostic and performance metrics tool for routine evaluation of Earth system models in CMIP](https://github.com/ESMValGroup/ESMValTool)
- [The Citation File Format lets you provide citation metadata for software or datasets in plaintext files that are easy to read by both humans and machines.](https://github.com/citation-file-format/citation-file-format)
- [An open-source deep learning framework for data mining of protein-protein interfaces or single-residue variants.](https://github.com/DeepRank/deeprank2) --> See for example [this class representing an amino acid](https://github.com/DeepRank/deeprank2/blob/78e2773634399433063fc4dd30fa7f6066c1fcae/deeprank2/molstruct/aminoacid.py#L23)