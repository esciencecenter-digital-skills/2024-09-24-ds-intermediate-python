
![](https://i.imgur.com/iywjz8s.png)


# Collaborative Document Day 2

2024-09-24-ds-intermediate-python.

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: https://tinyurl.com/intermediate-day-2

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


## 🗓️ Agenda day 2
09:00	Welcome + feedback from last week
09:05   Icebreaker in breakout rooms
09:15   Introduction to section 2 (Sander)
09:15	Section 2: Ensuring Correctness of Software at Scale
10:15	Coffee break
10:30	Section 2: Ensuring Correctness of Software at Scale
11:30	Coffee break
11:45	Section 2: Ensuring Correctness of Software at Scale
12:45	Wrap-up
13:00	END


## 🎓 Certificate of attendance
If you attend the full workshop you can request a certificate of attendance by emailing to training@esciencecenter.nl.
Please request your certificate within 8 months after the workshop, as we will delete all personal identifyable information after this period.

## :snowflake: Icebreaker
In breakout rooms:
1. What is something that not many people know about you? (And you are willing to share)
2. Thinking back about what you learned last time. What are things that were useful? What were things you learned that are overkill for your current work? What questions do you still have?
3. If you have any remaining questions, please 'Call for help?'

## 🧠 Collaborative Notes

> **[!IMPORTANT]**
> In the '[Improving Robustness with Automated Code Style Checks](https://carpentries-incubator.github.io/python-intermediate-development/24-diagnosing-issues-improving-robustness/index.html#improving-robustness-with-automated-code-style-checks)' section of today's final episode ('Diagnosing Issues and Improving Robustness') you can replace the following instruction:
> `$ git switch -c pylint-ci develop`
> with
> `$ git switch test-suite`
> instead. This is a known issue with the lesson material that will cause conflicts in later episodes.
> 

- Known problem on Windows: typing `python` in Git Bash 'hangs' and does not respond:
  - Paste the following command: `echo "alias python='winpty python.exe'" >> ~/.bashrc`
  - Restart Git Bash
  - Typing `python` should now work
  If not, please get in touch! Solution source: [StackOverflow](https://stackoverflow.com/questions/32597209/python-not-working-in-the-command-line-of-git-bash)
- Does the file remain empty when using `winpty python -m pip freeze > requirements.txt`? Adjust the alias to `alias python='winpty -Xallow-non-tty python'`
  - If that in turn adds strange characters, extend it further to  `alias python='winpty -Xallow-non-tty -Xplain python`
  - [Solution source](https://superuser.com/a/1322277/519432)

In the CI 

#### Error related to pylintrc file

If you get an error similar to this: 
  `UnicodeDecodeError: 'utf-8' codec can't decode byte 0xff in position 0: invalid start byte.`
  It may be that PyCharm is not writing files in utf-8 format. This can be fixed by incuding the encoding option: https://stackoverflow.com/questions/52418511/pylint-unicodedecodeerror-utf-8-cant-decode-byte
  or by changing your settings in PyCharm:https://discuss.streamlit.io/t/unicodedecodeerror-utf-8-codec-cant-decode-byte-0xff-in-position-0-invalid-start-byte/23429
  


## 🗒 Optional exercises
Here follow some optional exercises for section 2 if you are done early or need some extra practice.
The exercises have an explorative nature, so feel free to go off in any direction that interests you.
You will be looking at some tools that either complement or are alternatives to those already introduced.
Even if you find something that you really like,
we still recommend sticking with the tools that were introduced prior to this episode when you move onto other sections of the course.

### Exercise: Apply to your own project(s)
Apply what you learned in this section to your own project(s). 
This is the time to ask any questions to your instructors or helpers.
Everyone has different preferences for tooling, so getting the input of experienced developers is a great opportunity.

### Exercise: Branch coverage versus line coverage
For your test coverage, have a look at the concept of 
[branch coverage](https://about.codecov.io/blog/line-or-branch-coverage-which-type-is-right-for-you/)
as opposed to just line coverage. 
Which do you prefer and why?

### Exercise: Desirable test coverage
Look at the projects below and see how much test coverage they have. 
Should 100% line (or branch) coverage always be the goal? Why or why not?
- [pytest](https://github.com/pytest-dev/pytest)
- [pyjokes](https://github.com/pyjokes/pyjokes)
- [scikit-learn](https://github.com/scikit-learn/scikit-learn)

### Exercise: Coverage badges
Try to add a [coverage badge](https://github.com/marketplace/actions/coverage-badge) to the inflammation project.

## ❓ Questions regarding homework
- Q: After finishing today's exercises, I checked again on GitHub and noticed that all workflow runs after adding the .pylintrc file were failing. I made sure to edit my main.yml file to remove the fail-under argument to avoid redundancy, but still the runs fail. I can't seem to find why this happens - Jorick
- A: Let's have a look together today! Can you paste a link to the failing pipeline?
- A-to-A: https://github.com/JorickLania/python-intermediate-inflammation/actions
-
-
-
-



## Feedback
Please write down one thing that went well and one thing that can be improved.

### 👍 Tops
- The information in this workshop was presented very clearly, and the tutorial was easy to follow. It taught me a great deal of new concepts that will be directly applicable to my work, as it focusses on improving, debugging and modulating existing code.
- Content + (self-)pace are perfect. Great session again. Instructors are great too! x4
- The icebreaker helped to have a nicer start to the day x2
- I like the pacing of the course: learning something new and then having a week to apply it in my own work
- I like how instructors sometimes pop up in the breakout room and ask questions about how useful things are for us. It makes me feel they are really interested in our growth <3
- Instructors are fast with helping out with questions.
- Loved today's class, tutorial is so easy to follow
- I was so happy to finally get more explanation on github actions! They were a bit mysterious to me for a long time
- I was happy to learn more about testing and how you teach it very from the ground up to implement it well. Also the taught material of week 1 is nicely incorporated which makes it more memorable. x2
- It is great that everyone can work on their own pace in the beginning few sessions! And that there are optional assignments if you are done faster.

### 👎 Tips
- Extremely minor, this link in the set-up section doesn't work for me https://esciencecenter-digital-skills.github.io/2024-09-24-ds-intermediate-pythonsetup.html
- The testing section ends with an explanation on TDD. It would have been nice if the debugging section followed this approach so we could practice with it.
- I agree with the above (about TTD), while I understand the concept, it is still quite hard to visualize how it would go in practice, especially if the project would be more complex. Some examples or assignments with this would be nice!
- =
- I had (not only me) a couple of issues when switching from GitBash to PyCharm for some steps (nothing major), I would like to know in which exact situations can we expect them to be changed synchronically or how to do this switching more smoothly
    - What kind of issues?
- 

### Summary of feedback
- Set-up link in collab doc fixed! Thank you for informing us!
- We should add some practice with test-driven development to make it more concrete. One simple example in which I often apply it: 
    1. You find a bug in a specific situation
    2. You write a (failing) test that mimics this situation
    3. You run the test and use debugger to find the problem
    4. You fix the bug
    5. You commit both the test and the bug fix
- Issues GitBash - PyCharm, please show us what you mean in the breakout rooms!

## 📚 Resources

- A (way) more advanced way of parametrizing your tests can be done with the [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) package: It can generate all kinds of complex inputs for you, but the flip side is that it cannot generate expected outputs for you. You'll have to write your tests in such a way that you can test for _properties_ of the output, also called property based testing
