# Manual simples de makedown

___

### Objetivo:

Esse manual tem o objetivo de apresentar a construção de arquivos **MD** sem o uso de tags **HTML**;
___

Markdown é uma linguagem simples de marcação originalmente criada por John Gruber e Aaron Swartz. Markdown converte seu texto em HTML válido. Markdown é frequentemente usado para formatar arquivos README, para escrever mensagens em fóruns de discussão online e para criar rich text usando um editor de texto simples. [Wikipédia](https://pt.wikipedia.org/wiki/Markdown)

___

### Títulos

Como o **HTML**, o MD tem 6 níveis de títulos;

**Exemplo em MD** 
```
# Teste
## Teste
### Teste
#### Teste
##### Teste
###### Teste
```

O referênte está abaixo:

* # # h1 Teste;
* ## ## h2 Teste;
* ### ### h3 Teste;
* #### #### h4 Teste;
* ##### ##### h5 Teste;
* ###### ###### h6 Teste;

___

### Alternativas do "#"

Pode se utilizar os:
* "===" é igual a "#";
* "---" é igual a "##";

Exemplo desses estão abaixo:

Este utiliza o ===
===

Este utiliza o ---
---

___

### Separar linhas


Se utiliza o ```___``` como separador de linhas, o mesmo que a tag ```<hr>``` no **HTML**;

____

### Texto normal

O texto normal não precisa colocar nenhuma marcação, somente escrevê-lo;

___

### Quebrando a linha

Use ```&nbsp;``` para quebrar as linhas, Ex:

```
teste

&nbsp;

teste
```

A saída é:

teste

&nbsp;

teste

___

### Decoração de texto

Não misture métodos de decoração, só dificulta o entendimento final:

##### Itálico:
* *Teste* -> ```*Teste*```
* _Teste_ -> ```_Teste_```

##### BOLD:
* **Teste** -> ```**Teste**```
* __Teste__ -> ```__Teste__```

##### Tachar
* ~~Teste~~ -> ```~~Teste~~```

##### Justando ambos:
* ***Teste*** -> ```***Teste***```
* ___Teste___ -> ```___Teste___```

##### Mistureba (Não recomendado, más possível):
* *__Teste__* -> ```*__Teste__*```
* _**Teste**_ -> ```_**Teste**_```
* **_Teste_** -> ```**_Teste_**```
* __*Teste*__ -> ```__*Teste*__```

____

#### Listas

Valores que se pode usar para criar uma lista:
```
*
-
+
```

Exemplo:

* Uso do ```*``` 
+ uso do ```+```
- Uso do ```-```

Não é recomendavél misturar eles.

Podemos fazer nível tambem, **Exemplo:**

* teste
    * test
        * teste
        
ou:

```
* teste
    * test
        * teste
```

Tem tambem sobre os valores numéricos, **Exemplo:**

| MD | Resultado | 
| --- | --- |
| ```1. teste``` | 1. teste |
| ```5. teste``` | 2. teste |
| ```7. teste``` | 3. teste |
| ```2. teste``` | 4. teste |
| ```4. teste``` | 5. teste |
###### tabela simulada

Esses valores sempre vão seguir numéricamente, então não importa o valor antes do ponto, ele será controlá-do pelo primeiro valor, como **exemplos:**

**MD:**
```
1. teste
4. teste
```
**Saída:**

1. teste
4. teste

**MD:**
```
3. teste
3. teste
66. teste
    1. teste
    3. teste
```
**Saída:**

3. teste
3. teste
66. teste
    1. teste
    3. teste

**Justando dois:**

1. Teste
3. Teste
    - Teste
    - Teste
        - Teste
4. Teste

Ou:

```
1. Teste
3. Teste
    - Teste
    - Teste
        - Teste
4. Teste

```
____

### Bloco de citação

Bloco de citação, **Exemplo:**

```
>Teste
```

O resultado é: 

>Teste

Pode se fazer assim para multiplas linhas:

```
>Teste
Teste
```

O resultado é:

>Teste
Teste

____

### Imagens

Uso de imagens com MD:

![RSA](rsa.png)

Para fazer isso use:

```
![RSA](rsa.png)
```

____

### Tabela

Criando uma tabela, **Exemplo:**

| Cabeçalho | teste | teste | teste| 
| --- | --- | --- | --- |
| Corpo | teste | teste | teste |

**MD:**

```
| teste | teste | teste | teste| 
| --- | --- | --- | --- |
| teste | teste | teste | teste |
```

Tem que se utilizar o divisor ```| --- |``` para separar o cabeçalho do corpo;

Para se criar mais colunas, deve-se criar a quantidade igual entre **Cabeçalho** e **Divisor**;

___

### Links

Para se criar um link de redirecionar:

[Teste](#)

**MD:**
```
[Teste](#).
```

Uso de váriaveis de links:

[teste][1]

[1]: <#> "Teste"

Ou:

**MD:**
```
[teste][1]

[1]: <#> "Teste"
```

___

### Jutabdi link com imagem

Criando uma imagem com link:

[![teste](rsa.png "RSA")](#)

____
