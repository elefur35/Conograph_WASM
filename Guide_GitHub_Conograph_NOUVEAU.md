Conograph — lancer la compilation WebAssembly via GitHub Actions

Il faut seulement deux fichiers :
1) Conograph_WASM_Validation_Kit.zip (fourni précédemment)
2) compile_conograph_github.yml (accompagnant cette notice)

Sur https://github.com :
1. Créer un nouveau dépôt (New repository), par exemple conograph-wasm-test. Tu peux choisir Private.
2. Dans le dépôt, Add file -> Upload files, puis charger Conograph_WASM_Validation_Kit.zip et Commit changes.
3. Add file -> Create new file ; écrire comme nom : .github/workflows/compile_conograph.yml
4. Copier-coller le contenu du fichier compile_conograph_github.yml dans l'éditeur, puis Commit changes sur la branche principale.
5. Cliquer Actions -> Compiler Conograph en WebAssembly -> Run workflow -> Run workflow.
6. Cliquer l'exécution. Quand elle se termine, ouvrir Artifacts et télécharger Conograph-resultats-compilation.
7. Transmettre ici le ZIP d'artefacts ou le contenu de compilation.log pour analyse.

Une croix rouge signale que la compilation ou le test a échoué : c'est précisément ce que le journal permet de diagnostiquer.
La présence d'un conograph.js ne suffit pas : le test rutile doit aussi réussir.
Le dépôt GitHub n'a pas besoin d'inclure les données DRX expérimentales personnelles.
