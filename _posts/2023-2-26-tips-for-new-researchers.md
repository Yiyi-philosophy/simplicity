---
title: 'Tips for Success as a New Researcher'
tags: Mmethodology 
---
This guide is a compilation of tips I wish I knew when I was starting out doing computer science research as an undergraduate student at Stanford.

<!--more-->

> Reprinted from [https://www.alextamkin.com/essays/tips-for-new-researchers](https://www.alextamkin.com/essays/tips-for-new-researchers) by [Alex Tamkin](https://www.alextamkin.com/home)



This guide is a compilation of tips I wish I knew when I was starting out doing computer science research as an undergraduate student at Stanford.

It's targeted towards high school / undergraduate / Master's students working with a research mentor (e.g. a postdoc / PhD student), but might be helpful for junior PhD students or new industry researchers as well.

# Problem Solving Skills

## Perseverance

* Research will be hard at times!
* It's very different from the classroom model of success, where there are concrete learning goals and you can aim for the 'A' at the end.
* You're not going to understand stuff at first: it will feel overwhelming, the path won't be clear, and you'll question why what you're doing even matters
* You will have to keep on pushing through—effort, grit, and resilience are key ingredients for developing as a researcher
* Focus on your growth: gradually you'll understand more and more and be able to see farther and deeper into the research world around you

Asking for help

* This is one of the most important skills in research, and part of persevering!
* Asking for help shouldn't be viewed as a bad thing or "giving up"—it's a natural part of the learning process and will help you make progress
* For example, it's typically not productive to doom-scroll Stack Overflow for 10 hours if you're really stuck
  * Instead, you might send your mentor a message with a brief summary of the issue / question (or the full stack trace of an error) so they know you're stuck and can help you. You can also briefly share some different strategies you've tried.
  * Often it may be something they've experienced too, and can resolve for you quickly!
* Unsure whether you should reach out to your mentor? Ask them how long you should try to solve something on your own before reaching out for help
  * For some mentors this might be 20 minutes, for others this might be a day or more. Ask them to help you calibrate.
  * I personally tell my mentees to err on the side of pinging me too often at first (I'd rather spend a few seconds to unblock you, than learn you've been stuck for a week and unable to make progress)
* If something is taking you a long time, and you think there might be a better way—ask! There might not be, but it never hurts to ask!
  * Example 1: a student I worked with found using [tmux](https://www.google.com/url?q=https%3A%2F%2Fwww.hamvocke.com%2Fblog%2Fa-quick-and-easy-guide-to-tmux%2F&sa=D&sntz=1&usg=AOvVaw12SyrbUQXlBTA3zl8sNn9W) to be very slow. They asked for help and found out about mouse support!
  * Example 2: another student I worked with was waiting a long time for bash commands to finish before they could launch another one. They asked if there was a better way and learned about bash scripts and background processes!
* Another place to ask is in Slack (or whatever platform you use)—some workspaces have a #debug channel or similar where you can ask questions about bugs, libraries, the cluster, best practices, etc

## Resourcefulness

* Of course, your mentor won't always be there to answer your questions
* It's important to learn how to problem-solve for yourself. Some simple techniques:
  * If you run into a bug, Google the top-level error in your stack trace
  * Search up solutions on Slack, GitHub, Linux man pages, Stack Overflow, documentation, etc
  * If you don't know what a function or feature does, open an interactive Python session or make a mini jupyter notebook or script to try it out!
* Problem solving is a skill you get better at—observe your collaborators and mentors. Notice how they solve issues you aren't able to solve, or ask them!
* You can sometimes ask to observe other people while they work to pick up strategies
  * You can also do the reverse and have them watch and give you feedback
  * Pair programming is really great for gaining insights large and small about people's processes!

## Velocity

* Velocity just means how quickly you're able to iterate on tasks and experiments
* This is crucial for making progress on a week-to-week basis, since it enables you to test out hypotheses and obtain results
* It's very common to feel "slow" when you start doing research (or even for years after!), especially when comparing yourself to others. This is normal—don't sweat it. Your velocity will increase as you do more research
* One useful goal is to have some deliverable, however small, for each meeting
* Often times, velocity improves over time just due to familiarity with your tools, for example:
  * Reusing a codebase or library for a new project saves so much time compared with having to write it from scratch yourself
  * Once you know the bash command to do something (e.g., list the largest folders in your directory), you won't have to look it up again each time (or at the very least you'll know how to find the answer quickly)
  * There's only a finite number of common errors or bugs in any problem domain: once you figure out how to solve something the first time, you can solve it a lot more quickly the next time. (I remember it always seemed like magic to me when my mentors knew the fixes for all the bugs I ran into, but it was just this at play!)
  * See also: [Learning Curves ](https://www.google.com/url?q=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FLearning_curve&sa=D&sntz=1&usg=AOvVaw1hQfGVvkvU9YHTgtkP3j3b)[(](https://www.google.com/url?q=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FLearning_curve&sa=D&sntz=1&usg=AOvVaw1hQfGVvkvU9YHTgtkP3j3b)[Wikipedia)](https://www.google.com/url?q=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FLearning_curve&sa=D&sntz=1&usg=AOvVaw1hQfGVvkvU9YHTgtkP3j3b)
* You can also pay attention to your work habits and identify ways you can improve your velocity. Your mentor can help you identify strategies here! For example:
  * Queueing up jobs with a bash script or Slurm as opposed to running them manually
  * Searching your bash history for previous commands you've run instead of wandering through StackOverflow results you’ve already browsed before
  * Tracking experiments using a tool like [Weights and Biases](https://www.google.com/url?q=https%3A%2F%2Fwandb.ai%2Fsite&sa=D&sntz=1&usg=AOvVaw1g71yAtYbU2m3LgH17n5rA) or [Neptune](https://www.google.com/url?q=https%3A%2F%2Fneptune.ai%2F&sa=D&sntz=1&usg=AOvVaw3J6r0FjrA1CWyWnNnGpu89) instead of by hand or by copy-pasting results into spreadsheets
  * Learning how to search / organize your files effectively, vs navigating through tons of folders
* It can sometimes be hard for your mentor to know if slow velocity is due to lack of available time or if you're finding it challenging to complete your tasks.
  * Letting them know approximately how long you're spending on each task and which parts you're finding challenging can be a really effective way to help them help you
* Keep in mind that your energy is just as important as your time. If a tool feels like it's introducing a lot of friction (or you start to dread using it), often that can be an indicator that it's time to learn how to use it better or possibly find an alternative.

# Meetings / Communication

## Use meetings to zoom out

* When you've spent all week on a project, mentor meetings are a really good opportunity to take a step back and think about your project from a high-level perspective
  * This is useful for making sure you're directing all of your effort in a productive way—research is about working smarter not just harder
  * It also gives you practice in developing your "researcher brain:" How do your tasks fit into the project as a whole? How does your project fit into your broader field? (How does your field fit into the broader space of science / humanities / the arts / the world?)
* Another important reason to zoom out is that your mentor isn't steeped in the details of your project like you are, so they might need a bit of a refresher to see the connection between what you did last week and the broader goals of the project—and help you plan accordingly

## Invest time in data visualizations

* New researchers have a tendency to present their results verbally in meeting
  * e.g. saying statistics out loud: "Algorithm 1 got 34.4% and Algorithm 2 got 34.5%"
* It may take more time, but you'll get much much more out of the meetings with your mentor if you create a graph or table for you and your mentor to look at together
* This makes it much easier to analyze, ideate, and come up with next steps. Time making effective visualizations is time well spent!

## Communicate effectively over slack / email

* Even between meetings, it can be nice to ping your mentor / group slack channel with ideas, preliminary results, problems you're having, etc
* This is a good way to stay on your mentor's radar and help them support you
* What kinds of messages you send might depend on your personal style. Some ideas:
  * "I just ran the new baseline we talked about last meeting, here's a graph of the results compared to the simpler baseline. The performance looks slightly better but they're pretty similar"
  * "It looks like running the larger scale experiments might take a while—the cluster is really busy due to the upcoming deadline. My guess is it will take until Tuesday for our jobs to run. Do you think we should wait it out, or look into other compute options?"
  * "I talked to Alba about our project, and she passed along this paper: `<link>`. I added it to our related works doc with a few notes!"
  * "Not urgent, but I was wondering: why do we normalize our images before passing them through the network?"
  * "Hey, I've been curious to learn more about distributed training. Have any recommended papers / readings you like?"

## Take initiative and "manage up"

* Initially, your mentor will probably run your meetings by guiding the agenda and determining next steps
* But as you advance as a researcher (generally over a few months), you'll start to be able to determine some next steps by yourself, and save your mentor the effort of running the meeting by themselves (and coming up with each concrete next step / experiment / idea)
  * This is called taking initiative and "managing up"!
* One thing you can do at any stage is have an agenda for each meeting
  * Come to the meeting with questions you have + goals for what to accomplish during the meeting
* There are also other ways of showing initiative:
  * Writing a script to automate a common task
  * Trying to analyze/interpret the results of experiments, vs just running them
  * Reading and sharing a piece of related work with some notes about what it does and how it connects to the project

## "Levels of Research Autonomy" (how your independence might develop as a researcher)

* Level 1: New researchers often complete their task and just share the raw results (e.g. a graph or table)
  * Ex: "I ran what we talked about and here are the results!"
* Level 2: Slightly more experienced researchers might think about the results and give an interpretation
  * Ex:. "it's nice to see that the new algorithm improves performance, but the baseline is actually a lot higher than we were expecting"
  * Interpreting data may be hard at first, but will be more natural over time. Don't force it if no insights come to mind, but coming up with potential interpretations can be good practice.
* Level 3: Even more experienced researchers might further propose some next steps to talk about with their mentor
  * Ex: "I wonder if we should consider other tasks that better highlight the concept we're interested in. For example, I did some searching and found X, Y, and Z"
* Level 4: Another step beyond that might be taking the initiative to run additional studies or experiments beyond what was discussed
  * Ex: "I also ran our models on X, Y, and Z datasets and found that existing methods actually do quite poorly. Do you think it makes sense to run a larger scale study on these settings?"
  * This gets a lot easier as your velocity improves
* Level 5+: As you progress even further, you might be able to do this process at an even higher level of abstraction (first within the project and then across projects!)
  * Ex: "These last few experiments show property A of our system really well. I wonder if we could explore property B, maybe with experiments Q, R, or S?"
  * Ex: "Our last paper made point C really well. I'm wondering if we could push this even further by looking at setting D, using tools from field W?"
  * Ex: "One thing that's really unsatisfying about approaches in field Q is that they don't really get at property P. Do you think we might be able to operationalize this in some way? Here's a sketch of one possible approach."
* Note: your mentor won't always be right—sometimes they might suggest an idea that doesn’t work, or they might not have a great solution idea. This is normal, as research is exploratory, and you’re solving a new problem.

# Broader opportunities (in a lab setting)

## Go to events!

* Lab meetings: Can be a great way to get exposure to a research environment
* Talks / reading groups: Learn how research is conveyed + understood by your community
  * When you feel comfortable, try to present a paper in a reading group!
* Social events: get to know folks in the lab and become part of the community

## Reach out to grad students in the lab (and out of the lab)

* Read a bit about them + their papers on the website
* Reach out and mention something you found interesting, and that you'd love to chat more
* DMs on slack often work well in my experience

# Personal

*Note: It's the mentor's responsibility to create an environment where these personal values are the norm—and they should be strong models of these as well!*

## Confidence / intellectual humility

* Don't feel like you have to pretend you know everything coming in—your mentors know that you're learning (they are too!).
* Saying "I'm not sure I understand, can you explain that a bit more?" is one of the fastest ways to grow and learn—and you should be saying it a lot, especially at the start of the project!
* Also remember that you have knowledge and background that others don't—and the reverse will also be true. Embrace that and learn from (and share with!) your collaborators

## Honesty / Integrity

* Trust isn't something that's easy to regain on either side
* Stay true to your word, and communicate openly with your mentors—they should do the same for you
* If you're not going to be able to make a deadline or finish a task by the date you'd said, let them know as soon as possible so they can re-coordinate the rest of the team (or just their own expectations)
* If you discover a bug which affects your previous results—let the team know. Their response should ideally be constructive, e.g. "Well this is a bummer, but I'm really glad you caught this! Let's think about how to proceed, and how we can prevent something like this in the future…"
* You should expect the same honesty / integrity from your mentors and the other people you work with

## Identity, boundaries and health

* It should go without saying, but your mentors should create a space where you feel comfortable being yourself, and where you feel respected and supported in your identity so you can do your best work
* Every lab has a different work culture, but no research project should push out everything else in your life or imperil your physical or emotional health
* Having time for friends + family / rest / leisure is really important, and if you're feeling pressured to not have it, that's a problem

## Energy

* Being excited about the work and research is a great thing!This makes your collaborators feel good too.
* Don't force it, especially if you're feeling confused or frustrated (all natural parts of the research process), but feel free to express authentic excitement when you feel it
* Energy is infectious and can really make a big difference in a work environment

## **Acknowledgments**

Thanks to Shreya Shankar, Jesse Michel, and Daniel Fein for providing helpful feedback on an earlier draft of this, and Nick Tomlin for useful conversations!
