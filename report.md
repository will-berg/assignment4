# Report for assignment 4

## Project

Name: opsdroid

URL: https://github.com/opsdroid/opsdroid

An open source chatbot framework written in Python.

## Onboarding experience

Did you choose a new project or continue on the previous one?
> We started a new one since our last project was too small for this assignment.

If you changed the project, how did your experience differ from before?
> This project was a lot harder to start with since it didn't install properly. Some hidden requirements files and a lot of reading documentations later we managed to get it to work on most of our computers. Since the project also was bigger than our previous one, the code was more complex and therefore harder to understand. There was no one command that installed all dependencies, instead we needed to specify multiple modules (there was a module called "all" but this did confusingly not actually include everything).

## Effort spent

For each team member, how much time was spent in
> This assignment, more than previous assignments, we have all sat together and worked as a group than individually. Therefore the time is mostly the same for everyone in the group and we have choosen to write the same for everyone.

1. plenary discussions/meetings;
> We have each spent around 4 hours each in meetings of just planning, writing to each other in slack and getting our schedule to work with all the group members. Most of this time has been discussing if the issues we found where suitable for the project.

2. discussions within parts of the group;
> Some smaller things has been done in smaller groups, ~2 hours each, but most of the things has been done together in the full group.

3. reading documentation;
> Each person has spent around 4 hours searching individually for issues before the first 2 meetings in order to choose a repo and issue, and with that came a lot of documentation reading. We have also spent around 2 hours together in smaller groups reading more documentation.

4. configuration and setup;
> For the people with linux computer, this took around 1 hour since the code wasn't documented correctly. For the people with other operating systems, this was around 2 hours until some got it to work and others gave up and only pair programmed instead. This was one of the few things we wanted to do individually, but it would have been much better if we all sat together since we met the same problems.

5. analyzing code/output;
> Approximately 1-3 hours per person.

6. writing documentation;
> Approzimately 1 hour per person.

7. writing code;
> Approximately 4-5 hours per person. Some persons spent more time writing code while others spent more time writing the report.

8. running code?
> Approximately 1 hour per person.

9. Writing report;
> Approximately 1 hour per person in a meeting where we discussed this, then the persons that didn't write so much code spent more time writing the report.

## Overview of issue(s) and work done.

Title: Add get_skill method to opsdroid #1803

URL: https://github.com/opsdroid/opsdroid/issues/1803

Summary: Skills are python modules that are used to add functionality to the chatbot. The issue requests a method to return a skill given its method name, method name + class, method name + class + config file, or full path to the skill.

Scope: Two files were directly affected by our patch: `opsdroid/core.py` and `tests/test_core.py`. In the `core.py` file we added the requested method and some additional helper methods. We then added a test for our method in the `test_core.py` file that makes some simple assertions. Since the `get_skill` method is completely new it is not yet called somewhere else, so the scope did not expand beyond this.

Title for second issue: Replace our use of deadlinks with sphinx linkcheck

URL: https://github.com/opsdroid/opsdroid/issues/1696

Summary: We scanned for broken links with sphinx and fixed them.

Scope: Changed around 12 document files which had broken links.

## Code changes

### Patch

> The patch for #1803 is implemented on the [issue1803 branch](https://github.com/will-berg/assignment4/tree/1/report).
> The patch for #1696 is implemented on the [broken-links branch](https://github.com/will-berg/assignment4/tree/broken-links).

## Test results

> All the implemented tests passed for #1803, there were no tests to add to #1696.

## UML class diagram and its description
> Link to the UML diagram can be found [here](https://user-images.githubusercontent.com/47883315/222398651-e64e059b-6f5d-4f67-ad5c-6b37668a6548.png)


## Overall experience

What are your main take-aways from this project? What did you learn?
> It takes a long time to learn a project, and it took way longer to find a suitable issue than we thought it was going to take. We are thankful for the people who spends their spare time working on open source projects!

How did you grow as a team, using the Essence standard to evaluate yourself?
> Link to [essence document](https://docs.google.com/document/d/1hTcTf2wXyHpmJLGaf7FLB6UrkHsdOUrMGbju76j2pfE/edit?usp=sharing)
> We find ourself almost in the "performing" category, the only thing missing is one thing from the "Formed" category, "All team members understand how to perform their work.". This is mostly because all of us in the team were confused over this assignment. Both from that we weren't sure what the TA's would think of our work, and that open source project takes a long time to get used to (and many aren't writing issues in a good manner).
