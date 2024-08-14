# Feathers Node.js Developer Challenge: Rider Review System

## Objective

Extend our existing dispatch system by adding a rider review feature. This will allow customers to leave reviews for riders after a delivery is completed.

## Requirements

### 1. Create a new service called `rider-review` with the following features:
   - Create a review
   - Get all reviews for a specific rider
   - Get the average rating for a rider

### 2. The review schema should include:
   - id (auto-generated)
   - rider_id (references the dispatch user_id)
   - customer_id (the user leaving the review)
   - rating (1-5 stars)
   - comment (text)
   - created_at (timestamp)

### 3. Implement the following endpoints:
   - POST /rider-review (Create a new review)
   - GET /rider-review?rider_id=X (Get all reviews for a specific rider)
   - GET /rider-review/average?rider_id=X (Get the average rating for a rider)

### 4. Security requirements:
   - Only authenticated users can create reviews
   - Users can only create one review per rider
   - Riders cannot review themselves
   - Only the user who created a review can modify or delete it
   - Super admins can view all reviews

### 5. Integrate the new rider-review service with the existing dispatch service:
   - Add a virtual field `average_rating` to the dispatch service that fetches the rider's average rating

### 6. use the latest version of feathersjs , mongodb or postgres is fine


## Evaluation Criteria:
1. Code organization and clarity
2. Proper use of Feathers.js service structure
3. Correct implementation of authentication and authorization
4. Proper error handling and input validation
5. Ability to integrate the new service with the existing dispatch service
6. Basic understanding of database operations and queries
7. Proper use of Git (commit messages, branching)
8. api documentation
9. hosting of project


## Submission Instructions:
1. Fork this project repository
2. Create a new branch for the rider-review feature
3. Implement the required features
4. Write clear documentation for the new endpoints in the README
5. Create a pull request with your changes

## Time Limit: 
You have 2 days to complete this challenge. Please let us know if you need any clarifications or have any questions.

## Existing Project Structure

[Include a brief overview of your current project structure here, highlighting key services and files that the candidate should be aware of]



Good luck! We're excited to see your implementation.
