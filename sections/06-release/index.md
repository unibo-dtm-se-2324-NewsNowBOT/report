---
title: Release
has_children: false
nav_order: 7
---

# Release

## 6. RELEASE
 
The **NewsNowBot** web application release includes the entire frontend and backend services, ensuring all components are publicly accessible. It is published on GitHub as the central repository for code and versioning, while deployment to Firebase Hosting makes the application accessible globally through a live web interface.
The release process is automated through **GitHub Actions**, which triggers the deployment pipeline whenever new changes are pushed to the repository. Given the nature of Firebase Hosting, the system does not follow strict semantic versioning (SemVer) but ensures clear tracking of updates and deployments.
Versioning and Releases

Versions were defined retroactively using annotated tags (git tag -a) and associated with significant commits in the project's history. Below are the main milestones:
- **v0.1.0** – Basic Initialization and StructureInitial project structure: static HTML, first stylesheets and basic scripts. Setup of registration/login page and initial Firebase configuration.
- **v0.2.0** – Admin Backend and User ManagementImplementation of administrative functionalities for user and comment management. Introduction of admin panel and dynamic content management.
- **v0.3.0** – RSS Feed and Dynamic ContentAddition of RSS feed collection and display functionalities, both on user and admin side. Implemented JS scripts for dynamic loading from database.
- **v0.4.0** – Homepage, Team, and ImagesCreation of homepage, "Our Team" section and integration of representative images. Layout refinement with addition of graphic elements and textual content.
- **v0.5.0** – User/Admin Interface RefinementsEnhancement of user interface and admin page, CSS updates and HTML structure for improved visual experience.
- **v0.6.0** – Cleanup and Textual ImprovementsRemoval of unnecessary code comments, page text updates and general improvements to code readability.
- **v0.7.0** – Documentation and NormalizationAddition of README.md and Disclaimer.md files, update of .gitignore, removal of unwanted files like .DS_Store, and introduction of normalize.css for cross-browser consistency.
Thanks to this versioning scheme, it was possible to precisely track the functional and technical evolution of the project, facilitating debugging, collaboration, and future software extensibility.
 
**NewsNowBot** is distributed under the **MIT License**, a permissive open-source license allowing users to freely use, modify, and distribute the software with proper attribution. This choice aligns with the project's educational objectives, fostering collaboration and encouraging contributions from the open-source community.
