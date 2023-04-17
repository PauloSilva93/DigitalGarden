---
status: ongoing
---

WWH (Why What How) é uma abordagem pessoal para modularizar e facilitar o design de funções. É semelhante a ideia da [[A estrutura de tema de pirâmide WWH |estrutura de tema de pirâmide WWH]].


## O problema

Quando temos uma ação que deve ser traduzida em código, pensamos em "como fazer x, para que y". Como por exemplo, "como ordenar um array de números para exibí-los no console?"
Perceba como o foco da pergunta é o **COMO** (How) fazer, e não **o que** (What) deve ser feito, e **para que** (Why). Isso nos faz intuitivamente começar a escrever o código pelo algoritmo que descreve a ação principal. Isso é ainda mais comum em linguagens de [[paradigma imperativo]], onde escrevemos "como" as instruções devem ser executadas. 
Mas afinal, por que se preocupar com isso?
Veja este exemplo:

```javascript
let numbers = [3, 5, 2, 1, 4];
for (let i = 0; i < numbers.length; i++) {
    for (let j = 0; j < numbers.length; j++) {
        if (numbers[j] > numbers[j + 1]) {
            let temp = numbers[j];
            numbers[j] = numbers[j + 1];
            numbers[j + 1] = temp;
        }
    }
}
console.log(numbers) // [1, 2, 3, 4, 5]
```

Essa é a forma mais direta de como ordernar um array de forma ascendente, usando [[Bubble Sort]].
* O bloco de código é curto, mas apresenta os seguintes problemas:
	* Alto custo de manutenção: O desenvolvedor muitas vezes precisará ler e depurar o código para entender o que o bloco está fazendo, pois não há nenhum indicativo.
	* Não delimita o contexto da ação: Onde começa e termina essa ação, supondo que este bloco de código estivesse entre outros blocos?
	* Não fornece flexibilidade: Se quisermos executar o mesmo código em diferentes lugares, temos que repetir todas essas linhas do bloco.
	* Não escala facilmente: Para ordenar de forma descendente, precisaríamos repetir todo o bloco, alterando apenas o operador `>` para `<` na condicional `if (numbers[j] > numbers[j + 1])`. 

## Invertendo a pergunta

* Vamos mudar o foco, mudando a pergunta: "como fazer x, para que y" para "para que y, como x deve ser feito?"
* Então, a pergunta inicial que nos levou esse design falho: "como ordenar um array de números para exibí-los no console?", pode ser refeita como "para exibir um array de números ordenados no console, a ordenação deve ser feita como?"
* Agora o foco está no por quê do código. Secundariamente pensamos no que será feito, e finalmente como será feito. O segredo está em transformar o "Why", "What" e "How" em funções, com o nosso foco agora invertido:
	* Why: "Para exibir um array de números ordenados no console". 
		* Começar pelo "Why" nos faz pensar primeiro no que o cliente precisa, e cada cliente pode precisar de números ordenados por um motivo específico.
		* Definir o "Why" da nossa função é isolar o objetivo de uso da função, do "What" e do "How", e deixar que o **o cliente** decida o que fazer.
		* O ideal é que a função do cliente não reflita nem no nome, nem nos parâmetros, o objetivo específico de usar nossa função. Ela deve ser o mais abstrata possível.
		 ```javascript
		class Logger {
			static logNumbers(numbers) {
				console.log(numbers);
			}
		}
		```
	* What: "a ordenação".
		* O "What" nos diz o que o cliente precisa, e apenas isso. Nós podemos nos preocupar com os detalhes depois.
		```javascript
		function sortNumbers(numbers) {
		
			return sortedNumbers;
		}
		```
	* How: "deve ser feita como?".
		* O "How" descreve como a ordenação será feita. É aqui que o algoritmo em si é declarado.
		* É o corpo da função "What"
		* Pode ser uma série de funções ou apenas um bloco de código
		```javascript
		function sortNumbers(numbers) {
			for (let i = 0; i < numbers.length; i++) {
			    for (let j = 0; j < numbers.length; j++) {
			        if (numbers[j] > numbers[j + 1]) {
			            let temp = numbers[j];
			            numbers[j] = numbers[j + 1];
			            numbers[j + 1] = temp;
			        }
			    }
			}
			return sortedNumbers;
		}
		```

## Versão refatorada

 ```javascript
	class Logger {
		static logNumbers(numbers) {
			console.log(numbers);
		}
	}

	function sortNumbers(numbers) {
		for (let i = 0; i < numbers.length; i++) {
			for (let j = 0; j < numbers.length; j++) {
				if (numbers[j] > numbers[j + 1]) {
					let temp = numbers[j];
					numbers[j] = numbers[j + 1];
					numbers[j + 1] = temp;
				}
			}
		}
		return numbers;
	}
	
	// usage
	let sortedNumbers = sortNumbers(numbers);
	Logger.logNumbers(sortedNumbers); // [1, 2, 3, 4, 5]
	```

## Deixando o cliente decidir como

Às vezes o cliente quer especificar detalhes do algoritmo para atender necessidades mais específicas. Imagine por exemplo que o cliente precise ordenar os números em ordem decrescente. Nesse caso, a vantagem de ter isolado o "How" é evidente: podemos usar o padrão [[Strategy]] para definir estratégias de ordenação diferentes, e permitir que o cliente escolha qual usar.