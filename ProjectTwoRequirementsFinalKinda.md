# Word Bank

## Modules
### (Comment Module):
- Create Comment Object.
- Persist Comment Object.
- Display Comment Object
- Destroy Comment Object
### (Thread Module)
- Create Thread Object
- Persist Thread Object
- Display Thread Object
- Display Comments Within Thread Object
- Manage The Comments Within Existing Thread Object
- Manage User’s Currency Within Existing Thread Object
### (Community Module)
- Create Community Object
- Persist Community Object
- Display Community Object
- Manage Threads (Creation and Deletion)
### (Users Module)
- Creating User Object
- Persisting User Object
- Display User Object
- Manage User State

## Roles
__Cody Harkins__: Comment Module
__Baldemar Sepulveda__: Thread Module
__Thita Low__: Community Module
__John Paul__: Users Module

## Description
Word Bank is a full stack web forum similar to reddit that gamifies the act of communication with other people. A user can message to other users within a set of communities, except that each character they use in their messages is withdrew from their character bank within a thread. Each community will have threads. Users’ character bank are unique to each thread. A users’ character bank refills every time they are responded to. There is a max number of threads within a community. Any user will be able to create a thread as they wish but the oldest thread will be deleted as a result when exceeding the max number of threads.

## Purpose
Testing an interesting idea for a forum site that will allow users to experience a community that requires constant good communication.

## Requirements
1. Functionality must reflect user stories.
2. Messages will be stored within a database.
    - The database will be hosted on AWD RDS.
3. All communities and threads will be saved within a database
3. All users input will be retrieved through a fully functional front end.
    - Front end will be built with Angular.
    - Back end will be built with SpringBoot.
    - Front end will be hosted on AWS S3.
4. Logging will be implemented on the backend.
5. There will be frequent use of unit testing.
6. Using Jenkins for pipeline to facilitate CI/CD/CD.

## User Stories: 29 pts
* As a user
    * I can login: 1pt
    * I can logout: 1pt
    * I can register: 2pt
* As a user(in threads and communities)
    * I can view a list of communities and threads: 1pt
    * I can enter a community and thread: 1pt
    * I can write comments into a thread: 3pt
    * I can easily view an updated count of my remaining characters: 1pt
    * I can write replies to comments: 3pt
    * I get characters for getting replies to my messages: 1pt
* As a user(in a community)
    * I can create a thread with a title and initial message: 3pt
* As a thread
    * I have a list of users communicating within this thread: 1pt
    * I will prevent/allow users from messaging depending on their characters bank: 3pt
* As a community:
    * I will delete the oldest thread once a new thread is created and the limit of threads is reached: 1pt
    * I will limit the number of threads to 10 threads: 2pt
* As an admin:
    * I can do all the things that users can do without limited character banks: 2pt
    * I can delete threads: 1pt
    * I can ban a user: 2pt

