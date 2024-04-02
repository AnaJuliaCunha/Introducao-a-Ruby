Bem-vindo! Neste tutorial, você aprenderá conceitos básicos e fundamentais para começar a programar em Ruby. 

## Introdução a Ruby

Ruby é uma linguagem de programação dinâmica, orientada a objetos e de código aberto, conhecida por sua simplicidade e flexibilidade. Vamos começar com alguns conceitos básicos:

### Saída de Dados

O comando 'puts' é usado para imprimir informações na tela. Ele é frequentemente usado para exibir mensagens de boas-vindas, resultados de cálculos ou qualquer outra informação que você queira comunicar ao usuário. Por exemplo:
 
```ruby
puts "Hello World"
```
Este código simplesmente imprimirá "Welcome" na tela quando for executado. (Sempre começando com o famoso "Hello World" para seguir a tradição.)



### Variáveis e Loops
Variáveis em Ruby são usadas para armazenar dados. Você pode pensar nelas como recipientes que guardam valores. 
As variáveis são declaradas colocando um nome seguido do valor. No exemplo abaixo, a variável 'greeting' armazena a string "Welcome!".

    greeting = "Welcome!"

Os loops são usados para repetir a execução de um bloco de código várias vezes, ajudando a simplificar o código. No exemplo abaixo, o bloco puts greeting.upcase será executado três vezes.

```ruby
3.times do
  puts greeting.upcase
end
```

O 'do' inicia o bloco de código que será executado três vezes, uma vez para cada interação do método 'times'. Dentro deste bloco, o código especificado é executado. No caso, a linha 'puts greeting.upcase' está dentro do bloco e será executada três vezes, já que o método times foi chamado com o argumento 3.

O end marca o final do bloco associado ao método times. Tudo o que estiver entre do e end será executado repetidamente de acordo com o número especificado de vezes pelo método times.

Resumindo, o 'do...end' em Ruby é usado para delimitar um bloco de código que será executado em conjunto com uma construção de controle de fluxo, como um loop ou um condicional. Ele define o início e o fim desse bloco de código.


### Números e Strings

Em Ruby, você pode trabalhar com números e strings. Números são usados em cálculos matemáticos, enquanto strings são usadas para representar texto. Você pode até mesmo incluir variáveis dentro de strings usando #{}.


```ruby
movie = "The Avengers" #aqui armazenamos o nome do filme na variável 'movie', para ser chamado posteriormente
puts 25 / 2.0
puts "Mikey's favorite movie is #{movie}"
```


### Métodos e Classes

**Métodos** são blocos de código que realizam uma tarefa específica. Eles são definidos usando a palavra-chave **def** seguida pelo nome do método e, opcionalmente, parâmetros entre parênteses. O corpo do método é delimitado pelas palavras-chave **def e end**.

```ruby
def method_name(parametro)
  código_do_método
end
```

#### Instance Variable

Variáveis de instância são aquelas que ficam disponíveis para cada uma das instâncias de uma classe, ou seja, isoladamente em cada objeto. Variaveis de instância implementam os atributos de uma classe, ou suas variáveis membro e coletivamente representam o estado do objeto. Elas normalmente começam com o sinal @.


Uma **classe** é uma estrutura que define um tipo de objeto. Ela contém métodos e variáveis de instância que descrevem o comportamento e o estado do objeto. Um objeto é uma instância de uma classe.

```ruby
class ClassAnimal
  def initialize(nome)
    @name = Cachorro
  end
  
  def method_name
     puts "O meu animal preferido é o #{@name}."
  end
end
```


No exemplo acima, ClassAnimal é o nome da classe, initialize é um método especial usado para inicializar novos objetos, e method_name é um método regular(que é um bloco de código dentro de uma classe que realiza uma operação específica em um objeto dessa classe).

#### Arrays

Um array é uma estrutura que serve para armazenar uma lista organizada de elementos. Os elementos de um array podem ser acessados por meio de uma lista numérica, começando em 0. E por meios de vários métodos você consegue ir manipulando, adicionando, incluindo, removendo, entre outros . Por exemplo:

```ruby
fruits = ["apple", "banana", "orange"]
puts fruits[0] 
```

<center> TELL, DON'T ASK

![texto](img\tell_img.png) <center/>

Em vez de usar uma função para descobrir primeiro o estado interno e então tomar uma decisão com base nesse estado, podemos dizer ao objeto o que fazer e permitir que ele cuide de seu próprio estado interno.


