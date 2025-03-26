---
title: Development
has_children: false
nav_order: 5
---

# Development

## DVCS

The code was developed using Git, a Distributed Version Control System (DVCS), and managed through a shared GitHub repository, enabling seamless collaboration among team members.

This approach facilitated granular tracking of changes, with each developer modifying the code in Visual Studio Code (VSC) and synchronizing updates via Git.

***Branching Strategy***

In our project, we adopted a **single-branch workflow**, working exclusively on the main branch.

While many development teams use multiple branches for feature development and testing, we opted for this simpler approach for the following reasons:

-   **Project Scope and Complexity**: The project was relatively small and did not require extensive branching for different features or environments.
-   **Team Coordination**: With three developers working on the repository, we maintained direct communication to reduce conflicts and ensure smooth collaboration.
-   **Managing Merges**: Although we encountered some merge situations---including one with conflicts---we were able to resolve them efficiently through discussion and manual selection of the correct version. This highlighted the importance of keeping the repository up to date.
-   **Rapid Development Cycle**: By working directly on the main branch, we streamlined the workflow, allowing faster implementation of features and fixes without additional merge overhead.

While this approach was effective for our team size and project scope, we acknowledge that using multiple branches for development, testing, and new features would be beneficial in larger and more complex projects.

***Conventions for commits***

Commits followed a descriptive format to maintain a clear history of changes.\
Each commit included a concise message summarizing the modifications made or, at least, specifying the edited page.

Some examples are "Images and descriptions in homepage added ", "Modified user CSS part" or "Added the Rss feed collection to the database"

***Issues Encountered regarding merge***

During the development process, we encountered issues related to **merges **due to asynchronous commits and pushes.

A merge situation occurred in the following scenario:

-   A developer made changes, committed them locally, but did not push them immediately.
-   Meanwhile, other team members made their own changes, committed them, and successfully pushed them to the shared GitHub repository.
-   When the first developer eventually attempted to push their changes, Git detected that the remote repository had been updated since their last pull.

-   To resolve this, Git required the developer to first pull the latest changes before pushing their own, resulting in an automatic merge.

We encountered two different merge scenarios:

-   In the first case, the developers modified two different parts of the code, so the merge was automatically resolved by Git.\
    For example, one developer was working on the admin page while the other was editing the home page.
-   In the second case, two developers were working on the same file, specifically the admin page, and modified the same line of code.\
    Here, we discussed the changes among the team, decided which version to keep, and manually selected the correct one.

## IMPLEMENTATION DETAILS

***New and relevant learnings***

During the development of NewsNowBot, we have gained a number of significant lessons that have allowed us to improve as developers. We have explored the use of Firebase Authentication to manage user registration and login, learning how to apply advanced security practices to protect data. Managing data in Cloud Firestore taught us how to handle real-time databases, optimizing queries and ensuring synchronization between users. In addition, the serverless approach with Firebase allowed us to explore how to automatically scale infrastructure without the need to manage physical servers. Another important learning was the adoption of the Test-Driven Development (TDD) methodology, which helped us to write more robust and easily maintainable code, guaranteeing the quality of the final product.

***A class of which we are particularly proud***

*One of the most successful aspects of NewsNow is the CommentService class, designed to manage the sending, retrieval and moderation of comments efficiently and in real time.*

The main features of the class include instant comment updates *and role-based permission management, *allowing administrators to moderate or delete comments*.*

This class has significantly enhanced the interactivity of NewsNow*, improving the user experience and creating a dynamic and engaging environment for news discussion.*

## DEVELOPMENT DESCRIPTION

*NewsNow is a web-based news aggregator platform that allows users to stay up to date with articles from various sources and interact with the content through comments and votes.*

*The system uses Firebase Authentication for secure user management and Cloud Firestore for real-time data synchronization. Users can register, log in, comment, and vote on articles. Administrators have access to moderation tools to manage users, comments and RSS feeds. The front-end is built with HTML, CSS and JavaScript, offering a responsive and interactive interface.*

*The application is designed to be easily scalable, with features such as *RSS feed management, comment moderation, and user management, all supported in real-time through Cloud Firestore.

## ARCHITECTURE OVERVIEW

*NewsNow adopts a serverless client-server architecture, in which Firebase manages both the back-end and authentication and data management.*

*Firebase Authentication ensures secure access, while Cloud Firestore stores user data, comments and news, syncing them in real time. Data security is managed through Firebase Security Rules.
The system is based on three main entities: User, News and Comment, with business logic managed by domain services and data persistence through repositories.*

*The architecture is scalable and allows for instant updates.*

