---
title: Requirements
has_children: false
nav_order: 3
---
# REQUIREMENTS

## Goal

The goal of **NewsNowBOT** is to provide an easy-to-use website where users can to be constantly updated on the latest news from major newspapers allowing them to comment and vote on news.

## Functional Requirements

**1\. Authentication**

**Requirement:** Users must be able to create a profile and log in to the application.

**Acceptance Criteria:**

-   Users can create an account using an email, password and specifying their role (basic user or admin).
-   After creating an account, users can log in using their email and password.
-   On successful login, users are redirected to their homepage with different functionalities based on their role.

**2\. Deletion or modification of a user**

**Requirement:** Admin must be able to see the list of users and modify their fields or delete them from the database.

**Acceptance Criteria:**

-   In the admin homepage is shown a table with the list of users present in the database with their characteristics, and two buttons: "Edit" and "Delete"
-   If the admin clicks modify, a sequence of forms show the characteristics of the individual user allowing the modification
-   Otherwise by clicking delete, the user is deleted from the database.
-   Finally, the table updates automatically, showing the changes made.

**3\. Elimination of a newspaper**

**Requirement:** Admin must be able to see the list of newspaper and delete them from the database.

**Acceptance Criteria:**

-   In the admin homepage is shown a table with the list of newspaper present in the database, and a button: "Delete"
-   If the admin clicks delete, the newspaper is deleted from the database.
-   Finally, the table updates automatically, showing the changes made.

**4\. Add new newspaper**

**Requirement:** Admin must be able to add a newspaper into the database.

**Acceptance Criteria:**

-   In the admin pages there is a form to add new newspapers.
-   The admin must be able write the name of the newspaper and the URL of the RSS.
-   Finally, the newspaper table updates automatically, showing the changes made.

**5\. Delete comments and ratings**

**Requirement:** the admin must be able to display a table with the list of comments and ratings related to the news expressed by users.

**Acceptance Criteria:**

-   In the admin homepage is shown a table with the list of comments and ratings present in the database, and a button: "Delete"
-   If the admin clicks delete, the comment and rating is deleted from the database.
-   Finally, the table updates automatically, showing the changes made.

**6\. See the news**

**Requirement:** Users must be able to see the list of news and click on them to read the article

**Acceptance Criteria:**

-   In the user homepage is shown a list of news constantly updated from the newspapers included in the database.
-   If the user clicks on a news item, he should be redirected to the article page

**7\. Add comments and ratings**

**Requirement:** the user must be able to comment and rating a news.

**Acceptance Criteria:**

-   In the user homepage is shown a form where the user can choose a news, add a comment a mark from 1 to 5.
-   By clicking on "comment" the vote and the comment are saved in the database.

## Non-Functional Requirements

**1. Security**

**Requirement:** User data and access must be protected.

**Acceptance Criteria:**

-   Firebase Authentication ensures secure login and password management.
-   Firestore security rules define access permissions for users and admins.
-   HTTPS is enforced to encrypt data transmission.

**2. Performance**

**Requirement:** The application must be responsive and handle concurrent users efficiently.

**Acceptance Criteria:**

-   News retrieval and user interactions occur in real-time without noticeable delays.
-   Queries to Firestore are optimized for performance and scalability.

**3. Availability**

**Requirement:** The system must be available 24/7 with minimal downtime.

**Acceptance Criteria:**

-   Firebase Hosting ensures uptime and global accessibility.
-   Regular backups prevent data loss in case of failure.

## Implementation Requirements

**1. Programming Language & Frameworks**

**Requirement:**\
The application must utilize modern frameworks that support both mobile and desktop environments.

**Acceptance Criteria:**

-   The front-end is implemented using **HTML, CSS, and JavaScript**, ensuring flexibility and responsiveness.
-   User authentication and backend services are managed using **Google Firebase**, providing a scalable and secure solution.

**2. Database Management**

**Requirement:**\
User data and authentication records must be stored in a structured database system to ensure efficient management and security.

**Acceptance Criteria:**

-   **Cloud Firestore** is used as the database, allowing **seamless storage and retrieval** of user profiles and other relevant data.
-   The data structure is **optimized for scalability and performance**, ensuring efficient synchronization and access control.
