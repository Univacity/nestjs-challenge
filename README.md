# Task: NestJS Application for Program Search

## Description:
As part of our evaluation process for potential collaboration with Univacity, we invite you to showcase your expertise in developing a NestJS application that enables users to search for educational programs offered by various institutes. This task will assess your skills in creating a robust search functionality based on different criteria.

## Task Details:

### Backend (NestJS with Mongoose):
Develop a RESTful API using NestJS and Mongoose that allows users to search for educational programs. The application should have the following components:

**Program Management**: Implement API endpoints for adding, retrieving, updating, and deleting program details.

**MongoDB Integration:** Use Mongoose to model and interact with a MongoDB database to store program information.

**Search Functionality:** Implement a comprehensive search functionality that enables users to search programs based on different criteria such as program level, institute, country, and text search on program name and description.

**Error Handling:** Implement appropriate error handling mechanisms to ensure a smooth user experience.

## Requirements:

Develop the backend application using NestJS and integrate it with MongoDB using Mongoose.
Define API routes and controllers for managing program information.
Implement Mongoose models and schemas for structuring and storing program data in MongoDB.
Design a robust search mechanism that accommodates various search criteria.
Implement data validation and error handling for various scenarios.
Organize the project's codebase following best practices and maintainable structure.
Host your project on a version control platform such as GitHub.
Provide a README with instructions for setting up and running the application locally.

### Sample Interface:

```typescript

// Program Interface
interface Program {
  _id: string;
  name: string;
  level: 'undergraduate' | 'masters' | 'phd';
  institute: string;
  country: string; // 2 characters long eg 'NG' | 'US'
  description: string;
}

// Program Search Criteria
interface ProgramSearchCriteria {
  level?: 'undergraduate' | 'masters' | 'phd';
  institute?: string;
  country?: string;
  searchText?: string;
}

// Program DTO (Data Transfer Object)
class CreateProgramDto {
  name: string;
  level: 'undergraduate' | 'masters' | 'phd';
  institute: string;
  country: string;
  description: string;
}
```
## Submission:
Share the link to your GitHub repository containing the project. If you have any questions or need clarification, feel free to reach out to us.

This task aims to evaluate your ability to develop a NestJS application that includes a robust program search functionality, which aligns with the core features of our platform at Univacity. We're looking forward to seeing your implementation and assessing your skills!




