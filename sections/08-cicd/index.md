---
title: CI/CD
has_children: false
nav_order: 9
---

# CI/CD
The **CI/CD pipeline** for **NewsNowBot** automates the process of testing and deploying the application, ensuring a smooth workflow and maintaining code quality throughout development. The pipeline is managed using **GitHub Actions**, which integrates directly with the project repository.
 
Whenever new code is pushed to the repository or a pull request is created, the **CI process** is triggered automatically. This involves running **unit tests on JavaScript code** and verifying **Firestore security rules**, ensuring that changes do not introduce regressions or break existing functionality.
 
Once tests pass successfully, the **CD process** takes over. The pipeline automatically deploys the latest version of **NewsNowBot** to **Firebase Hosting**, making the update immediately available to users. Since Firebase Hosting does not require traditional versioning, releases are tracked through **GitHub commits** rather than **Semantic Versioning (SemVer)**.
 
This automated workflow reduces manual intervention, accelerates the development process, and ensures that each deployment is **tested, secure, and consistently updated**, enhancing the reliability and stability of the **NewsNowBot** platform.
