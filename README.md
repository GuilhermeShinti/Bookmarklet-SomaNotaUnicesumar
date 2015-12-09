# Bookmarklet-SomaNotaUnicesumar 

`
javascript:void function(){(function(){if(linha=document.getElementsByTagName("tr")[4],linha.getElementsByTagName("td")[9])alert("As notas já foram somadas!");else for(linha.insertCell(9),linha.getElementsByTagName("td")[9].innerHTML="TOTAL",limite=document.getElementsByTagName("tr").length-8,j=5;j<limite+5;j++){for(total=0,linha=document.getElementsByTagName("tr")[j],i=1;i<9;i++)isNaN(parseInt(linha.getElementsByTagName("td")[i].textContent.replace(".","")))||(total+=parseInt(linha.getElementsByTagName("td")[i].textContent.replace(".","")));total>=240%3Fcor="%23218530":cor="%23851D1D",linha.getElementsByTagName("td")[9].innerHTML=total,linha.getElementsByTagName("td")[9].style.color=cor}})()}();
`