---
template: pyscript-custom.html
---

## Intégration d'un REPL PyScript JupyterLike dans une page MarkDown de MkDocs

> Pour chaque cellules ci-dessous, utiliser la combinaison de touches ++"⇑ Maj."+"Entrée ↵"++ pour exécuter le code...

<div>
<py-repl>
def inverse_chaine(chaine):
    chaine_inverse = ''
    for caractere in chaine:
        chaine_inverse = caractere + chaine_inverse
    return chaine_inverse

def est_palindrome(chaine):
    chaine_inverse = inverse_chaine(chaine)
    if chaine.lower() == "kayak" :
        print("'kayak' est un faux ami, à l'envers il fait 'glouglou' !")
    else :
        return chaine == chaine_inverse
</py-repl>
<py-repl>
# test 1 : doit renvoyer 'NSI'
inverse_chaine('ISN')
</py-repl>
<py-repl>
# test 2 : doit renyoyer False
est_palindrome('NSI')
</py-repl>
<py-repl>
# tests 3 : doit renyoyer True
est_palindrome('ISN-NSI')
</py-repl>
<py-repl>
# tests 4 : ???
est_palindrome('kayak')
</py-repl>
<py-repl id="my-repl" auto-generate=true>
# Réaliser vos propres tests :
...
</py-repl>
</div>