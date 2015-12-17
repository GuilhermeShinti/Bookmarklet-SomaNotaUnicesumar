# Bookmarklet-SomaNotaUnicesumar 

## O que é um Bookmarklet?



## Para que serve?

Serve para somar as notas de todas as disciplinas de forma automatizada, gerando o resultado da soma na própria tabela de notas.

## Como usar?

Selecione o código abaixo e arraste aos favoritos, após isso você pode renomear para o que preferir ou simplesmente usar assim mesmo.
Ao entrar na página de notas da Unicesumar, clique nele e pronto. As notas estarão todas somadas.

```
javascript:void%20function(){(function(){function%20e(e,t){parseFloat(linha.getElementsByTagName(%22td%22)[e].textContent)%3EparseFloat(linha.getElementsByTagName(%22td%22)[t].textContent)%3Ftotal-=parseFloat(linha.getElementsByTagName(%22td%22)[t].textContent):total-=parseFloat(linha.getElementsByTagName(%22td%22)[e].textContent)}if(url=%22https://online.cesumar.br/lyceump/aonline/notas_freq.asp%22,window.location.href==url)if(linha=document.getElementsByTagName(%22tr%22)[4],linha.getElementsByTagName(%22td%22)[9])alert(%22As%20notas%20já%20foram%20somadas!%22);else%20for(linha.insertCell(9),linha.getElementsByTagName(%22td%22)[9].innerHTML=%22TOTAL%22,linha.getElementsByTagName(%22td%22)[9].style.font=%22bold%2012px%20arial%22,linha.insertCell(10),linha.getElementsByTagName(%22td%22)[10].innerHTML=%22-F/+S%22,linha.getElementsByTagName(%22td%22)[10].style.font=%22bold%2012px%20arial%22,limite=document.getElementsByTagName(%22tr%22).length-8,j=5;j%3Climite+5;j++){for(total=0,linha=document.getElementsByTagName(%22tr%22)[j],i=1;i%3C9;i++){if(!isNaN(parseFloat(linha.getElementsByTagName(%22td%22)[i].textContent)))switch(i){case%203:e(3,1);break;case%204:e(4,2);break;case%207:e(7,5);break;case%208:e(8,6)}isNaN(parseFloat(linha.getElementsByTagName(%22td%22)[i].textContent))||(total+=parseFloat(linha.getElementsByTagName(%22td%22)[i].textContent))}linha.insertCell(10),total%3E=24%3Fcor=%22%23218530%22:cor=%22%23851D1D%22,linha.getElementsByTagName(%22td%22)[9].innerHTML=total.toFixed(1),linha.getElementsByTagName(%22td%22)[9].style.color=cor,diferenca=total-24,linha.getElementsByTagName(%22td%22)[10].innerHTML=diferenca.toFixed(1),linha.getElementsByTagName(%22td%22)[10].style.color=cor,linha.getElementsByTagName(%22td%22)[10].className=%22font01%22,linha.getElementsByTagName(%22td%22)[10].setAttribute(%22align%22,%22right%22)}else%20confirm(%22Você%20não%20está%20na%20página%20de%20notas%20da%20Unicesumar.\nDeseja%20ser%20redirecionado%20à%20ela%3F%22)%26%26(location.href=%22https://online.cesumar.br/lyceump/aonline/logon.asp%22)})()}();
```