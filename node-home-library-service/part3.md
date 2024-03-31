### Basic Scope `0/240`

#### Logging and Error Handling `0/100`

- [ ] Custom `Logging Service` is implemented and used for logging: `20/20`
- [ ] Custom `Exception Filter` is implemented and used for handling exceptions during request processing: `20/20`
- [ ] Logging for request (of at least `url`, `query parameters`, `body`) and response with `status code` is implemented: `20/20`
- [ ] Error handling is implemented including sending response with an appropriate `http status code` and errors logging: `20/20`
- [ ] Error handling and logging is implemented for `uncaughtException` event: `10/10`
- [ ] Error handling and logging is implemented for `unhandledRejection` event: `10/10`

#### Authentication and Authorization `0/140`

- [ ] Route `/auth/signup` implemented correctly, related logic is divided between controller and corresponding service: `30/30`
- [ ] Route `/auth/login` implemented correctly, related logic is divided between controller and corresponding service: `30/30`
- [ ] User password saved into database as hash: `10/10`
- [ ] Access Token is implemented, JWT payload contains `userId` and `login`, secret key is saved in `.env`: `20/20`
- [ ] Authentication is required for the access to all routes except `/auth/signup`, `/auth/login`, `/doc` and `/`: `40/40`
- [ ] Separate module is implemented within application scope to check that all requests to all routes except mentioned above contain required JWT token: `10/10`

### Advanced Scope `0/100`

#### Logging and Error Handling `0/70`

- [ ] Logs are written to a file: `20/20`
- [ ] Logs files are rotated with size: `10/10`
- [ ] Add environment variable to specify max file size: `10/10`
- [ ] Error logs are written to a separate file (either only to a separate file or in addition to logging into a common file): `10/10`
- [ ] Add environment variable to specify logging level and corresponding functionality. Logs with configured level to be registered as well as other higher priority levels. For example if you set level 2, all messages with levels 0, 1 and 2 should be logged. You should use Nest.js logging levels: `20/20`

#### Authentication and Authorization `0/30`

- [ ] Route `/auth/refresh` implemented correctly, related logic is divided between controller and corresponding service: `30/30`

### Forfeits

- [ ] Failing tests with `npm run test:auth` (`-10` for each): `-340`
- [ ] Commits after deadline, except commits that affect only `Readme.md`, `.gitignore`, etc.: `-102`
- [ ] Errors either on `npm run lint` on the basis of the local config or for compilation errors on the basis of the local tsconfig (`-10` for each): `-340`
- [ ] No separate development branch: `-20`
- [ ] No Pull Request: `-20`
- [ ] Pull Request description is incorrect: `-10`
- [ ] Less than 3 commits in the development branch, not taking into account commits, making changes only in `Readme.md` or similar files (`tsconfig.json`, `.gitignore`, `.prettierrc.json`, etc.): `-20`

### Total: `0/340 points`
