# **Checklist for merging to main branch**

## Commits
- [ ] Verify commits policy is respected
```diff
@@ Note : "History is flatten" + commits propres et découpés en petites fonctionnalités@@
```
- [ ] Every commit compils
```diff
@@ Note : A automatiser pour la release + régulièrement sur les rc_candidate, par exemple hebdomadairement@@
```


## Versionning
- [ ] Version numbers has been incremented in code files
```diff
@@ Note : all repos Luos + HAL, Examples + profiles + ...  A voir si c'est facilement automatisable@@
```
- [ ] Version numbers has been incremented in documentations


## Documentations
- [ ] Documentation is up to date
- [ ] Changelog is up-to-date with new functionnalities
- [ ] Changelog is up-to-date with bug fixes
- [ ] Changelog is up-to-date with known bugs
- [ ] All new manual tests results are described
```diff
@@ Note : Doc spécifique ???? dans le code ????@@
```
```diff
@@ Note : for functionalities to deliver with no automatic test : formalize manual tests between Dev team & QA. Final validation by QA@@
```


## Quality Assurance
- [ ] Code is commented (particularly in hard to understand areas)
- [ ] There are no new warnings
```diff
@@ Note : A automatiser ???@@
```
- [ ] All new manual tests results are reviewed
- [ ] Manual tests are passed OK
- [ ] All GitHub actions workflows are OK (build, compiled, unit tests ...)
```diff
@@ Note : C'est fait automatiquement. Peut-être garder la possibilité de ne pas mettre tous les worflows en status check ?@@
```
- [ ] Existing tests (non regression) are passed OK
```diff
@@ Note : C'est déjà dans les workflows@@
```
- [ ] Tests for new features exists and are passed OK
```diff
@@ Note : C'est déjà dans les workflows en partie : nouveaux tests unitaires + tests autos@@
```
- [ ] Tests for bug fixes exists and are passed OK
- [ ] Check opened issues don't need to be corrected in current release
- [ ] If Code coverage < X% = block merge ???
```diff
@@ Note : A automatiser@@
```


## To be completed if needed
- etc



## TODO after merging to main branch :
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
