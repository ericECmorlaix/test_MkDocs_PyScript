---
template: pyscript-custom.html
---

## Intégration de PyScript dans une page MarkDown de MkDocs

- Le code :
```html
<div>
<py-script>
    print("Demat d'an holl")
</py-script>
<br>
<p><strong>Aujourd'hui nous sommes le <label id='date'></label></strong></p>
<br>
<py-script>  
    print("Calculons π :")
    def calcul_pi(n):
        pi = 2
        for i in range(1,n):
            pi *= 4 * i ** 2 / (4 * i ** 2 - 1)
        return pi
    pi = calcul_pi(100000)
    s = "&nbsp;" * 10 + f"π vaut approximativement {pi:.5f}"
    print(s)
</py-script>
<br>
<div id="toto" class="alert alert-primary"></div>
<py-script>
import time
pyscript.write('date', time.strftime('%d/%m/%Y %H:%M:%S'))      
pyscript.write('toto', f'Toto est dans la place !')
</py-script>
</div>
```
- produit :

<div>
<py-script>
    print("Demat d'an holl")
</py-script>
<br>
<p><strong>Aujourd'hui nous sommes le <label id='date'></label></strong></p>
<br>
<py-script>  
    print("Calculons π :")
    def calcul_pi(n):
        pi = 2
        for i in range(1,n):
            pi *= 4 * i ** 2 / (4 * i ** 2 - 1)
        return pi
    pi = calcul_pi(100000)
    s = "&nbsp;" * 10 + f"π vaut approximativement {pi:.5f}"
    print(s)
</py-script>
<br>
<div id="toto" class="alert alert-primary"></div>
<py-script>
import time
pyscript.write('date', time.strftime('%d/%m/%Y %H:%M:%S'))      
pyscript.write('toto', f'Toto est dans la place !')
</py-script>
</div>

