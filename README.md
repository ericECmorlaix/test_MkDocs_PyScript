# MkDocs Material avec PyScript

Modèle de base pour produire un site web avec MkDocs et le thème Material en lui associant PyScript


> Le site est visible à l'adresse : [https://ericecmorlaix.github.io/test_MkDocs_PyScript/](https://ericecmorlaix.github.io/test_MkDocs_PyScript/)


## Quelques liens :

- https://github.com/pyscript/pyscript
- https://pyscript.net/examples/

- https://realpython.com/pyscript-python-in-browser/

- https://www.lemondeinformatique.fr/actualites/lire-avec-pyscript-le-code-python-s-execute-dans-un-navigateur-86652.html
- https://anaconda.cloud/pyscript-python-in-the-browser



## Quelques notes :

C’est très très cool, on va pouvoir écrire du code Python directement au milieu du code HTML d’une page web !

Une des branches d’avenir pour Python semble donc être celle de Pyodide/WASM[^1] qui permet de faire dialoguer les bibliothèques de Python avec celles de JavaScript directement sur une page web statique chargée sur la machine coté client. C’est le cas de :
-	[Basthon](https://basthon.fr/)
-	[JupyterLite](https://github.com/jupyterlite)
-	[MkDocs+Pyodide]( https://bouillotvincent.gitlab.io/pyodide-mkdocs/)
-	[starboard-notebook](https://github.com/gzuidhof/starboard-notebook)
-	[futurecoder](https://futurecoder.io/)
-	Et bien d’[autres dans le futur](https://pyodide.org/en/stable/project/related-projects.html)

[^1]:  WASM = WebAssembly : https://www.jesuisundev.com/comprendre-webassembly-en-5-minutes/
