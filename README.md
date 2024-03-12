# REST-API-for-workout-plan-system
RESTful API for a Personalized Workout Plan system that allows users to create and manage customized workout plans and track their fitness goals

# Features
- **User Authentication**: Secure user registration, login, and logout functionality using JWT.
- **Exercise Management**: CRUD operations for managing exercises with details like name, description, and target muscles.
- **Workout Plans**: Create, update, and delete workout plans specifying exercises, sets, repetitions, etc.
- **Exercise-Plan Association**: Select exercises, create an exercise plan and associate it with workout plans to create personalized workout routines.
- **Tracking Goals**: Set and track fitness goals, set weight goal and track weight.
- **API Documentation**: Interactive API documentation powered by Swagger UI.

## Installation and Setup
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

## API Endpoints

### User Authentication:
- Register a new user: `POST /register`
- Log in: `POST /login`
- Log out: `POST /logout`

### Exercises:
- Create a new exercise: `POST /exercises`
- Retrieve all exercises: `GET /exercises`
- Retrieve a specific exercise: `GET /exercises/<exercise_id>`
- Delete an exercise: `DELETE /exercises/<exercise_id>`

### Workout Plans:
- Create a new workout plan: `POST /plans`
- Retrieve all workout plans: `GET /plans`
- Retrieve a specific workout plan: `GET /plans/<plan_id>`
- Update a workout plan: `PUT /plans/<plan_id>`
- Delete a workout plan: `DELETE /plans/<plan_id>`

### Exercise-Plans:
- Select an exercise and create its plan: `POST /exercise_plans/<int:exercise_id>`
- Change an exercise plan: `PUT /exercise_plans/<int:exercise_id>`
- Delete an exercise plan: `DELETE /exercise_plans/<int:exercise_id>`
- Retrieve an exercise plan: `GET /exercise_plans`
- Retrieve an exercise plans: `GET /exercise_plans/<int:exercise_id>`

### Tracking Goals:
- Set fitness goals: `POST /tracking_goal`
- Delete fitness goals: `DELETE /tracking_goals/<tracking_goals_id>`
- Change fitness goals: `PUT /tracking_goals/<tracking_goals_id>`
- Track progress towards goals: `GET /tracking_goal`
- Track progress towards goal: `GET /tracking_goals/<tracking_goals_id>`
  
### API Documentation:
 - Explore the API using Swagger UI: [Swagger UI](https://your-api-documentation-url.com)
