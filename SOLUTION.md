# Solution Documentation

## 1. Introduction

a. The Problem Statement was to create a full stack application that will show code difference as per the commit id provided for any github repository.
...

## 2. Architecture

- The Architecture for the solution is straight forward.

1. User will open the the base url.
2. Base URL will talk to our Backend.
3. Backend server will talk to GitHub Rest APIs to collect the required data.
4. Once data is received from GitHub, It is shared to frontend for rendering.

...

## 3. Technology Stack

1. React.js for Frontend
2. TypeScript for Type checking
3. Node.js for Backend
4. GitHub REST API for Metadata.
   ...

## 4. Implementation Details

1. User will open the http://localhost:3000/repositories/username/repo_name/commit/commit_hash
2. Once User loads this our Frontend Application will hit the Backend API to collect basic details for users like Commit Name, Commit Author, Parent Commit ID etc.
3. When the API will hit our Backend in Step 2 we will hit GitHub API to collect required data for frontend and push the response.
4. Once data is received, it'll we rendered on the `<Header/>` Component.
5. Parallely we will also hit the Difference API to collect all the patch and hunk which is necessary and follow the same process as Step 2.
6. Once all required data is at frontend we will render our `<Difference />` Component.

...

## 5. Known Limitations
1. Error Handling at Backend as well as Frontend is missing.
2. Invalid Commit ID or any invalid data is not yet parsed at backend.
3. Only test cases are present for  `<Difference />` Component due to time limit.
4. Support is limited to Added or Modified Files. Removed, Empty and assets (svg, png etc) are unsupported.
5. GitHub REST API Rate Limits can cause white page issue.
...

...

## 6. Testing
1. Testing is done for `<Difference />` Component and test cases can be ran using `yarn test` command inside `yarngitdiff-fe` folder.
...

## 7. Future Improvements
1. Error Handling for Backend and Frontend can be added.
2. Support for Empty, Removed and assets (svg, png etc) files.
...

## 8. Setup and Running Instructions
> Included in README.md
...