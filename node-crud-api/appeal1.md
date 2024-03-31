### Basic Scope `69/72`

- [x] The repository with the application contains a `Readme.md` file containing detailed instructions for installing, running and using the application: `10/10`
- [x] GET `api/users` implemented properly: `10/10`
- [x] GET `api/users/{userId}` implemented properly: `10/10`
- [x] POST `api/users` implemented properly: `10/10`
- [x] PUT `api/users/{userId}` implemented properly: `10/10`
- [ ] DELETE `api/users/{userId}` implemented properly: `7/10`

When trying to delete user with valid `userId`, server returns 200 instead of 204.

- [x] Users are stored in the form described in the technical requirements: `6/6`
- [x] Value of port on which application is running is stored in `.env` file: `6/6`

Would be nice to add smth like `.env.example` file to the repo.

### Advanced Scope `70/70`

- [x] Task implemented on Typescript: `30/30`
- [x] Processing of requests to non-existing endpoints implemented properly: `10/10`
- [x] Errors on the server side that occur during the processing of a request should be handled and processed properly: `10/10`
- [x] Development mode: npm script `start:dev` implemented properly: `10/10`
- [x] Production mode: npm script `start:prod` implemented properly: `10/10`

### Hacker Scope `50/80`

- [x] There are tests for API (not less than 3 scenarios): `30/30`
- [ ] There is horizontal scaling for application with a load balancer: `20/50`

The load balancer isn't working properly. It fails when handling the `userId`.  
For instance, after adding a user, I can view the list of all users via `GET api/users`, but I'm unable to retrieve details about a specific user via `GET api/users/{userId}` or delete it using `DELETE api/users/{userId}`.
Furthermore, the state of the database isn't consistent across different workers; it's only preserved for one worker.

### Penalties

- [ ] Any external tools except `nodemon`, `dotenv`, `cross-env`, `typescript`, `ts-node`, `ts-node-dev`, `eslint` and its plugins, `webpack` and its plugins, `prettier` and its plugins, `uuid`, `@types/*` as well as libraries used for testing: `-211`
- [ ] Commits after deadline (except commits that affect only `Readme.md`, `.gitignore`, etc.): `-67`
- [ ] Missing PR or its description is incorrect: `-20`
- [ ] No separate development branch: `-20`
- [ ] Less than 3 commits in the development branch, not including commits that make changes only to `Readme.md` or similar files (`tsconfig.json`, `.gitignore`, `.prettierrc.json`, etc.): `-20`

### Total: `189/222 points`
