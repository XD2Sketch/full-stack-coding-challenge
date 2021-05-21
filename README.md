![magicul-logo](https://user-images.githubusercontent.com/5519740/102984834-a3dad200-4527-11eb-83da-237d3c63cea9.png)

# Full Stack Coding Challenge

The goal of this coding challenge is to demonstrate your skills developing an application across the entire stack (frontend, backend and even a bit of database knowledge).

We wish magicul coding 🚀🧙‍

## General Tech Bla Bla
We’ve designed the technical requirements to match the stack that we currently work with:
- NextJS with TypeScript
- Fastify with TypeScript
- PostgreSQL connected with TypeORM

The architecture will be split between frontend and backend into two separate repositories (no mono-repo). The communication should be implemented using a RESTful API.

## What the tool does
You’ll be building a tool that allows users to upload metadata (file name, file size, file type) of files. The files themselves are not uploaded at all. The frontend then also shows all metadata that was previously uploaded. 

![Desktop HD](https://user-images.githubusercontent.com/5519740/119175937-c3d8d800-ba6a-11eb-8cf5-53a49a981435.jpg)
![Desktop HD 2](https://user-images.githubusercontent.com/5519740/119175947-c5a29b80-ba6a-11eb-8dc9-0b8b7349163f.jpg)

### Acceptance Criteria:
- The user can select a file when clicking “Choose File”
- Once the user has selected a file the button “Reset File” and “Save File” will show up
- The button “Reset File” resets the file selection and brings you back to the default state
- Clicking “Save File” submits the files metadata to the backend
- Clicking “Save File” will also add the file to the table “File History”
- The table “File History” always displays all files that the backend returns
- When the backend receives a request for a file submission the file metadata is stored in the PostgreSQL database
- If the user clicks on the “X” button inside the table, then the frontend request the backend to delete the entry from the database
- Only PDF, DOCX and DOC files are allowed to be uploaded
- The following metadata should be stored: file name, file size, last modified, file format (doc, docx or pdf)


## Boilerplates to get you started

### Frontend:

### Backend:

## Stuff we will pay attention to

### Must-have

#### Frontend & Backend
- TypeScript
- Usage of modern js functionality (ES6+)

#### Frontend:
- NextJS + State Management (ContextAPI/Redux/MobX/xState, … knock yourself out)

#### Backend:
- Fastify or Express
- ORM (TypeORM is recommended)
- Defined REST endpoints

### Nice to have
- Clean code (run linters, prettier)
- Add some tests
- Conventional Commit Messages
- Gitflow Branch Naming

### Very nice to have:
- Github Actions to run linting and tests

### General Stuff:
- How you split code for components
- How your store looks like and how you communicate with redux/mobx
- Reusability of the components
- Code repetitions and reusability (keep your code DRY and simple KISS)
- How and where you put your business logic
- Working in accordance with good practices in general
- How you communicate with API
- Handling unexpected errors or potential exceptions

## Host it!
The hosting is up to you, but we recommend using Heroku for the backend and Vercel for the frontend. If you use heroku then you can use Heroku Postgres otherwise ElephantSQL has a free plan to let you create a hosted managed PostgreSQL database (we use that actually at Magicul).
