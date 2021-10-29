# Checklist : Merging to DEV branch

GitHub actions workflows are OK : 
-   Code reviewed
-   Build
-   Linting
-   Compilation
-   Unit tests
-   Code coverage
-   Auto Tests are OK (non regression stress test, robustness connect/disconnect, bootloader)

## Versionning
- [ ]  Version numbers have been incremented in C code files
- [ ]  Version numbers have been incremented in documentation
- [ ]  Version numbers have been incremented in config files (platformio.ini, json, examples apps)

## Documentation
- [ ] Documentation is up to date
- [ ] Changelog is up-to-date with new functionnalities and bug fixes
- [ ] If needed, all new manual tests results are documented

## Quality Assurance
- [ ] Commits policy is respected (constitancy commits, clear commits comments)
- [ ] Code is commented (particularly in hard to understand areas)
- [ ] There are no new warnings that can be corrected
- [ ] Check opened issues don't need to be corrected in current release

## Tests
- [ ]  Manual and Auto Tests for new features are reviewed
- [ ]  All new tests (for bug fixes and for new features) are OK
- [ ]  Existing tests are OK (non regression)
