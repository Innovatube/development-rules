# Code Review Principle

The main goal of appling code review to every project is to ensure the quality of source code and quality of final product/service 
by sharing knowledge beetwean the senior and junior developer and beetwean the development team in the whole company.

You can refer to this [document](https://docs.google.com/presentation/d/1MxtqdUUcWgQvuBufwfXdQiV5cwuJmDWce73qWLNAWMY/edit#slide=id.p3) to understand more about code review activity at `INNOVATUBE`.

## Code Review Plan

To ensure the code quality and product quality of all project, at the early stage of each project or in the kick-off time of project, 
PC need to confirm with client and development team how to process the code review in the project. 
We will define some typical code review models on the next section, then each project can choose the relevant code review model to apply to the project's process.

> If the defined code review models are not relevant to the project, 
> team member can tailoring the code review model for more relevant with the project and team members.

After selecting the relevant code review model, development team should put the code review decision into the README.md file of the project's repository for everyone can understand which code review model project are using.

And consequently, code review activities should be included into the madatory task for all project 
to ensure the quality of source code and eventually to ensure the quality of the final product/service that we provide to our client.
So, all the task related to code review also need to put into the backlog when doing the sprint planning 
and/or we need to add the code review into the `definition of done` for each coding task.

## Code Review models

### Github pull request model

This code review model is suiable for the project that have more than one developer working on the same project; then developers can perform peer-review for each others via gihub pull request system.
Or for the project that we can assign an senior developer to perform code review for every pull request of each commit from development team.

Basically, we will follow the pull request workflow of github. You can refer to detail information on this [link](https://help.github.com/articles/about-pull-requests/)

> In some emergency case, we can have an exception. 
> For instance, if the senior cannot spend time to approve the PR but client want to see some feature 
> then we can ignore the PR system and go ahead to deliver the feature that client needs.

### One shot code review system

This code review model is suiable for the project that have only one developer and we cannot assign a senior developer to do the fully code reivew for every commit.
In this model, we can perform some action to ensure the quality of the project

1. Get consultant/advise from senior to find the good boilerplate to start the project.
2. Apply the `pair-programming` with other senior at the begginning of the project to make a good code base.
3. Perform one shot code review activity by external developer every week. 
All the commemt code will be log into the github issue and including in the next sprint backlog.
    - Team code review within the team (team-ios, team-android, team-frontend, team-backend,...)
    - Assign one senior to review again the whole source code once every week.


Happy coding and grow together! ^^