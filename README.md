# Bookmarklet-SomaNotaUnicesumar 

```html
<a href="javascript:(function(){
	linha = document.getElementsByTagName("tr")[4];
	linha.insertCell(9);
	linha.getElementsByTagName("td")[9].innerHTML = "TOTAL"
	limite = document.getElementsByTagName("tr").length-8; 
	for(j=5;j<limite+5;j++){     
		total = 0;     
		linha = document.getElementsByTagName("tr")[j];     
		for(i=1;i<9;i++){         
		if(!isNaN(parseInt(linha.getElementsByTagName("td")[i].textContent.replace('.','')))){             
		total = total + parseInt(linha.getElementsByTagName("td")[i].textContent.replace('.',''));         
		}     
	}     
    if(total>=240){cor = "#218530"}
    else {cor = "#851D1D"}
	linha.getElementsByTagName("td")[9].innerHTML = total;
    linha.getElementsByTagName("td")[9].style.color = cor; 
}})();"><button>Arraste ao Favoritos</button></a>

<pre>
    <div class="container">
        <div class="block two first">
            <h2>Your title</h2>
            <div class="wrap">
            //Your content
            </div>
        </div>
    </div>
</pre>
```