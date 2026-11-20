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
