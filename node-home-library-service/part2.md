### Basic Scope `0/230`

#### Containerization, Docker `0/130`

- [ ] `Readme.md` has instruction how to run application: `20/20`
- [ ] User-defined `bridge` is created and configured: `30/30`
- [ ] Container auto restarts after crash: `30/30`
- [ ] Application is restarting upon changes implemented into `src` folder: `20/20`
- [ ] Database files and logs are stored in volumes instead of container: `30/30`

#### Database, ORM `0/100`

- [ ] `Users` data is stored in PostgreSQL database and ORM interacts with the database to manipulate data: `20/20`
- [ ] `Artists` data is stored in PostgreSQL database and ORM interacts with the database to manipulate data: `20/20`
- [ ] `Albums` data is stored in PostgreSQL database and ORM interacts with the database to manipulate data: `20/20`
- [ ] `Tracks` data is stored in PostgreSQL database and ORM interacts with the database to manipulate data: `20/20`
- [ ] `Favorites` data is stored in PostgreSQL database and ORM interacts with the database to manipulate data: `20/20`

### Basic Scope `0/130`

#### Containerization, Docker `0/50`

- [ ] Final size of the Docker image with application is less than 500 MB: `20/20`
- [ ] Implemented npm script for vulnerabilities scanning (free solution): `10/10`
- [ ] Your built image is pushed to DockerHub: `20/20`

#### Database, ORM `0/80`

- [ ] Migrations are used to create database entities: `30/30`
- [ ] Variables used for connection to database are stored in `.env`: `10/10`
- [ ] TypeORM decorators or Prisma relations create relations between entities: `10/10`
- [ ] Local PostgreSQL installation is not required for task check, connection is implemented to database stored in docker container: `30/30`

### Forfeits

- [ ] Specific image is not used (it is required to use images like `postgres` and `node`, but not `ubuntu` with installation of `node` or `postgres`): `-20`
- [ ] Postgres container is not configured as dependency for application container: `-20`
- [ ] Failing tests with `npm run test` (`-10` for each): `-360`
- [ ] `docker-compose.yml` contains hardcoded variables: `-20`
- [ ] Commits after deadline, except commits that affect only `Readme.md`, `.gitignore`, etc.: `-108`
- [ ] No Pull Request created: `-40`
- [ ] PR description is incorrect: `-20`
- [ ] No separate development branch: `-40`
- [ ] Less than 3 commits in the development branch, not taking into account commits, making changes only in `Readme.md` or similar files (`tsconfig.json`, `.gitignore`, `.prettierrc.json`, etc.): `-20`
- [ ] Errors either on `npm run lint` on the basis of the local config or for compilation errors on the basis of the local tsconfig (`-10` for each): `-360`
