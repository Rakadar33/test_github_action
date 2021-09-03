# **Checklist for merging to main branch**

## Commits
- [ ] Verify commits policy is respected  **DEV_PR**
```diff
@@ Note : "History is flatten" (fast-forward merge) + commits propres et découpés en petites fonctionnalités@@
```
- [ ] Every commit compils **DEV_PR**
```diff
@@ Note : A automatiser pour la release + régulièrement sur les rc_candidate, par exemple hebdomadairement@@
```


## Versionning
- [ ] Version numbers has been incremented in code files  **RELEASE_PR**
```diff
@@ Note : all repos Luos + HAL, Examples + profiles + json + platformio.ini...  A voir si c'est facilement automatisable. A priori pas des masses...@@
```
- [ ] Version numbers has been incremented in documentations **RELEASE_PR**


## Documentations
- [ ] Documentation is up to date  **RELEASE_PR**
- [ ] Changelog is up-to-date with new functionnalities  **DEV_PR**
- [ ] Changelog is up-to-date with bug fixes  **DEV_PR**
- [ ] Changelog is up-to-date with known bugs  **DEV_PR**
- [ ] If needed, all new manual tests results are described  **DEV_PR**
- [ ] Changelog is up-to-date with new functionnalities, bug fixes and eventually unfixes known bugs  **RELEASE_PR**
```diff
@@ Note : Doc spécifique ???? dans le code ????@@
```
```diff
@@ Note : for functionalities to deliver with no automatic test : formalize manual tests between Dev team & QA. Final validation by QA@@
```


## Quality Assurance
- [ ] Code is commented (particularly in hard to understand areas) **DEV_PR**
- [ ] There are no new warnings that can be corrected **DEV_PR**  and  **RELEASE_PR**
```diff
@@ Note : A automatiser ???@@
```
- [ ] All new manual tests results are reviewed **DEV_PR**
- [ ] Manual tests are passed OK **DEV_PR**  **RELEASE_PR**
- [ ] All GitHub actions workflows are OK (build, linting, compiled, unit tests ...) **DEV_PR**  **RELEASE_PR**
```diff
@@ Note : C'est fait automatiquement. Peut-être garder la possibilité de ne pas mettre tous les worflows en status check ?@@
```
- [ ] Existing tests (non regression) are passed OK  **DEV_PR**  **RELEASE_PR**
```diff
@@ Note : C'est déjà dans les workflows@@
```
- [ ] Tests for new features exists and are passed OK  **DEV_PR**  **RELEASE_PR**
```diff
@@ Note : C'est déjà dans les workflows en partie : nouveaux tests unitaires + tests autos@@
```
- [ ] Tests for bug fixes exists and are passed OK **DEV_PR**  **RELEASE_PR**
- [ ] Check opened issues don't need to be corrected in current release **RELEASE_PR**
```diff
@@ Note : Revue de Bugs avant release
```
- [ ] If Code coverage < X% = block merge ???
```diff
@@ Note : A automatiser dans... longtemps@@
```


## To be completed if needed
- etc



## TODO after merging to main branch  (deployment job):
- Add a tag version for the new release
- Deployment : Create packages
```diff
@@ Note : A automatiser => création du zip(cf https://github.com/Luos-io/Tools) + envoyer au registery@@
```
```diff
@@ Note : A automatiser => Idem pour pyluos@@
```
- Check publication of Luos libraries are deployed on platformio registry (https://platformio.org/lib)
```diff
@@ Note : A automatiser@@
```
- Non regression test on platformio registry
```diff
@@ Note : A automatiser. Pull les libs + pyluos => Tests à définir @@
```
