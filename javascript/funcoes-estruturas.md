# ARRAYS

```javascript


    //Índice dos arrays se inicia em 0
    const carros = ['Gol',
     'Ranger', 
     'Maverick', 
     'Fiesta'
     ]

    console.log(carros)
    console.table(carros)

    //Adiciona um elemento ao final do array
    carros.push('Ferrari)

    //Adiciona um elemento no início do array
    carros.unshift('Camaro')

    //Remove um elemento pelo final do array
    carros.pop()

    //Remove um elemento a partir do início do array
    carros.shift()

    //Os comandos de retirada de um elemento retorna o elemento que foi retirado quando chamado
    const carro = carros.shift()
    const carro = carros.pop()

    //Vai pra o index 1 e exclui 2 itens(exclui a partir do index 1)
    carros.splice(1, 2)

    //Vai pra o item 1, não exclui nenhum item e adiciona o item 'Toro'
    carros.splice(1, 0, 'Toro')

    //Vai pra o item 1, exclui 1 item e adiciona o 'Uno'
    carros.splice(1, 1, 'Uno')

    //Altera a ordem dos itens para ordem alfabética
    carros.sort()
    

    //Outra forma de criar um array:

    const anos = new Array(1998, 2026, 2032)


```

# Arrays Multidimensionais(Matrizes)


```javascript

    const notas = [
        [5, 10, 6, 8],
        [9, 7, 4, 3],
        [2, 10, 8, [4, 5, 6, 8] ]

    ]

    //Pega o dado na posição x, dado x
    console.table([2][3])

    //Pega o dado na posição x, dado x(OUTRO ARRAY), item x
    console.table([2][3][2])

    //Pode-se fazer um array de objetos

    //Importante saber o tipo de dado de cada item dentro do array

```


# Funções


```javascript


    //Presume-se que há código html com os id's utilizados nessa função
    //Padrão de função mais utilizado
    Function  somar() {
        const n1 = Number(document.getElementById('n1').value)
        const n2 = Number(document.getElementById('n2').value)

        const soma = n1 + n2

        document.getElementById('resultado').innerHTML = 'A soma dos números é ' + soma

    }

    //Para linkar o código JS ao html utiliza-se o código abaixo:
    <script type='text/javascript' src='js/funcoes.js'></script>

    //Padrões de função menos utilizados

    const somaExpressao = function(n1, n2) {
        return n1 + n2
    }

    const somaArrow = (n1, n2) -> {
        return n1 + n2
    }

```
