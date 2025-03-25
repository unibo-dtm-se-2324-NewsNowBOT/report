---
title: Home
layout: home
has_children: false
nav_order: 1
---

# NewsNowBot
 
## Authors
- **Paramjit Kaur** - paramjit.kaur@studio.unibo.it
- **Alessandro Zecchini** – alessandro.zecchini4@studio.unibo.it
- **Alice Sturaro** – alice.sturaro@studio.unibo.it
 
## Abstract
**NewsNowBot** is a web-based news aggregation and interaction platform designed to provide users with up-to-date news from multiple sources while enabling engagement through comments and ratings. The system leverages Firebase Authentication for secure user management and Cloud Firestore for real-time data synchronization.
The platform retrieves news articles from RSS feeds, categorizes them, and presents them in an accessible interface. Users can register, log in, and interact with the news by posting comments and ratings. Administrators have access to moderation tools for managing users, comments, and feed sources.
 
## Client-Side
The client-side of **NewsNowBot** is built using HTML, CSS, and JavaScript, ensuring a responsive and interactive user experience. Users can:
- Register and log in via Firebase Authentication.
- View news articles aggregated from RSS feeds.
- Post, edit, and delete comments on news articles.
- Rate news content and interact with other users.
- Navigate through an intuitive interface with categorized news sections.
 
## Server-Side
As a serverless application, **NewsNowBot** relies on Firebase services for backend functionality:
- **Authentication**: Firebase Authentication manages user registration, login, and session handling.
- **Database Management**: Cloud Firestore stores user data, news articles, and comments, ensuring real-time updates and scalability.
- **News Aggregation**: RSS feed sources are stored in Firestore, and the client retrieves and displays news dynamically.
- **Access Control & Moderation**: Admin users have the ability to manage users, comments, and RSS feed configurations through a dedicated admin panel.
 
## Key Features
**NewsNowBot** stands out by integrating a community-driven approach to news consumption, bridging the gap between passive reading and active discussion. Unlike many competitors that require subscriptions for premium features, **NewsNowBot** is designed as a free and accessible alternative with potential for future monetization through advertising or premium services.
 
## Future Developments
The project follows Domain-Driven Design (DDD) principles, ensuring modularity and scalability. Planned improvements include:
- AI-based comment moderation to filter spam and inappropriate content.
- Personalized news feeds based on user preferences.
- Mobile application development to enhance accessibility.
- Improved caching and performance optimization to handle large-scale user interactions.
