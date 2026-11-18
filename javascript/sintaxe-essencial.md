**Estruturas de condição** 

# IF/ELSE e Operador Ternário

## Exemplo
```javascript

    //Number -  Converte o valor para tipo int/float.
    //prompt - Quando usado no html abre uma caixa(alert) na tela estimulando a interação para receber algum dado.
    //const - é o tipo de variável CONSTANTE.
    const n1 = Number(prompt('Digite a nota 1'))
    const n1 = Number(prompt('Digite a nota 2'))
    const n1 = Number(prompt('Digite a nota 3'))
    const n1 = Number(prompt('Digite a nota 4'))

    const media = (n1 + n2 + n3 + n4) / 4

    console.log("A média final é " + media)

    if(media >= 7) {
        console.log("Aprovado!")
    } else if(media < 5) {
        console.log("Reprovado :(")
    } else {
        console.log("Recuperação. Estude mais para passar.")
    }

    

    const n1 = Number(prompt('Digite a nota 1'))
    const n1 = Number(prompt('Digite a nota 2'))
    const n1 = Number(prompt('Digite a nota 3'))
    const n1 = Number(prompt('Digite a nota 4'))

    const media = (n1 + n2 + n3 + n4) / 4

    console.log("A média final é " + media)
    
    //IF Ternário
    media >= 7 ? console.log('Aprovado') : console.log('Reprovado')
    //Outra forma 
    let mensagem = media >=7 ? 'Aprovado' : 'Reprovado'
    console.log(mensagem)


```

# Switch Case

## Exemplo

```javascript


    /* Verificar o aumento de salário com os seguintes cargos:

    Estagiário: 100%
    Analista: 50%
    Gerente: 30%
    Presidente: 10%
    */
    const salario = prompt('Digite um Salário')
    const cargo = prompt('Digite um cargo')
    
    //let - variável q pode ser reatribuída
    let aumento = 0

    switch(cargo) {
        case 'Estagiário':
        case 'Analista':
            aumento = 2;
            break;
        case 'Gerente':
            aumento = 1.5;
            break;
        case 'Presidente':
            aumento = 1.1;
            break;
        default: alert('Favor escolher um cargo válido!')
    }

    const novoSalario = salario * aumento
    console.log("O novo salário é: R$ " + novoSalario)

``` 

**Estruturas de repetição**

## While / Do while

# Exemplos

```javascript

    let contador = 1
    const qtd = prompt('Quantas notas para tirar a média?')
    let soma = 0
    let nota = 0
    const media = soma / qtd

    while(contador <= qtd) {
        nota = Number(prompt('Digite a nota' + contador))
        soma = soma + nota
        contador++
    }

    

    console.log('Soma: ' + soma)
    console.log('Nota: ' + nota)
    console.log('Média: ' + media)

    const resultado = media >= 7 ? 'Aprovado' : 'Reprovado'
    console.log('O seu resultado foi ' + resultado)

    //Do While
    /*Faça(do) tal comando e repita o loop enquanto(while) determinada condição for aceita. O Do executa ao menos 1 vez o código até verificar a condição do While
    */
    
    do {
         nota = Number(prompt('Digite a nota' + contador))
    } while(nota > 10)


```