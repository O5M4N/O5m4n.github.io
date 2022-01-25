---
title: "Basics for Computer-Networking"
layout: page
categories: [Computer-Networking]
tags: [Computer-networking, Binary Decimal]
---
<br />  
## Conversiones

- [Convertir de Binario a Decimal](https://o5m4n.github.io/Basic-Computer-Networking#convertir-de-binario-a-decimal)
- [Convertir de Decimal a Binario](https://o5m4n.github.io/Basic-Computer-Networking#convertir-de-decimal-a-binario)
<br />  
<br />  
<br />  

### Convertir de Binario a Decimal

**Tabla de Referencia**  

| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |  

<br />
**Ejemplo**  
convertir 101101  
colocamos cada 1 de derecha a izquierda  

<div class="table-wrapper" markdown="block">
  
| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> | Numero |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |     |
|     |     | 1   | 0   | 1   | 1   | 0   | 1   | BIN |
| 0   | 0   | 32  | 0   | 8   | 4   | 0   | 1   | 45  |
  
</div>  

Sumamos los valores y nos da 45  
  
<br /> 
### Convertir de Decimal a Binario

| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |  

<br />
**Ejemplo**  
convertir 78  
comparamos el 78 con cada numero  

<pre>
78 >= 128 = No 
78 >= 64  = SI -> 78 - 64 = 14  
14 >= 32  = NO  
14 >= 16  = NO  
14 >= 8   = SI -> 14 - 8  = 6
6  >= 4   = SI -> 6  - 4  = 2
2  >= 2   = SI -> 2  - 2  = 0
0  >= 1   = NO
</pre>


REMPLAZAMOS LOS SI POR 1 en la tabla  

| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| 0   | 1   | 0   | 0   | 1   | 1   | 1   | 0   |  

78 = 01001110
