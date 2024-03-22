# Perceptrons

### Oq são perceptrons?

- É um tipo de neuronio artificial desenvolvido entre os anos de 1950 e 1960, pelo cientista Frank rosenblatt, que por sua vez foi inspirado no trabalho de Warren McCulloch e Walter Pitss

### Perceptrons são usados?

- O modelo de neuronio artificial mais moderno é o modelo de neuronio sigmoid

### Como um neuronio perceptron funciona?

- Um neuronio perceptron recebe N inputs e devolve um output podendo ser 0 ou 1, cada input que ele recebe, acompanha um Peso (weight) que representa a importancia desse input em relação as demais, A saida de um perceptron é definida por uma regra, é determinado a sua saida se a soma ponderada dos inputs é maior ou menor que um valor de um treshold. uma forma mais programatica ficaria algo assim:

```js
function calculaPerceptron(inputs, treshold) {
  let sum = 0;
  for (let i = 0; i < inputs.length; i++) {
    sum += inputs[i].weigth * inputs[i].value;
  }

  if (sum <= treshold) {
    return 0;
  } else {
    return 1;
  }
}
```

### Oque é o "treshold"?

- esse treshold, na verdade é mais chamado de "bias", pode ser pensar em "O quão facil é de um neuronio perpectron pode retornar 1", por exemplo, com um valor de bias alto, é muito facil o neuronio retornar 1, ou, caso meu valor de bias seja muito baixo, é muito dificil o meu neuronio ativar, logo ele me retorna 0. agora com o bias.
