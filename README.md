# Setup and Running Instructions

## 1. Setting up environment for Backend

1. Navigate to directory called `yarngitdiff-be` using `cd yarngitdiff-be`
2. Run `yarn install` (Recommended) or `npm install` to install required `node_modules`
3. Run `yarn start` (Recommended) to start the Backend Project.
4. Both APIs are `GET` hence can be run though browser as well as Postman.
5. Postman collection file can be found in the same directory with name as `FS Dev Backend.postman_collection.json`
6. You can use `http://localhost:5000/repositories/ownerName/repoName/commits/commtiHash` for testing 1st API (Get Commit by ID).
7. You can use `http://localhost:5000/repositories/ownerName/repoName/commits/commtiHash/diff` for testing 2nd API (Get the diff of a commit).

## 2. Setting up environment for Frontend

1. Navigate to directory called `yarngitdiff-fe` using `cd yarngitdiff-fe`
2. Run `yarn install` (Recommended) or `npm install` to install required `node_modules`
3. Run `yarn start` (Recommended) to start the Frontend Project.
4. Once project starts, you can navigate to `http://localhost:3000/repositories/ownerName/repoName/commit/commtiHash` to view the UI.


## 3. Notes
> `ownerName`, `repoName`, `commtiHash` to be replaced by actual values. 


