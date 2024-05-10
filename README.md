
# FlickFix - Movie Booking Management System

Flickfix is the ultimate movie booking platform that transforms how you experience movies at your local theaters. It offers a seamless portal to explore and book the latest films at cinemas near you. Not just for movie-goers, Flickfix also provides a platform to theater owners to grow their business.

## Project Concept

Flickfix aims to redesign and enhance the movie theater ticket booking system, making it streamlined and user-friendly.

## Key Features

- Customer-Centric Interface
- Admin Control Dashboard
- Integrated Payment Gateway
- Real-time Booking
- User Interfaces for Multiple Roles

## Tech Stack

- **Backend**: Node.js & Express.js
- **Frontend**: React
- **Database**: MongoDB
- **Other Tools**: Visual Studio Code, Git

## Application Architecture Overview

### System Architecture

Flickfix implements a hybrid architecture combining elements of microservices and monolithic models, emphasizing a service-based framework:

- **Frontend Service(s)**: Built with React.js, focusing on reusable, modular UI components for a dynamic user experience.
- **Backend Service(s)**: Utilizes Node.js and Express.js for RESTful API interactions and modular business logic processing.
- **Database(s)**: MongoDB is chosen for its flexibility and scalability, fitting well with the JavaScript-based backend due to its document-based storage.

This structure allows leveraging the strengths of both architectural models to enhance scalability and maintain development efficiency.

### Application Structure

- **Client-Side**: Built with React.js, utilizing Ant Design for UI components and managing state with Redux and Redux Toolkit.
- **Server-Side**: Uses Express.js running on Node.js to handle API requests, connect with MongoDB, and manage server logic.
- **Database**: MongoDB for data storage with complex queries, schemas, and models designed to handle movie, theatre, and booking data.

## User Roles and Interfaces

- **General Users**: Interface for browsing movies and booking tickets.
- **Admin**: Interface to upload movies, manage theatre owners, and oversee application settings.
- **Theatre Owners**: Interface to add theatres and manage shows after receiving admin approval.

### Architecture Style

Flickfix adopts a hybrid architecture style in software design, blending elements from various architectural styles. This approach leverages the strengths of each style while mitigating their limitations.

- **Key Characteristics**:
  - Performance: Non-blocking I/O with React.js and Node.js ensures high throughput.
  - Scalability: Modular design and MongoDB’s horizontal scaling enhance the system’s ability.
  - Security: Robust security with layered authentication and authorization.
  - Responsiveness: React.js provides fluid and interactive user interfaces.
  - Fault Tolerance: Redundancy and failover mechanisms minimize downtime and maintain service continuity.

## Software Design Principles

- **Modularity**: 
  - Frontend: Reusable React.js components, utilizing Ant Design for UI consistency.
  - Backend: Express modules manage distinct functionalities like user authentication and data processing.
- **Separation of Concerns**: Clear functional division enhances code maintainability and readability.
- **Bounded Context**: Well-defined component responsibilities, ensuring efficient management of user roles and application features.
- **CI/CD Pipelines**: Automated building, testing, and deployment using Docker and GitHub workflows.
- **Iterative Development**: Agile development with regular sprints and stakeholder feedback for continuous improvement.

## Challenges Faced

1. Handling concurrent bookings where multiple users attempt to book the same seat simultaneously.
2. Ensuring secure logins and access control for users and administrators.
3. Integrating third-party payment gateways.

### Solutions

1. Used a locking mechanism.
2. Implemented JWT for secure authentication.
3. Utilized secure, well-documented APIs provided by payment gateways.

## Lessons Learned

- **Real-Time Data Handling**: Techniques for managing real-time data interactions.
- **Agile Methodology**: Importance of sprint planning, retrospectives, and testing for application development.
- **Security Practices**: Implementation of security measures, including JWTs and HTTPS.

## Improvements

1. **Refined User Interface**: Adding more interactive elements to enhance the booking experience.
2. **Microservices Approach**: For better scalability, easier maintenance, and faster deployment of new features.
