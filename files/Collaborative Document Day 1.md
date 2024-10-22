
![](https://i.imgur.com/iywjz8s.png)


# Collaborative Document Day 1

2024-09-24-ds-intermediate-python.

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: https://tinyurl.com/intermediate-day-1

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

You can email training@esciencecenter.nl if you feel this code was violated and feel uncomfortable saying it directly.

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

[link](https://esciencecenter-digital-skills.github.io/2024-09-24-ds-intermediate-python/#setup)

📖 Course Material

[Link](https://carpentries-incubator.github.io/python-intermediate-development/00-setting-the-scene/index.html)


## 👩‍🏫👩‍💻🎓 Instructors

Sven van der Burg, Dani Bodor, Jaro Camphuijsen

## 🧑‍🙋 Helpers
Claire Donnely, Sander van Rijn


## 🗓️ Agenda day 1

09:00	Welcome and icebreaker
    - Collaborative document
    - eScience Center introduction
    - Workshop introduction
09:30	Section 1: Setting up Environment For Collaborative Code Development
10:15	Coffee break
10:30	Section 1: Setting up Environment For Collaborative Code Development
11:30	Coffee break
11:45	Section 1: Setting up Environment For Collaborative Code Development
12:45	Wrap-up
13:00	END


## 🎓 Certificate of attendance
If you attend the full workshop you can request a certificate of attendance by emailing to training@esciencecenter.nl.
Please request your certificate within 8 months after the workshop, as we will delete all personal identifiable information after this period.

## :snowflake: Icebreaker
If you can be an animal for one day. Which animal would you pick and why?



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

### Exercise: Try out different Integrated Development Environments
Install different Integrated Development Environments (IDEs) and test them out.
Which one do you like the most and why?
You can try: 
- [Visual Studio Code](https://code.visualstudio.com/), with setup instructions [in the Extras of this course](https://carpentries-incubator.github.io/python-intermediate-development/vscode/index.html)
- [Atom](https://atom-editor.cc/)
- [Sublime Text](https://www.sublimetext.com/)
- [RStudio](https://posit.co/download/rstudio-desktop/)

Technically, compared to PyCharm, the 'IDEs' listed above are source code editors capable of functioning as an IDE 
(with RStudio as an example).
To function as an IDE, you have to manually install plugins for more powerful features 
such as support for a specific programming language or unit testing. 
What do you prefer, a lot of tooling out of the box or a lightweight editor with optional extensions?

If you want an even more lightweight setup you can try out these configurable source code editors:
- [Emacs](https://www.gnu.org/software/emacs/)
- [Vim](https://www.vim.org/)

### Exercise: Customize the command line
You can customize the command line or use alternatives to `bash` to make yourself more productive.
- Try out [z](https://github.com/rupa/z), a simple tool to more quickly move around directories.
- Try out [Z shell (zsh)](https://zsh.sourceforge.io/), a shell designed for interactive use.
- Try out [Oh My ZSH](https://ohmyz.sh/), which is a theming and package manager of the `zsh` terminal.
- Try out [fish](https://fishshell.com/), a smart and user-friendly command line shell.
- Try out [Bash Prompt Generator](https://bash-prompt-generator.org/), it lets you try out different prompts, 
depending on the information you want displayed.

### Exercise: Try out different virtual environment managers
So far we used `venv`, but there are other virtual environment managers for Python:
- [Poetry](https://python-poetry.org/).
- conda, which is part of [Anaconda Distribution)](https://www.anaconda.com/download). 
Anaconda is widely used in academia, but the current license does not allow use for research in most circumstances. 
An open-source alternative is [mini-forge](https://github.com/conda-forge/miniforge).

### Exercise: Customize `pylint`
You decide to change the max line length of your project to 100 instead of the default 80. 
Find out how you can configure pylint. You can first try to use the pylint command line interface, 
but also play with adding a configuration file that pylint reads in.


## Collaborative Notes

- Known problem on Windows: typing `python` in Git Bash 'hangs' and does not respond:
  - Paste the following command: `echo "alias python='winpty python.exe'" >> ~/.bashrc`
  - Restart Git Bash
  - Typing `python` should now work
  If not, please get in touch! Solution source: [StackOverflow](https://stackoverflow.com/questions/32597209/python-not-working-in-the-command-line-of-git-bash)
- Does the file remain empty when using `winpty python -m pip freeze > requirements.txt`? Adjust the alias to `alias python='winpty -Xallow-non-tty python'`
  - If that in turn adds strange characters, extend it further to  `alias python='winpty -Xallow-non-tty -Xplain python`
  - [Solution source](https://superuser.com/a/1322277/519432)


## ❓ Questions regarding homework
- I forgot to ask whether it is expected that Git asks for the passphrase everytime you push to origin. I thought it would not be necessary once you have the key linked, but I keep having to input the passphrase. Did I configure something wrongly?
  - Windows or Mac or Linux? --> Windows!
  - Probably you have set a password on your SSH-key? The trick is to set an empty passphrase when you create your SSH key. It is still secure enough. Or somehow store the password in your keychain, which is more difficult to setup and depends on your operating system. --> I did indeed. I'll see if I can change to an empty one. Thank you.
- 
- 

## Feedback
Please write down one thing that went well and one thing that can be improved.

### 👍 Tops
- Obtained a much better understanding of Git version control and standard software development workflow
- I was not aware of the best practices, I have been coding in a certain way for 10 years without knowing this!
- Material is very clear and nicely organised. Instuctors are also knowledgeable and friendly!
- Hosts join the break out rooms quite fast, and if they don't know the answer, they tell you instead of making stuff up, that's highly appreciated
- Very helpful and knowledgable instructors
- I liked the elaborate explanations and content-wise: the structure of using main/develop/feature branches.
- Some of coding style rules were new to me, useful to learn more about.
- Very clear instructions. Extra info were needed, but also easy to just skim through right to the tasks and ignore the parts that are not necessary depending on one's level.
- Really great that 'go at your own pace, don't worry if you're behind' is emphasised. x2
- Amazing to have all these "basic" things better understood, refreshed and out of the way, I just am afraid of forgetting these helpful things. x2
- Amazing learning environment for coding alongside with! And of course great support from the instructors. Smaller break-out rooms fit the type of assignments.
- Clear step-by-step instructions that work well with the additional support from the instructors. The break-out rooms work well.
- very useful to learn more background knowledge on this stuff (Git, environments etc) and learn about state-of-the-art conventions 
- I think the topics of the whole section are very well organized, it's easy to follow the texts
- Nice course material and also great to start with a general overview on how to structure and organize programming projects.-Something I really wanted to improve.
- Great way to start the course by getting everyone on the same page and getting used to the format

### 👎 Tips
- I don't know if there is a compendium or overview of common setup problems or hiccups that attendees often run in to, but having such issues and potential fixes neatly in one place would be very useful.
- 
- No incentive to work together with the people in the same break-rooms x2.5
- 
- 
- Perhaps not needed but a bit of more detail on how the inflammation repo is structured would help navigating the tasks.
- 
- Bit silly, but; the link to  ‘Putting comments in code: the good, the bad, and the ugly’ blogpost is broken
- Perhaps replace the section about PyLint with a section about ruff in the future? x2
- Curious how I would set up pyCharm for automatic Sphinx-format docstring generation. Perhaps include a short bonus section on this or a link?
- Why is use of wsl not recommended? Perhaps for people who already set it up for PyCharm it is still useful?
- (Not necessarily a tip, but more of a question): Is/Will there be a pdf-version of the content of this first session will all the subsections? I was looking up some of the command line statements by navigating back, then I copied them. But on the long run, I would love to have all in one file, so I could just quickly look it up. Also not sure if the web-page(s) remain online accessible (and unchanged)?!

### Sven's summary:
- We take notes of the problems we encounter and add them to the material. See [Common Issues, Fixes & Tips](https://carpentries-incubator.github.io/python-intermediate-development/common-issues/index.html) 
Unfortunately, these problems are always different so it's an ongoing endeavor to keep the material up-to-date.
- Actually working together in breakout rooms will start in section 4. But you are encouraged to ask each other for help, complain about this new thing you learned about that is absolute bullshit. We will have a little exercise today to encourage this a bit.
- ruff instead of pylint
- We will fix broken links, thanks for lettig us know!
- PyCharm auto docstring: https://medium.com/@djnrrd/automatic-documentation-with-pycharm-70d37927df57.
- WSL is not recommended, because it is more difficult to setup and configure. If you are used to it, feel free to use it though!
- The webpage remains online, we will send you an email after the course with all information. There is no PDF-version of all the codeblocks, perhaps you could adapt our [exercises extractor](https://github.com/esciencecenter-digital-skills/carpentries-exercises-extractor) to extract the code blocks instead of exercises.

## 📚 Resources

- [NLeSC Python template](https://github.com/NLeSC/python-template) - Start a package from scratch according to the current best practices