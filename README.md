# Bookmarklet-SomaNotaUnicesumar 

## Como usar?

```
javascript:void%20function(){(function(){if(linha=document.getElementsByTagName(%22tr%22)[4],linha.getElementsByTagName(%22td%22)[9])alert(%22As%20notas%20já%20foram%20somadas!%22);else%20for(linha.insertCell(9),linha.getElementsByTagName(%22td%22)[9].innerHTML=%22TOTAL%22,linha.getElementsByTagName(%22td%22)[9].style.font=%22bold%2012px%20arial%22,limite=document.getElementsByTagName(%22tr%22).length-8,j=5;j%3Climite+5;j++){for(total=0,linha=document.getElementsByTagName(%22tr%22)[j],i=1;i%3C9;i++){if(!isNaN(parseInt(linha.getElementsByTagName(%22td%22)[i].textContent.replace(%22.%22,%22%22))))switch(i){case%203:parseInt(linha.getElementsByTagName(%22td%22)[3].textContent.replace(%22.%22,%22%22))%3EparseInt(linha.getElementsByTagName(%22td%22)[1].textContent.replace(%22.%22,%22%22))%3Ftotal-=parseInt(linha.getElementsByTagName(%22td%22)[1].textContent.replace(%22.%22,%22%22)):total-=parseInt(linha.getElementsByTagName(%22td%22)[3].textContent.replace(%22.%22,%22%22));break;case%204:parseInt(linha.getElementsByTagName(%22td%22)[4].textContent.replace(%22.%22,%22%22))%3EparseInt(linha.getElementsByTagName(%22td%22)[2].textContent.replace(%22.%22,%22%22))%3Ftotal-=parseInt(linha.getElementsByTagName(%22td%22)[2].textContent.replace(%22.%22,%22%22)):total-=parseInt(linha.getElementsByTagName(%22td%22)[4].textContent.replace(%22.%22,%22%22));break;case%207:parseInt(linha.getElementsByTagName(%22td%22)[7].textContent.replace(%22.%22,%22%22))%3EparseInt(linha.getElementsByTagName(%22td%22)[5].textContent.replace(%22.%22,%22%22))%3Ftotal-=parseInt(linha.getElementsByTagName(%22td%22)[5].textContent.replace(%22.%22,%22%22)):total-=parseInt(linha.getElementsByTagName(%22td%22)[7].textContent.replace(%22.%22,%22%22));break;case%208:parseInt(linha.getElementsByTagName(%22td%22)[8].textContent.replace(%22.%22,%22%22))%3EparseInt(linha.getElementsByTagName(%22td%22)[6].textContent.replace(%22.%22,%22%22))%3Ftotal-=parseInt(linha.getElementsByTagName(%22td%22)[6].textContent.replace(%22.%22,%22%22)):total-=parseInt(linha.getElementsByTagName(%22td%22)[8].textContent.replace(%22.%22,%22%22))}isNaN(parseInt(linha.getElementsByTagName(%22td%22)[i].textContent.replace(%22.%22,%22%22)))||(total+=parseInt(linha.getElementsByTagName(%22td%22)[i].textContent.replace(%22.%22,%22%22)))}total%3E=240%3Fcor=%22%23218530%22:cor=%22%23851D1D%22,linha.getElementsByTagName(%22td%22)[9].innerHTML=total,linha.getElementsByTagName(%22td%22)[9].style.color=cor}})()}();```
