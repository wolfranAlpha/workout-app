# workout-app
A workout application exercise.

## Goals

This is a fullstack development exercise built to test a potential candadite for a FS developer position.
The exercise is built as an application with a frontend and backend, and utilizing development best-practices.

For each candidate the exercise might look a little bit different - discuss with your supervisor the scope of this exercise and their expectations.

### Time-Frame

* Between one week and two weeks
  * One - Only FE or BE
  * Two - Both

### Communication

* I'm available for communication via watsapp during the evenings, and in office-hours.

## The Exercise

You will be creating an application (FE + BE) for managing workouts built by users.You may take exercuses from 

The exercise is split into two parts: https://exrx.net/ . You don't need a lot of data, just make sure that it is varied.

* design
* implementation

## Design

There are a lot of requirements - read the SRD and make sure that you understand all of the requirements.

Create a design document in your pprefered format. It should help your reviewer understand your intentions for implementing the application. Make sure to include a description of your API, the backend architecture, and anything else that you feel would help someone understand your implementation.

As part of your design, make sure to include a mock of the FE - created in whatever interface you prefer - such that we can understand how a user will interract with the flows in your application.

Make sure that your design allows you to implement all of the requirements **eventually**.

You should spend **roughly one day** on your design document. Send it to your reviewer when you are done.

## Implementaion - SRD

### Required Technologies

* BE - python 3 (preferably using fastapi or django)
* FE - react or angular
* DB - You may choose an SL or noSQL database
* DevOps - use Docker and github/gitlab workflows to streamline testing and deployment.

### Basic

* The user should be able to create a workout session. A workout session contains:
  * name
  * exercises in the workout - chosen from a preset list. An exercise contains
    * exercise name
    * muscle group
    * required equipment
  * the number of repettitions of each exercise
 * The user can start a workout. This includes
   * choosing the workout
   * trackng the time spent in the workout.
   * displaying the current exercise and allowing to mark an exercise as done
 * dockerize your frontend and backend using Docker and docker-compose
 * Handle invalid inputs sent by a user working with the API alone.

### Medium

* The user can search for an exercise or workout by muscle group worked.
* The option to pause a workout and take a break.
* Saving data to an external DB - existing workouts and exercises, workouts perfomed, time spent working out.

### Advanced

* Sign in - handle multipule users by allowing a user to sign in.
  * bonus: sign in using JWT
* Allow a user to mark a workout as shared such that any user can access it.
* Testing - write tests for your code that show that it functions as intended. Run them as part of the CI.
