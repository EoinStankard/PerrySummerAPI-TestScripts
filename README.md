# PerrySummerAPI-TestScripts
Imagine we are making a private messaging service for our new company Perry’s Summer Vacation Goods and Services. We need you to create an automated test script that verifies the Message API, not User API.

### Requirements of Perry’s Summer Vacation Goods and Services.
**Develop a scalable API to be able to handle the many messages this company is going to handle**

- The application should be a REST API (No need for any kind of UI)

- The application should be ready to run in the cloud or in a container.

- The application data must be persisted in a database of some type.

- The application must be able to create and get users.

- We do not expect you do handle any kind of authentication for users.
  - The application must allow users to send a message to one other user.

- No need to consider group chats.
  - The application must allow editing and deleting messages.

- The application must be able to get all the messages sent between two users.


### Overview
All testing was done in postman, This was my first time using the environment so it took a while to figure out how testing was done and how variables were created. I created a collection with multiple different tests and collection variables were created and updated throughout


### Test Scripts
**Postman link to collection:** https://www.getpostman.com/collections/d071fe7e38f5b6324bcd

All test scripts were exported from postman and are saved as the json file - "PerrysTestScripts.postman_collection.json"
To run these test scripts import the above collection into postman and run the full collection

#### Whats being tested
1. Successfully create a user
2. Read all users and create variables for future tests
3. Create messages from two different users
4. Read messages from different users
5. Delete a user
6. Read messages back from deleted user
7. Create a blank message
8. Verigy if the messages returned are from the correct users
9. Check for blank ids from and to users

#### Issues seen
1. Blank messages can be sent
2. If a user is deleted a message can still be sent with a blank uuid
3. Incorrect messages are being returned
