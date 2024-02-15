### Basic Scope `0/240`

#### General `0/16`

- [ ] Application accepts username and prints proper message: `6/6`
- [ ] Application exits if user pressed `ctrl+c` or sent `.exit` command and proper message is printed: `10/10`

#### Operations fail `0/30`

- [ ] Attempts to perform an operation on a non-existent file or work on a non-existent path result in the operation fail: `20/20`
- [ ] Operation fail doesn't crash application: `10/10`

#### Navigation & working directory operations `0/40`

- [ ] Go upper from current directory: `10/10`
- [ ] Go to dedicated folder from current directory: `10/10`
- [ ] List all files and folders in current directory: `20/20`

#### Basic operations with files `0/60`

- [ ] Read file and print its content in console: `10/10`
- [ ] Create empty file: `10/10`
- [ ] Rename file: `10/10`
- [ ] Copy file: `10/10`
- [ ] Move file: `10/10`
- [ ] Delete file: `10/10`

#### Operating system info `0/34`

- [ ] Get EOL (default system End-Of-Line): `6/6`
- [ ] Get host machine CPUs info (overall amount of CPUs plus model and clock rate (in GHz) for each of them): `10/10`
- [ ] Get home directory: `6/6`
- [ ] Get current system user name: `6/6`
- [ ] Get CPU architecture for which Node.js binary has compiled: `6/6`

#### Hash calculation `0/20`

- [ ] Calculate hash for file: `20/20`

#### Compress and decompress operations `0/40`

- [ ] Compress file (using Brotli algorithm): `20/20`
- [ ] Decompress file (using Brotli algorithm): `20/20`

### Advanced Scope `0/90`

- [ ] All operations marked as to be implemented using certain streams should be performed using Streams API: `30/30`
- [ ] No synchronous Node.js API with asynchronous analogues is used (e.g. not used `readFileSync` instead of `readFile`): `20/20`
- [ ] Codebase is written in ESM modules instead of CommonJS: `20/20`
- [ ] Codebase is separated (at least 7 modules): `20/20`

### Penalties `0/-413`

- [ ] Any external tools/libraries are used: `-314`
- [ ] Commits after deadline (except commits that affect only `Readme.md`, `.gitignore`, etc.): `-99`

### Total: `0/330 points`

---
