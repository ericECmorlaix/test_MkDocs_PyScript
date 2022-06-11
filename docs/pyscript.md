<div>
<py-script>
    print("Demat d'an holl")
</py-script>
<br>
<py-script>  
    print("Calculons π :")
    def calcul_pi(n):
        pi = 2
        for i in range(1,n):
            pi *= 4 * i ** 2 / (4 * i ** 2 - 1)
        return pi
    pi = calcul_pi(100000)
    s = f"π vaut approximativement {pi:.5f}"
    print(s)
</py-script>
      <br>
      <strong><p>Aujourd'hui nous sommes le <label id='today'></label></p></strong>
      <br>
      <div id="toto" class="alert alert-primary"></div>
      <py-script>
      import datetime as dt
      pyscript.write('today', dt.date.today().strftime('%A %B %d, %Y'))      
      pyscript.write('toto', f'Toto est dans la place !')
</py-script>
</div>