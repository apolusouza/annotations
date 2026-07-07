`"As vezes é preciso aprender a correr antes de começar a andar...." `
_`Tony Stark - Iron man.`_

### **Índice**

1\. Estrutura básica do projeto e método Main
* <input type="checkbox" id="opcao" name="opcao">Organização de código em pacotes #pacotes
2\. Fundamentos da Linguagem
   
- <input type="checkbox" id="opcao" name="opcao">Declaração e Nomenclatura de Variáveis (CamelCase) #nomenclatura
* <input type="checkbox" id="opcao" name="opcao">Tipos Primitivos Inteiros (byte, short, int, long)  #primitivos
* <input type="checkbox" id="opcao" name="opcao">Tipos Primitivos Decimais (float, double)  #primitivos
* <input type="checkbox" id="opcao" name="opcao">Tipos de Texto e Caractere (String, char)  #primitivos 
* <input type="checkbox" id="opcao" name="opcao">Tipos Lógicos (boolean)  #primitivos
* <input type="checkbox" id="opcao" name="opcao">Inferência de Tipo com var  #var
* <input type="checkbox" id="opcao" name="opcao">Classes Wrappers (Byte, Short, Integer, Long, Float, Double, Character, Boolean)  #wrappers

3\. Manipulação de Dados e Entrada/Saída

* <input type="checkbox" id="opcao" name="opcao">Concatenação de Strings #strings  
* <input type="checkbox" id="opcao" name="opcao">Entrada de dados pelo usuário via terminal (Classe Scanner) #EntradaDeDados

4\. Operadores

* <input type="checkbox" id="opcao" name="opcao">Operadores Aritméticos `(+,-,*, /,%) ` #aritmeticos
* <input type="checkbox" id="opcao" name="opcao">Operadores de Igualdade `(==, !=)` #igualdade
* <input type="checkbox" id="opcao" name="opcao">Operadores Relacionais `(>, >=, <, <=)`  #relacionais
* <input type="checkbox" id="opcao" name="opcao">Operadores Lógicos `(&&, ||)` #logicos
* <input type="checkbox" id="opcao" name="opcao"> Operadores de atribuição #atribuicao

5\. Estruturas de Controle e Decisão

* <input type="checkbox" id="opcao" name="opcao">Condicionais com if, else if, else  #condicionais1
* <input type="checkbox" id="opcao" name="opcao">Condicionais com switch, case, break, default #condicionais2

6\. Estruturas de Repetição (Loops)

* <input type="checkbox" id="opcao" name="opcao">Laços: while, do-while e for  #while
* <input type="checkbox" id="opcao" name="opcao">Controle  de laços: break e continue #for

7\. Estruturas de Dados Básicas

* <input type="checkbox" id="opcao" name="opcao">Arrays (Declaração, índices e iteração) #arrays

8\. Programação Orientada a Objetos (POO)

* <input type="checkbox" id="opcao" name="opcao">Conceitos de Classe e Objeto  
* <input type="checkbox" id="opcao" name="opcao">Propriedades (Atributos/Variáveis de Instância)  
* <input type="checkbox" id="opcao" name="opcao">Métodos (Comportamentos/Ações)  
* <input type="checkbox" id="opcao" name="opcao">Métodos Getters e Setters  
* <input type="checkbox" id="opcao" name="opcao">Construtores  
* <input type="checkbox" id="opcao" name="opcao">Variáveis de Classe (Modificador static)  
* <input type="checkbox" id="opcao" name="opcao">Herança (extends e palavra-chave super)  
* <input type="checkbox" id="opcao" name="opcao">Modificadores de Acesso (public, private, protected)  
* <input type="checkbox" id="opcao" name="opcao">Interfaces e Implementações (implements e override)

9 . Programação Orientada a Objetos
- Introdução a Classes, Objetos e Coesão
- Referência de Objetos
- Métodos
- Referência `this`
- Varargs


## **Organização de código em pacotes** #pacotes 

```Md
📁 curso de Java/                              
└── 📁 src/                                    
    ├── 📄 Main.java                           
    │  
    ├── 📁 programação orientada a objetos/    
    │   ├── 📄 Carro.java                      
    │   └── 📄 Conta.java                      
    │  
    ├── 📁 herança/                            
    │   ├── 📄 Veiculo.java                    
    │   └── 📄 Moto.java                       
    │  
    └── 📁 interfaces/                         
        └── 📄 Veiculo.java  
        
``` 

#### Entendendo a organização visual:  

**Curso de Java:** É a pasta raiz do projeto, escolhida no momento da criação na IDE.  
**src:** É a pasta principal de código-fonte (source). Todo o código que você escreve fica obrigatoriamente dentro dela.  

**Main.java:** É o arquivo da classe principal que fica solto logo na entrada da pasta src (no pacote principal). É dentro deste arquivo que reside o método estático principal (public static void main(String\[\] args)), sendo o ponto de entrada onde toda a execução do programa de fato acontece.  

**Pastas internas (Pacotes):** Ao expandir a aplicação, criam-se pacotes para separar as responsabilidades e organizar os arquivos. No exemplo visual, estão as subpastas criadas para programação orientada a objetos, herança e interfaces, contendo suas respectivas classes e modelos de objetos.

A estrutura básica de um projeto Java é organizada de forma que os arquivos de código-fonte fiquem armazenados dentro de uma pasta chamada src. Dentro dessa pasta, localizam-se os pacotes e o arquivo da classe principal, como por exemplo, Main.java.  
Para que a aplicação consiga executar o seu código, é obrigatório existir uma função principal, que consiste em uma classe e um método estático main. Esse método recebe um array de Strings como parâmetro e serve como o ponto de entrada do sistema, ou seja, é dentro dele que a execução do seu programa de fato acontece. Abaixo está um exemplo de código ilustrando essa estrutura fundamental:

```Java
// Classe principal do arquivo  
public class Main {  
      
    // Método estático principal, obrigatório para a execução do código  
    public static void main(String\[\] args) {  
          
        // O código da sua aplicação será executado aqui dentro  
        System.out.println("Executando o projeto\!");  
          
    }  
}
```
## **Declaração da nomenclatura** #nomenclatura 

Por padrão existe uma  convenção de ser usado o CamelCase nas váriavés de Java ex: IdadeAluno ou IdadeAluno

## **Os tipos primitivos** #primitivos 

| Tipo | Explicação | Exemplo de Código |
| ----- | ----- | ----- |
| byte | Ocupa 1 byte na memória e armazena números inteiros de \-128 a 127\. É útil para economizar memória com valores pequenos, como a idade. | byte idade \= 120; |
| short | Ocupa 2 bytes e suporta números inteiros maiores, variando de \-32.768 até 32.767. | short estoque \= 32000; |
| int | Ocupa 4 bytes e suporta números inteiros na faixa de até aproximadamente 2 bilhões. É o padrão para a maioria dos números inteiros. | int numero \= 2000000000; |
| long | Ocupa 8 bytes, utilizado para números inteiros gigantescos (ex: dados bancários). Obrigatoriamente o valor deve terminar com a letra L maiúscula. | long contaCorrente \= 9999999999999L; |
| float | Ocupa 4 bytes e armazena números fracionados (decimais) suportando até 7 casas de precisão. Exige a inserção da letra f ao final do valor. | float real \= 10.50f; |
| double | Ocupa 8 bytes e possui precisão muito maior para decimais, aguentando até 15 casas após o ponto. Não requer nenhuma letra ao final da declaração. | double dolar \= 50.123456789012345; |
| char | Suporta a inserção de apenas um único caractere (uma letra, um símbolo, etc.), e o seu valor deve ser delimitado por aspas simples. | char minhaLetra \= 'a'; |
| boolean | Utilizado para validar estados lógicos, aceitando apenas dois valores: verdadeiro (true) ou falso (false). | boolean botaoAtivado \= true; |

## **Inferência de tipo com var** #variaveis 

```Java
// O sistema infere automaticamente que a variável é do tipo String  
var sobrenome = "Duarte Gomes";

// O sistema infere que a variável é do tipo número inteiro (int)  
var numero = 10;

// O sistema infere que a variável é do tipo Double (decimal)  
var valorFracionado = 50.50;

// O sistema infere que a variável é do tipo char (caractere único)  
var minhaLetra = 'a';

```

Ao utilizar a palavra var, você não precisa especificar o tipo de dado explicitamente, pois o sistema reconhece e define automaticamente o tipo da variável com base no valor que está sendo atribuído a ela  Por exemplo, ao inserir um texto entre aspas duplas, ele o reconhece como String; ao inserir um número sem casas decimais, ele o lê como inteiro, e assim por diante

## **Classes Wrappers (Byte, Short, Integer, Long, Float, Double, Character, Boolean)** #wrappers 

A palavra wrapper em inglês significa "embrulho" ou "capa". O que essas classes fazem é literalmente "embrulhar" um tipo primitivo (que é apenas um dado cru na memória) para transformá-lo em um Objeto.

O Java possui tipos primitivos como int, double, char e boolean. Eles são excelentes para performance porque guardam apenas o valor bruto e não ocupam muito espaço.

A limitação: Eles não são objetos. Portanto, um int não tem métodos atrelados a ele. Você não pode digitar meuNumero. e esperar que o Java sugira alguma ação. Além disso, estruturas de dados no Java (como o ArrayList) só aceitam objetos. Você não pode criar um ArrayList\<int\>, precisa ser um ArrayList\<Integer\>.

Para resolver essa limitação, o Java fornece uma Classe Wrapper correspondente para cada tipo primitivo. Elas geralmente começam com letra maiúscula (padrão para classes em Java):

```M̀d
int -> Integer

double -> Double

char -> Character

boolean -> Boolean  
(O mesmo vale para Byte, Short, Long e Float).

```

```Java
// 1\. Usando tipo primitivo (apenas o valor, sem métodos)  
int numeroPrimitivo \= 10;  
// numeroPrimitivo. ??? \-\> Não há métodos disponíveis. Não compila.

// 2\. Usando a Classe Wrapper (é um objeto, cheio de métodos)  
Integer numeroWrapper \= 10; 

// Agora você pode usar métodos úteis\!  
String texto \= numeroWrapper.toString();  // Converte o número para texto ("10")  
int max \= Integer.max(10, 20);            // Retorna o maior número entre os dois  
int convertido \= Integer.parseInt("123"); // Lê um texto e transforma em número
```
## **Concatenação de Strings** #strings 

A concatenação de strings na linguagem Java é o conceito de juntar textos e valores de variáveis para montar mensagens ou frases mais completas e dinâmicas.  
Principais características: Operador Utilizado: Para realizar a concatenação, utiliza-se o sinal de soma (+). Comportamento com Textos vs. Números: Quando o sinal de \+ é aplicado em um contexto que envolve String (textos), o sistema entende que deve unir os valores lado a lado, e não realizar uma operação matemática de soma. Por exemplo, ao tentar "somar" duas variáveis de texto contendo "10" e "20", o resultado gerado será "1020", pois os textos foram apenas juntados.  
Textos Fixos e Dinâmicos: A grande vantagem da concatenação é permitir a mescla de textos fixos (escritos diretamente no código entre aspas duplas) com valores dinâmicos (oriundos de variáveis), permitindo que a frase mude automaticamente caso o valor da variável seja alterado.

Exemplo prático de código:  
String nome \= "Marcos";  
int idade \= 30;

// Utilizando o sinal de \+ para concatenar textos fixos com os valores das variáveis  
System.out.println("Meu nome é " \+ nome \+ " e eu tenho " \+ idade \+ " anos.");  
A saída deste código exibirá: Meu nome é Marcos e eu tenho 30 anos.

## **Entrada de dados pelo usuário via terminal (Classe Scanner)** #EntradaDeDados 

   
A classe Scanner em Java é utilizada para capturar e ler dados inseridos pelo usuário através do terminal . Essa ferramenta é fundamental para tornar os programas dinâmicos e interativos, pois permite que a aplicação receba valores em tempo de execução, em vez de depender apenas de dados fixos escritos diretamente no código.  

**Principais características e funcionamento:** Instanciação (System.in): Para utilizar o Scanner, é necessário criar (instanciar) um objeto da classe passando o parâmetro System.in. O in significa Input Stream (fluxo de entrada), indicando que o sistema deve aguardar a inserção de um dado, diferentemente do System.out, que é usado para saída de dados.  

**Leitura de Textos (String):** Para capturar textos, utiliza-se o método .nextLine(). Esse método lê o que o usuário digitou e automaticamente passa a leitura para a próxima linha.  

**Leitura de Números:** A classe possui métodos específicos para capturar dados numéricos de acordo com o seu tipo, como o .nextByte(), .nextInt(), .nextDouble(), etc..  

**Comportamento de quebra de linha:** É importante ter atenção ao misturar a leitura de números com textos. Métodos numéricos, como o .nextByte(), capturam o valor numérico mas não consomem a quebra de linha do terminal (quando o usuário aperta Enter), o que pode fazer com que o próximo .nextLine() seja ignorado. Em algumas situações, a recomendação é ler tudo como String com .nextLine() e converter os valores, ou organizar as perguntas numéricas por último.

Exemplo prático de código:  
```Java
// 1\. Instanciando o Scanner para receber dados do sistema  
Scanner entradaUsuario \= new Scanner(System.in);

System.out.println("Qual é o seu nome?");  
// 2\. Capturando um texto digitado pelo usuário  
String nome \= entradaUsuario.nextLine();

System.out.println("Qual é a sua idade?");  
// 3\. Capturando um valor numérico (byte) digitado pelo usuário  
byte idade \= entradaUsuario.nextByte();

System.out.println("Meu nome é " \+ nome \+ " e tenho " \+ idade \+ " anos.");
```

## **Operadores aritméticos(+, \-, \*, /, %)** #aritmeticos 

Os operadores aritméticos na linguagem Java são fundamentais para realizar cálculos e operações matemáticas básicas dentro da aplicação.  

Aqui está o resumo de cada um deles:

**Soma (+):** Realiza a adição entre dois valores numéricos. Atenção: Existe uma diferença de contexto. Se o sinal de + for utilizado entre números (inteiros ou decimais), ele faz um cálculo matemático. No entanto, se houver qualquer variável de texto (String) no meio, ele deixa de somar e passa a concatenar (juntar) os textos.  

**Subtração (-):** Subtrai um valor do outro. O resultado pode ser negativo caso o número subtraído seja maior que o número inicial.  

**Multiplicação (*)**: Representada pelo asterisco, realiza a multiplicação comum entre dois números.  

**Divisão (/):** Representada pela barra, realiza a divisão de um valor pelo outro. Ao trabalhar com divisão na programação, muitas vezes é recomendado utilizar variáveis decimais (como o double, ex: 5.0 / 10) para que o resultado exiba as casas decimais corretamente em vez de retornar zero.  
**Resto da Divisão (%):** Representado pelo sinal de porcentagem, esse operador não entrega o valor final da divisão, mas sim o resto que sobra dela. É muito utilizado na programação para descobrir se um número é par ou ímpar, por exemplo.  

Exemplos de código:  

```Java
int numero1 \= 10;  
int numero2 \= 20;

// Soma  
System.out.println(numero1 \+ numero2); // Resultado: 30

// Subtração  
System.out.println(numero2 \- numero1); // Resultado: 10

// Multiplicação  
System.out.println(numero1 \* numero2); // Resultado: 200

// Divisão (utilizando decimais para maior precisão)  
System.out.println(5.0 / 10); // Resultado: 0.5

// Resto da divisão (55 dividido por 7 tem resto 6\)  
System.out.println(55 % 7); // Resultado: 6

```

## **Operadores de Igualdade `(==, !=)`** #igualdade 

Os operadores de igualdade na linguagem Java são utilizados para comparar dois valores e determinar se eles são equivalentes ou distintos. A principal característica desses operadores é que eles sempre retornam um resultado lógico (booleano), ou seja, apenas verdadeiro (true) ou falso (false)  
.  
Aqui estão os dois operadores de igualdade:  

**Igual a `(==)` :** Representado obrigatoriamente por dois sinais de igual juntos. Ele verifica se o valor de um lado é exatamente igual ao valor do outro. Atenção: Na programação Java, um único sinal de igual (=) é usado para atribuir um valor a uma variável, enquanto os dois sinais `(==)` são usados para fazer a comparação.  

**Diferente de (!=):** Representado por um ponto de exclamação seguido de um sinal de igual. Ele verifica se os valores comparados são diferentes. Se de fato forem diferentes, ele retorna verdadeiro (true); se forem iguais, retorna falso (false).  

Exemplo prático de código:  

```Java
int numero1 \= 10;  
int numero2 \= 10;  
int numero3 \= 50;

// Operador de Igual (==)  
// 10 é igual a 10? Sim, então retorna true.  
System.out.println(numero1 \== numero2); // Resultado: true 

// 50 é igual a 10? Não, então retorna false.  
System.out.println(numero3 \== numero1); // Resultado: false 

// Operador de Diferente (\!=)  
// 50 é diferente de 10? Sim, então retorna true.  
System.out.println(numero3 \!= numero1); // Resultado: true 

// 10 é diferente de 10? Não (são iguais), então retorna false.  
System.out.println(numero1 \!= numero2); // Resultado: false 
```

## **Operadores Relacionais (\>, \>=, \<, \<=)** #relacionais 

Os operadores relacionais são utilizados para analisar a relação de grandeza entre dois valores (se um é maior, menor ou igual ao outro). Assim como os operadores de igualdade, o resultado de uma operação relacional será sempre um estado lógico (booleano), retornando apenas verdadeiro (true) ou falso (false)  
.  
Aqui estão os operadores relacionais da linguagem Java:  
Maior que (\>): Verifica se o valor do lado esquerdo é estritamente maior do que o valor do lado direito  
.  
Maior ou igual a (\>=): Verifica se o primeiro valor é maior OU igual ao segundo. Na prática, o sistema faz duas comparações muito rápidas: se o número não for maior, ele verifica em seguida se é igual. Se pelo menos uma das comparações for verdadeira, o resultado final será verdadeiro  
.  
Menor que (\<): Representado pelo sinal virado para a esquerda, verifica se o valor do lado esquerdo é estritamente menor que o da direita  
.  
Menor ou igual a (\<=): Verifica se o valor é menor OU igual ao outro, operando com a mesma lógica de dupla verificação descrita no operador maior ou igual  
.  
Exemplo prático de código:  


```Java
int numero1 \= 10;  
int numero2 \= 20;

// Operador Maior que (\>)  
// 10 é maior que 20? Não, então retorna false.  
System.out.println(numero1 \> numero2); // Resultado: false 

// Operador Maior ou igual (\>=)  
// 20 é maior que 20? Não. Mas 20 é igual a 20? Sim. Então retorna true.  
System.out.println(numero2 \>= 20); // Resultado: true 

// Operador Menor que (\<)  
// 10 é menor que 20? Sim, então retorna true.  
System.out.println(numero1 \< numero2); // Resultado: true 

// Operador Menor ou igual (\<=)  
// 10 é menor que 10? Não. Mas 10 é igual a 10? Sim. Então retorna true.  
System.out.println(numero1 \<= 10); // Resultado: true 
```
## **Operadores Lógicos (&&, ||)** #logicos 

Os operadores lógicos na linguagem Java são utilizados para combinar múltiplas comparações ou verificações dentro de uma única condição, como na estrutura de um if. O resultado final da avaliação desses operadores será sempre um valor booleano: verdadeiro (true) ou falso (false).

Aqui estão os dois principais operadores lógicos:  
**Operador OU `(||)`:** Representado por dois pipes (barras verticais). Esse operador verifica múltiplas condições e retorna verdadeiro se pelo menos uma das comparações for verdadeira. 

Ele só retornará falso se absolutamente todas as verificações forem falsas.  

**Operador E `(&&)`:** Representado por dois E comerciais. Diferente do operador OU, o operador E exige estritamente que todas as comparações sejam verdadeiras para que o resultado final seja verdadeiro. Se apenas uma das condições analisadas for falsa, o bloco inteiro retornará falso, mesmo que as outras sejam verdadeiras.  

Exemplo prático de código:

```Java
int numero1 \= 10;  
int numero2 \= 20;  
int numero3 \= 30;  
int numero4 \= 40;

// Operador Lógico OU (||)  
// 10 é igual a 20? (Falso) OU 30 é menor que 40? (Verdadeiro).  
// Como pelo menos uma condição é verdadeira, o IF será executado.  
if (numero1 \== numero2 || numero3 \< numero4) {  
    System.out.println("Verdadeiro");   
}

// Operador Lógico E (&&)  
// 10 é menor que 20? (Verdadeiro) E 30 é igual a 40? (Falso).  
// Como uma das condições falhou (é falsa), o resultado final é falso, indo para o else.  
if (numero1 \< numero2 && numero3 \== numero4) {  
    System.out.println("Verdadeiro");  
} else {  
    System.out.println("Falso");  
}
```

## **Operador Ternário**

O **operador ternário** foi criado no Java para **simplificar as condições `if` e `else`**, sendo extremamente útil quando você precisa avaliar uma condição e **atribuir o resultado diretamente a uma variável** em uma única linha.

Sua sintaxe é dividida em três partes:

1. A **condição** a ser avaliada.
2. Um sinal de interrogação (**`?`**), seguido pelo valor que será retornado caso a condição seja **verdadeira**.
3. O sinal de dois pontos (**`:`**), seguido pelo valor que será retornado caso a condição seja **falsa**.

Uma regra fundamental na utilização desse operador é que os tipos dos valores retornados (tanto no verdadeiro quanto no falso) **precisam obrigatoriamente ser compatíveis com o tipo da variável** que receberá a atribuição.

**Exemplo de código:** Abaixo, temos um exemplo prático demonstrando o funcionamento do operador ternário para decidir o texto de uma mensagem baseada no valor do salário:

```Java
public class OperadorTernario {
    public static void main(String[] args) {

        double salario = 6000.0;

        // Sintaxe: condição ? valor_se_verdadeiro : valor_se_falso
        String resultado = salario > 5000 ? "Vou doar para o DevDojo" : "Ainda não tenho condições";

        // Como a condição (6000 > 5000) é verdadeira, a primeira opção é atribuída à variável
        System.out.println(resultado); // Imprime: Vou doar para o DevDojo
    }
}
```

Nesse exemplo, o uso do ternário evita a criação de um bloco `if-else` inteiro de múltiplas linhas apenas para decidir qual `String` associar à variável `resultado`.

## Operadores de atribuição #atribuicao

Os **operadores de atribuição** são utilizados para associar e guardar um valor dentro do espaço de memória de uma variável, sendo o **sinal de igual (`=`) o operador mais básico**. Além dele, a linguagem oferece os operadores de atribuição compostos, que foram criados com o objetivo de **simplificar e economizar a escrita do código**.

Esses operadores combinam operadores aritméticos com o sinal de atribuição, resultando em **`+=`, `-=`, `*=`, `/=` e `%=`**. Na prática, utilizar uma expressão como `bonus += 1000` é exatamente o mesmo que escrever `bonus = bonus + 1000`, servindo apenas como uma forma de aplicar uma operação matemática sobre o valor que a variável já possui e atribuir o novo resultado a ela mesma.

Nesse mesmo contexto, existem também os **operadores unários de incremento (`++`) e decremento (`--`)**, que servem como uma forma ainda mais abreviada para adicionar ou subtrair o valor `1` de uma variável. No entanto, é fundamental **prestar atenção na posição desses operadores unários**:

*   **Antes da variável (ex: `++contador`)**: a variável é **incrementada primeiro** e o novo valor é utilizado na execução da instrução daquela linha.
*   **Depois da variável (ex: `contador++`)**: o programa **executa a instrução da linha primeiro utilizando o valor original** da variável, e somente depois realiza o incremento na memória.

**Exemplo de código**

Aqui está um exemplo prático em Java demonstrando o uso dos operadores de atribuição e de incremento/decremento discutidos:

```Java
public class OperadoresAtribuicao {
    public static void main(String[] args) {

        // Atribuição básica
        int bonus = 1800;

        // Operadores de atribuição compostos
        bonus += 1000; // Exatamente o mesmo que: bonus = bonus + 1000
        System.out.println("Bônus após soma: " + bonus); // Imprime 2800

        bonus *= 2;    // Exatamente o mesmo que: bonus = bonus * 2
        System.out.println("Bônus após multiplicação: " + bonus); // Imprime 5600

        bonus %= 2;    // Pega o resto da divisão por 2 e atribui à variável
        System.out.println("Resto da divisão: " + bonus); // Imprime 0 (número par)


        // Operadores unários de incremento e decremento
        int contador = 0;
        contador++; // Forma abreviada de adicionar 1 (contador agora é 1)

        // Diferença na ordem de execução (Pré x Pós incremento)
        int contador2 = 0;

        // Pós-incremento: Imprime primeiro o valor original (0) e SÓ DEPOIS soma 1 na memória
        System.out.println("Pós-incremento: " + contador2++);

        // Pré-incremento: O valor de contador2 agora é 1.
        // Aqui ele SOMA 1 PRIMEIRO (vira 2) e depois imprime o novo valor.
        System.out.println("Pré-incremento: " + ++contador2);
    }
}
```

Neste código, fica claro como os operadores compostos (`+=`, `*=`, `%=`) ajudam a encurtar a escrita ao realizar uma operação matemática sobre a própria variável. Também é possível notar o comportamento da ordem de execução dos operadores unários: ao colocar o `++` depois da variável (`contador2++`), a instrução da linha é executada primeiro com o valor original e, ao colocar o `++` antes (`++contador2`), o incremento acontece primeiro e o novo valor já é utilizado na mesma linha.
## **Condicionais com if, else if, else** #condicionais1 

As estruturas condicionais na linguagem Java são utilizadas para criar tomadas de decisões na aplicação, permitindo que o programa execute blocos de código diferentes dependendo de uma condição ser avaliada como verdadeira (true) ou falsa (false).  

`if (Se):` É a estrutura principal e a primeira verificação feita pelo sistema. O bloco de código que está dentro das chaves {} do if só será executado caso a condição declarada dentro dos parênteses seja verdadeira.  

`else if (Senão se):` Utilizado para adicionar novas condições subsequentes caso o primeiro if seja falso. Se a primeira condição falhar, o sistema pula para verificar a condição estipulada no else if. Você pode encadear quantos else if forem necessários para cobrir todas as suas validações.

`else (Senão):` Funciona como a opção de escape padrão da sua validação. O bloco de código do else só será executado quando absolutamente todas as verificações anteriores (o if e os eventuais else if) resultarem em falso. Justamente por ser a resposta padrão quando tudo falha, o else não possui nenhuma condição própria entre parênteses.

Exemplo prático de código: 

No cenário abaixo, a aplicação utiliza a idade de um usuário para decidir de forma dinâmica se ele deve ser classificado como criança, adolescente ou adulto.

```Java
byte idade \= 15;

// 1\. Primeira verificação: testa se a idade é menor ou igual a 10  
if (idade \<= 10\) {  
    System.out.println("Criança");

// 2\. Segunda verificação: como a primeira falhou, testa se é menor ou igual a 17  
} else if (idade \<= 17\) {  
    System.out.println("Adolescente");

// 3\. Resposta padrão: se todas as condições acima forem falsas, executa o else  
} else {  
    System.out.println("Adulto");  
}  
```
(Neste exemplo, a primeira condição falha pois 15 não é menor ou igual a 10\. O sistema então passa para o else if, que retorna verdadeiro pois 15 é menor que 17\. A palavra "Adolescente" é exibida e a execução ignora o restante do bloco)

## Laços: while, do-while e for #lacos1

As estruturas de repetição (ou laços) são fundamentais quando queremos que o programa execute um bloco de código múltiplas vezes de forma contínua. O Java possui três estruturas clássicas para isso:

- **`while` (Enquanto):** Avalia uma condição booleana **antes** de executar o bloco de código. O laço continuará repetindo as instruções enquanto essa condição for verdadeira. É crucial garantir que o estado da variável de controle seja alterado dentro do laço (geralmente por meio de um incremento ou decremento), caso contrário, o programa entrará em um loop infinito, rodando para sempre.
- **`do-while` (Faça-Enquanto):** A principal diferença em relação ao `while` é que a estrutura `do-while` executa o bloco de código primeiro e só avalia a condição no final. Isso garante que as instruções dentro do laço sejam executadas **pelo menos uma vez**, mesmo que a condição já seja inicialmente falsa.
- **`for` (Para):** É a estrutura mais utilizada para contagens e iterações sobre coleções, pois agrupa todo o controle do laço em uma única linha. Sua sintaxe é dividida em três partes separadas por ponto e vírgula (`;`):
    1. **Inicialização:** Declaração e inicialização da variável de controle (ex: `int i = 0`).
    2. **Condição:** A expressão que define até quando o laço deve continuar rodando (ex: `i < 10`).
    3. **Alteração de status:** O incremento ou decremento da variável ao fim de cada iteração (ex: `i++`).

**Exemplo de código:**

Abaixo, um exemplo prático demonstrando o funcionamento de cada um dos laços para imprimir uma contagem de 1 a 3:

```Java
public class LacosDeRepeticao {
    public static void main(String[] args) {

        // 1. Exemplo com WHILE
        System.out.println("Usando while:");
        int contador1 = 1;
        while (contador1 <= 3) { // Condição checada no início
            System.out.println("Contagem: " + contador1);
            contador1++; // Se esquecermos isso, o laço será infinito
        }

        // 2. Exemplo com DO-WHILE
        System.out.println("\nUsando do-while:");
        int contador2 = 1;
        do {
            System.out.println("Contagem: " + contador2);
            contador2++;
        } while (contador2 <= 3); // Condição checada no final. Executa pelo menos 1 vez.

        // 3. Exemplo com FOR
        System.out.println("\nUsando for:");
        // ( inicialização ; condição ; incremento )
        for (int i = 1; i <= 3; i++) {
            System.out.println("Contagem: " + i);
        }
    }
}
```

Nesse código, todos os três laços farão exatamente a mesma coisa (imprimir de 1 a 3), mas com estruturas de controle diferentes. O `for` costuma ser o favorito para quando se sabe exatamente o número de iterações, enquanto o `while` e o `do-while` brilham em situações onde a repetição depende de fatores externos ou dinâmicos que podem não ter um número fixo de ciclos.
## Controle de laços #lacos2
O controle de fluxo em laços de repetição pode ser manipulado e otimizado através de duas palavras-chave fundamentais: **`break`** e **`continue`**. Elas permitem alterar o comportamento padrão dos loops (como `for`, `while` e `do-while`) com base em condições específicas.

- **`break`:** Tem a função de **parar a execução do laço e sair dele imediatamente**. Quando o programa encontra um `break`, ele quebra o loop inteiro (ou um bloco `switch`) e pula para a próxima linha de código que estiver fora da estrutura de repetição. É extremamente útil para economizar processamento, permitindo que você encerre um loop assim que atingir seu objetivo, sem precisar rodar as iterações restantes desnecessariamente. Vale ressaltar que o `break` não serve para sair de blocos `if`, ele sai do laço de repetição ou `switch` no qual aquele `if` está inserido.
- **`continue`:** Ao invés de parar totalmente o loop, ele **ignora todo o código que estiver abaixo dele e pula direto para a próxima iteração**. Quando o `continue` é executado, o programa volta imediatamente para o início do laço (para realizar o incremento e a avaliação da condição) e continua rodando a partir do próximo ciclo. Isso é muito útil para pular lógicas de processamento para valores que não atendem aos critérios desejados.

**Exemplo de código:**

Abaixo, um exemplo demonstrando o uso prático de ambos em uma contagem de 1 a 10:

```Java
public class ControleDeLacos {
    public static void main(String[] args) {

        System.out.println("Iniciando o laço for:");

        for (int i = 1; i <= 10; i++) {

            // Se o número for 4, ignora o código abaixo e VAI PARA A PRÓXIMA iteração (5)
            if (i == 4) {
                System.out.println("Encontrou o 4: Pulando iteração com 'continue'.");
                continue;
            }

            // Se o número for 8, ENCERRA o laço completamente
            if (i == 8) {
                System.out.println("Encontrou o 8: Saindo do laço com 'break'.");
                break;
            }

            System.out.println("Contagem: " + i);
        }

        System.out.println("Laço finalizado.");
    }
}
```

No código acima, o número 4 não será impresso na contagem normal porque o `continue` força o laço a ignorar o print final e voltar ao início da estrutura. Já quando o valor chegar a 8, o `break` é acionado e o laço é encerrado por completo, fazendo com que o laço termine antes do tempo e os números 8, 9 e 10 nunca sejam impressos.
## **Condicionais com switch, case, break, default** #condicionais2 

A estrutura condicional switch é uma alternativa ao if/else que trabalha de forma um pouco diferente: em vez de avaliar lógicas complexas de verdadeiro ou falso, ela verifica diretamente o conteúdo de uma variável e o compara com diversas opções pré-definidas. É uma estrutura mais simples, mas extremamente efetiva para criar menus ou algoritmos de múltiplas escolhas.  
Resumo de como cada componente funciona:  
switch: Inicia a estrutura de decisão e recebe, entre parênteses, a variável exata cujo valor será analisado.  
case (Caso): Representa cada valor específico que a variável pode assumir. Caso o valor armazenado na variável seja igual ao estipulado no case, o bloco de código logo abaixo dele é executado.  
break (Parar): É uma palavra-chave fundamental utilizada no final do bloco de cada case para interromper e finalizar a execução da estrutura condicional. Se você omitir o break, a aplicação continuará executando os códigos de todos os blocos case subsequentes em cascata, mesmo que a condição deles não tenha sido a escolhida.  
default (Padrão): Funciona como uma trava de segurança da sua aplicação, sendo equivalente ao else. Ele será executado automaticamente caso o valor da variável analisada não corresponda a absolutamente nenhuma das opções definidas nos case anteriores. Diferente dos blocos case, o valor default não precisa ser encerrado com a palavra break.  
Exemplo prático de código: No cenário abaixo, a aplicação simula o menu de um banco baseado em um número de opção escolhido pelo usuário.  

```Java
byte opcaoBanco = 2; // Variável que armazenará a escolha do usuário

// 1\. O switch recebe a variável para avaliar o seu conteúdo  
switch (opcaoBanco) {  
      
    // 2\. Compara: a variável tem o valor 1?  
    case 1:  
        System.out.println("Ver fatura do cartão");  
        break; // Paralisa a execução caso entre neste bloco  
          
    // 3\. Compara: a variável tem o valor 2? (Neste exemplo, é o que será executado)  
    case 2:  
        System.out.println("Saldo conta corrente");  
        break; // Paralisa a execução para não vazar para os blocos de baixo  
          
    // 4\. Compara: a variável tem o valor 3?  
    case 3:  
        System.out.println("Poupança");  
        break;  
          
    // 5\. Segurança: se a variável não tiver os valores 1, 2 ou 3, cai no default  
    default:  
        System.out.println("Nenhuma opção válida selecionada");  
}
```
## **Arrays (Declaração, índices e iteração)** #arrays 

Os `Arrays` na linguagem Java funcionam como "super variáveis" capazes de armazenar múltiplos valores de um mesmo tipo dentro de uma única estrutura. Eles são ideais para criar listas, como uma lista de compras, lista de usuários ou lista de números.  

Declaração: Para criar um array, você deve informar o tipo de dado seguido por colchetes vazios `[ ]` . 

Os valores atribuídos a essa variável devem ser colocados dentro de chaves `{}` e separados por vírgula. 

Você pode criar arrays de diversos tipos, como textos `(String[ ])`, números inteiros `(int[ ])`, decimais `(double[ ])` ou lógicos `(boolean[ ])`, mas o array não aceita a mistura de tipos diferentes (um array de String não aceitará a inserção de um número inteiro, por exemplo).  

**Índices:** Cada item guardado dentro do array ocupa uma posição específica chamada de índice, e a contagem desses índices sempre começa no zero (0). 

Portanto, o primeiro item da lista estará posicionado no índice 0, o segundo no índice 1, e assim por diante. 

Para buscar um valor específico, você informa o nome do array seguido do índice desejado entre colchetes (ex:`nomeArray['nome']`).

**Iteração e Exibição:** Se você tentar imprimir o array inteiro diretamente (ex: `System.out.println(listaDeCompras))`, o sistema não conseguirá ler os itens corretamente.

Para exibir a lista toda, você pode usar a classe `Arrays.toString()` para converter o array em texto. Para iterar (percorrer item por item), você pode utilizar estruturas de repetição como o for ou o `while`, aproveitando a propriedade `.length`, que retorna o tamanho total da lista para saber até quando o loop deve continuar rodando.

Exemplo prático de código:

```Java  
// DECLARAÇÃO: Criando um array de Strings com 3 itens  
String[ ] listaDeCompras = {"Banana", "Carne", "Ovos"};

// ÍNDICES: Buscando e imprimindo um item específico (o primeiro item fica no índice 0\)  
System.out.println(listaDeCompras); // Resultado: Banana  
System.out.println(listaDeCompras[9]); // Resultado: Carne

// ITERAÇÃO: Usando o loop 'for' e o '.length' para percorrer e imprimir todos os itens  
for (int indice = 0; indice < listaDeCompras.length; indice++) {  
    System.out.println(listaDeCompras[indice]);  
}

// EXIBIÇÃO DIRETA: Exibindo o array completo de uma vez convertendo para String  
// (Requer a importação de java.util.Arrays)  
System.out.println(Arrays.toString(listaDeCompras));   
// Resultado: \[Banana, Carne, Ovos\]  
```

## Foreach #foreach

O **`foreach`** é uma versão simplificada do laço `for`, criada especificamente para iterar sobre arrays (e coleções) de forma mais limpa, sem a necessidade de calcular o tamanho do array ou de gerenciar o incremento de índices manualmente.

**Sintaxe e Funcionamento:** Para utilizá-lo, você deve declarar uma variável local de referência que seja **exatamente do mesmo tipo** dos dados contidos no array, seguida por dois pontos (`:`) e o nome do array que será percorrido. Por debaixo dos panos, a cada iteração do laço, essa variável de referência apontará automaticamente para o próximo valor do array (começando da primeira posição até a última).

**Limitação Principal:** A principal diferença do `foreach` é que ele **não fornece acesso ao índice** da iteração atual. Portanto, se a sua regra de negócio exigir que você saiba em qual posição exata o elemento está, ou se você precisar fazer manipulações baseadas nesse índice, o ideal é utilizar o laço `for` tradicional indexado.

**Arrays Multidimensionais:** O `foreach` também funciona perfeitamente com arrays multidimensionais. A diferença é que a variável do primeiro laço representará um array (ex: `int[] arrayBase`), e você precisará de um segundo `foreach` aninhado para acessar os valores finais desse array base.

**Exemplo de código:**

Abaixo, um exemplo de como imprimir todos os valores de um array usando o `foreach`:

```Java
public class LacoForeach {
    public static void main(String[] args) {

        // Inicializando um array de inteiros
        int[] numeros = {5, 4, 3, 2, 1};

        // Sintaxe: for (Tipo variavelLocal : nomeDoArray)
        for (int num : numeros) {
            // A variável 'num' assumirá os valores 5, 4, 3, 2 e 1 sequencialmente
            System.out.println("Valor: " + num);
        }
    }
}
```

## **Multidimensionais (Inicialização e Foreach)** #multidimencionais
Arrays multidimensionais no Java são, essencialmente, **arrays que guardam referências para outros arrays**. O array principal (base) não guarda os valores finais diretamente, mas sim os endereços de memória dos arrays secundários. Isso traz a vantagem de criar estruturas flexíveis, onde cada "linha" (o array referenciado) pode ter um tamanho diferente da outra.

**Inicialização:** Ao criar um array multidimensional instanciando com a palavra `new`, você é **obrigado a definir o tamanho apenas da primeira dimensão**, podendo deixar o tamanho das dimensões seguintes em branco para serem inicializadas depois com tamanhos diferentes. Outra forma muito comum é a **inicialização direta**, onde você agrupa os valores utilizando blocos de chaves aninhadas (`{ }`) no momento da criação, e o compilador calcula os tamanhos automaticamente.

**Foreach com Arrays Multidimensionais:** Para iterar utilizando o `foreach`, você precisará de dois laços aninhados. O detalhe fundamental aqui é que **a variável de referência do primeiro `foreach` deve ser do tipo array**, pois é exatamente isso que cada posição do array base guarda. Somente no segundo `foreach` (o laço mais interno) é que você criará uma variável do tipo primitivo (ou objeto) para ler os valores finais de cada array.

**Exemplo de código e representação visual:**

```
public class ArrayMultidimensional {
    public static void main(String[] args) {

        // Inicialização direta: um array base com 3 posições que guardam arrays de tamanhos diferentes
        int[][] arrayMulti = {
            {1, 2},             // Posição 0 do array base guarda um array de tamanho 2
            {3, 4, 5},          // Posição 1 do array base guarda um array de tamanho 3
            {6, 7, 8, 9, 10}    // Posição 2 do array base guarda um array de tamanho 5
        };
        // Referência visual em memória:
        //  --->
        // --->
        // --->


        // Lendo com laço Foreach

        // 1º Laço: O tipo da variável precisa ser um array (ex: int[])
        for (int[] arrayBase : arrayMulti) {

            // 2º Laço: Iteramos sobre o array extraído na linha de cima para obter os valores
            for (int valor : arrayBase) {
                System.out.print(valor + " ");
            }
            System.out.println(); // Pula linha ao final de cada array interno
        }
    }
}
```

## **POO - Programação Orientada a Objetos com JAVA**
### Introdução a Classes, Objetos e Coesão

A transição para a **Programação Orientada a Objetos (POO)** marca uma mudança fundamental: em vez de usarmos variáveis primitivas soltas na memória (como um `int idade` e uma `String nome` separados e sem vínculo), passamos a agrupar esses dados para representar entidades do mundo real no mundo computacional.

Para entender essa estrutura, precisamos dividir o conceito em três pilares principais: Classes, Objetos e Coesão.

#### 1. Classes e Objetos

- **Classe:** É como se fosse um _template_, um molde ou uma planta baixa que define quais características (atributos) e comportamentos (métodos) uma entidade terá. Por exemplo, uma classe `Carro` definirá que todo carro deve ter os atributos `nome`, `modelo` e `ano`.
- **Objeto (Instância):** É a materialização dessa classe na memória. Para criar (instanciar) um objeto, utilizamos a palavra-chave `new`. Ao fazer isso, o Java aloca um espaço na memória para guardar os atributos definidos pela classe.
- **Variável de Referência:** É a variável que criamos para "apontar" e controlar o objeto criado na memória. É como se a variável de referência fosse um controle remoto e o objeto fosse a televisão. Utilizamos o sinal de ponto (`.`) para acessar e modificar os atributos do objeto através de sua referência (ex: `estudante.nome = "Gohan"`).

#### 2. Coesão

A **coesão** é um dos conceitos de design de código mais importantes na orientação a objetos e está diretamente relacionada ao **propósito de existência de uma classe**.

- **Alta Coesão (Bom):** Significa que a classe tem um propósito único, bem definido e específico. Por exemplo, a classe `Estudante` deve possuir apenas os atributos e métodos que dizem respeito a um estudante.
- **Baixa Coesão (Ruim):** Ocorre quando uma classe faz mais coisas do que deveria, misturando responsabilidades. Um exemplo clássico de baixa coesão seria colocar os atributos de um `Professor` (como `nomeProfessor` e `idadeProfessor`) dentro da classe `Estudante`. Qualquer alteração nas regras de professores afetaria o código dos estudantes, gerando um efeito cascata de problemas de manutenção. Outro exemplo de baixa coesão é inserir o método de execução `main` dentro da própria classe de domínio (molde), misturando a representação do objeto com a execução do sistema. O correto é ter uma classe separada apenas para testes/execução.

**Exemplo de código:**

Abaixo, vemos a aplicação de **alta coesão**, separando perfeitamente a classe que serve de molde (domínio) da classe que executa o código (teste):

```Java
// Classe de Domínio com ALTA COESÃO (Representa apenas o conceito de Estudante)
public class Estudante {
    public String nome;
    public int idade;
    public char sexo;
}
```

```Java
// Classe focada apenas em executar e testar o código
public class EstudanteTeste {
    public static void main(String[] args) {

        // Criando a variável de referência e instanciando o objeto com 'new'
        Estudante estudante1 = new Estudante();

        // Acessando os atributos do objeto através do controle remoto (referência)
        estudante1.nome = "Luffy";
        estudante1.idade = 18;
        estudante1.sexo = 'M';

        System.out.println("Nome: " + estudante1.nome);
    }
}
```


#### Referência de objetos
No Java, quando instanciamos um objeto com a palavra `new`, o que guardamos na variável não são os dados do objeto em si, mas sim o **endereço de memória** onde ele foi criado. Essa variável é chamada de **variável de referência**. Uma analogia clássica é pensar na variável de referência como um **controle remoto** e no objeto alocado na memória como a **televisão**.

O comportamento mais importante desse conceito é que **múltiplas variáveis de referência podem apontar para o mesmíssimo objeto na memória**.

Se você atribuir o valor de uma variável de referência a outra (por exemplo, `carro1 = carro2;`), a variável `carro1` deixa de fazer referência ao seu objeto original. Esse objeto original fica "perdido" na memória e, se nenhuma outra variável estiver apontando para ele, será eventualmente limpo pelo _Garbage Collector_ do Java. A partir desse momento, tanto `carro1` quanto `carro2` passam a controlar o mesmo objeto. Consequentemente, qualquer alteração feita nos dados do objeto usando o `carro1` será imediatamente visível ao acessar pelo `carro2`, pois ambos manipulam o exato mesmo espaço de memória.

**Exemplo de código e representação visual:**

```Java
public class ReferenciaObjeto {
    public static void main(String[] args) {

        // Criamos dois objetos diferentes na memória
        Carro carro1 = new Carro();
        carro1.nome = "Fusca";

        Carro carro2 = new Carro();
        carro2.nome = "Mustang";

        // Representação em memória neste momento:
        // carro1 (Controle 1) ---> [ Objeto Memória: Fusca ]
        // carro2 (Controle 2) ---> [ Objeto Memória: Mustang ]

        // Fazemos carro1 apontar para o mesmo objeto que carro2
        carro1 = carro2;

        // O [ Objeto Memória: Fusca ] perdeu sua única referência e está perdido.
        // Nova representação em memória:
        // carro1 ---> \
        //              ---> [ Objeto Memória: Mustang ]
        // carro2 ---> /

        // Se alterarmos o nome do objeto usando o controle remoto carro1...
        carro1.nome = "Ferrari";

        // ...a alteração afeta o objeto real.
        // Logo, ao ler com o carro2, vemos a mudança:
        System.out.println(carro2.nome); // Imprime: Ferrari
    }
}
```

### Métodos

Os **métodos** representam o comportamento (as ações) que os objetos de uma classe podem executar. A sintaxe básica de um método é composta por um modificador de acesso, um tipo de retorno (ou `void` caso não retorne nada), o nome do método (seguindo a convenção _camelCase_) e parênteses para os parâmetros. Para executar um método, você utiliza a variável de referência do objeto seguida de um ponto e o nome do método (ex: `calculadora.soma()`). Ao ser chamado, o fluxo do programa entra no método, executa suas instruções e depois retorna para a linha onde foi chamado.

**Parâmetros (Tipos primitivos e referência)** Os parâmetros são variáveis locais declaradas dentro dos parênteses do método, servindo como um "contrato" que exige que quem chama o método forneça os valores (argumentos) necessários para sua execução. Existe uma diferença fundamental em como o Java lida com os tipos de dados passados:

- **Tipos Primitivos (Passagem por Valor):** Quando você passa um tipo primitivo (como `int`, `double`), o Java cria uma **cópia exata** desse valor na memória para ser usada pelo método. Qualquer alteração feita nessa variável local dentro do método **não afetará** a variável original de quem chamou o método.
- **Tipo Referência (Passagem por Referência):** Quando você passa um objeto, você está passando uma **cópia da referência** (o endereço de memória). Isso significa que a variável local do método apontará exatamente para o **mesmo objeto na memória** que a variável original. O grande perigo aqui é que **qualquer alteração nos atributos do objeto dentro do método mudará o estado do objeto original** no sistema inteiro.

**Retorno de métodos** Se a assinatura do método tiver um tipo de dados ao invés da palavra `void`, o método é obrigado a devolver um valor compatível para quem o chamou usando a palavra-chave **`return`**. O valor retornado pode ser impresso diretamente ou guardado em uma variável local para uso posterior. O `return` também atua como uma parada imediata do método: assim que o Java lê essa linha, ele sai do método e volta para a execução original, ignorando qualquer código que estiver abaixo. Curiosamente, até mesmo métodos `void` podem usar um `return;` vazio apenas com o intuito de interromper e sair do método precocemente (como uma espécie de `break` de métodos).

**Referência `this`** A palavra reservada **`this`** faz referência direta ao **objeto atual que está executando o método** na memória. Como o método está dentro do espaço do objeto, o `this` permite acessar todos os atributos daquela instância específica. Ele é extremamente utilizado para diferenciar um atributo da classe de uma variável local ou parâmetro que tenha exatamente o mesmo nome, garantindo que o valor correto seja atribuído ao lugar certo.

**Varargs (Variable Arguments)** O `varargs` é uma sintaxe especial (`...` após o tipo do parâmetro) que permite passar uma quantidade indefinida de argumentos do mesmo tipo para um método, separando-os por vírgula no momento da chamada (ex: `soma(1, 2, 3, 4, 5)`). Por debaixo dos panos, o **Java transforma automaticamente todos esses argumentos em um Array** para ser utilizado dentro do método. Existem duas regras rígidas para utilizar o varargs:

1. Se o método receber múltiplos parâmetros diferentes, **o varargs deve ser obrigatoriamente o último parâmetro** declarado na assinatura.
2. Você só pode ter **um único varargs** por método, caso contrário, o compilador não saberá onde os valores de um terminam e onde começam os do outro.

Aqui está um exemplo prático em Java que reúne todos os conceitos de métodos (parâmetros, retorno, referência `this` e varargs) explicados anteriormente:

```Java
// Classe de domínio
public class Estudante {
    public String nome;
    public int idade;

    // 1. Método com Referência 'this' e sem retorno (void)
    public void imprimirDados() {
        // O 'this' aponta para o objeto atual que chamou o método
        System.out.println("Nome: " + this.nome);
        System.out.println("Idade: " + this.idade);
    }

    // 2. Método com Retorno (boolean)
    public boolean isMaiorDeIdade() {
        if (this.idade >= 18) {
            return true; // Retorna um valor e sai do método
        }
        return false;
    }

    // 3. Método com Varargs (recebe múltiplos valores como um array)
    // O varargs (...) deve ser sempre o último parâmetro da assinatura
    public void calcularMedia(String disciplina, double... notas) {
        double soma = 0;
        for (double nota : notas) {
            soma += nota;
        }
        System.out.println("Média em " + disciplina + ": " + (soma / notas.length));
    }
}
```

``` Java
// Classe de execução/teste
public class EstudanteTeste {

    // 4. Parâmetro de Tipo Primitivo (Passagem por Valor)
    public static void alterarIdade(int idadeCopia) {
        idadeCopia = 99; // Altera apenas a cópia local, não afeta a variável original
    }

    // 5. Parâmetro de Tipo Referência (Passagem por Referência)
    public static void alterarNome(Estudante estudanteRef) {
        estudanteRef.nome = "Gohan"; // Altera o objeto real na memória!
    }

    public static void main(String[] args) {
        Estudante estudante1 = new Estudante();
        estudante1.nome = "Goku";
        estudante1.idade = 35;

        // Executando método que usa o 'this'
        System.out.println("--- Dados Iniciais ---");
        estudante1.imprimirDados();

        // Executando método com retorno
        boolean maior = estudante1.isMaiorDeIdade();
        System.out.println("É maior de idade? " + maior);

        // Executando método com Varargs (passando múltiplos double separados por vírgula)
        estudante1.calcularMedia("Matemática", 8.5, 9.0, 7.5, 10.0);

        System.out.println("\n--- Testando Passagem de Parâmetros ---");

        // Testando Tipo Primitivo: a variável original não muda
        alterarIdade(estudante1.idade);
        System.out.println("Idade após método primitivo: " + estudante1.idade); // Imprime 35

        // Testando Tipo Referência: o objeto original é alterado
        alterarNome(estudante1);
        System.out.println("Nome após método referência: " + estudante1.nome); // Imprime Gohan
    }
}
```

**Como os conceitos se aplicam no código:**

- **Retorno de Métodos:** O método `isMaiorDeIdade` possui a palavra `boolean` na assinatura, obrigando-o a devolver um valor verdadeiro ou falso utilizando a palavra-chave `return`.
- **Referência `this`:** Dentro de `imprimirDados`, o `this` é usado para acessar os atributos `nome` e `idade` do exato objeto `Estudante` que ativou o método.
- **Varargs:** No método `calcularMedia`, o parâmetro `double... notas` permite receber uma quantidade indefinida de notas separadas por vírgula. Como existe um outro parâmetro (`disciplina`), o varargs foi posicionado obrigatoriamente no final da assinatura.
- **Tipos Primitivos:** O método `alterarIdade` recebe um `int`. O Java cria uma cópia exata do valor em memória, então alterar para 99 dentro do método não surte nenhum efeito no objeto original.
- **Tipos de Referência:** O método `alterarNome` recebe o objeto `Estudante`. Como o endereço de memória foi passado, a alteração para "Gohan" modifica definitivamente o estado do objeto original no sistema inteiro.
### Modificadores de acesso

Os **Modificadores de Acesso (`private`, `get` e `set`)** são ferramentas fundamentais para garantir um baixo acoplamento e a proteção dos dados de uma classe. Ao utilizar o modificador **`private`** em um atributo, você restringe o acesso a ele, tornando-o invisível e inacessível para outras classes. Para permitir que o mundo externo interaja com esses dados de forma controlada, a convenção é criar métodos **`public`**: os **`setters`** (que recebem um parâmetro para atribuir valor ao atributo em memória) e os **`getters`** (que não recebem parâmetros e apenas retornam o valor que está na memória).

#### **Sobrecarga de Métodos** 
Acontece quando você cria **múltiplos métodos com o exato mesmo nome dentro de uma classe, mas com a quantidade ou o tipo dos parâmetros diferentes**. O tipo de retorno e o modificador de acesso não influenciam na sobrecarga; o que o Java avalia para não gerar ambiguidade é a assinatura dos parâmetros no momento em que o método é chamado.

### **Construtores** 
São responsáveis por inicializar e construir o objeto na memória e possuem uma sintaxe específica: **eles não possuem tipo de retorno (nem mesmo a palavra `void`) e devem ter o nome exato da classe**. Se você não escrever nenhum construtor, o compilador do Java criará um construtor padrão sem argumentos para você. A **Sobrecarga de construtores** segue a mesma lógica da sobrecarga de métodos, permitindo instanciar objetos passando diferentes conjuntos de dados. Para evitar repetição de código, um construtor pode chamar outro construtor da mesma classe utilizando a palavra-chave **`this()`**, mas existe uma regra rígida: **o `this()` deve ser obrigatoriamente a primeira linha executável do construtor**.

### **Blocos de Inicialização** 

São trechos de código executados durante o ciclo de vida do objeto ou da classe:

- **Bloco de Inicialização de Instância:** É criado abrindo e fechando chaves `{ }` diretamente no corpo da classe. Ele é **executado todas as vezes que um novo objeto é criado**, ocorrendo estritamente antes da execução do construtor.
- **Bloco de Inicialização Estático:** É criado adicionando a palavra `static` antes das chaves `static { }`. Ele é **executado apenas uma única vez, no exato momento em que a JVM carrega a classe na memória**, acontecendo antes mesmo de qualquer espaço de objeto ser alocado ou dos construtores serem chamados.

### **Modificador `static`**

O **Modificador `static`** muda a forma como atributos e métodos pertencem à estrutura do Java:

- **Atributos Estáticos:** Ao colocar `static` em uma variável, ela **deixa de pertencer à instância (objeto) e passa a pertencer à classe**. Isso significa que todos os objetos criados a partir dessa classe compartilharão o mesmo espaço em memória para aquele valor. Se você alterar o valor através da classe, todos os objetos refletirão essa mudança.
- **Métodos Estáticos:** São métodos que podem ser chamados diretamente pelo nome da classe, sem precisar de um objeto instanciado. A regra fundamental aqui é: **um método estático nunca pode acessar atributos ou métodos de instância (não-estáticos) e não pode usar a palavra-chave `this`**. Isso ocorre porque o método estático pode ser executado antes mesmo de qualquer objeto existir na memória.

**Exemplo de Código:**

``` Java
public class Anime {

    // Atributo estático: pertence à classe e é compartilhado
    private static String estudioPadrao;

    // Atributos de instância: protegidos pelo modificador private
    private String nome;
    private int episodios;

    // Bloco de inicialização estático: roda 1x quando a JVM carrega a classe
    static {
        estudioPadrao = "Toei Animation";
        System.out.println("Bloco estático inicializado.");
    }

    // Bloco de inicialização de instância: roda a cada 'new Anime()' antes do construtor
    {
        System.out.println("Bloco de instância: Preparando para alocar o anime.");
    }

    // Construtor 1
    public Anime(String nome) {
        this.nome = nome;
    }

    // Construtor 2: Sobrecarga de construtores
    public Anime(String nome, int episodios) {
        // Chamando o Construtor 1 (DEVE ser a primeira linha)
        this(nome);
        this.episodios = episodios;
    }

    // Método de instância
    public void exibirInfo() {
        System.out.println("Anime: " + this.nome + " | Estúdio: " + estudioPadrao);
    }

    // Sobrecarga de método
    public void exibirInfo(boolean detalhado) {
        if (detalhado) {
            System.out.println("Anime: " + this.nome + " | Eps: " + this.episodios + " | Estúdio: " + estudioPadrao);
        } else {
            exibirInfo();
        }
    }

    // Método Estático: Só pode acessar dados estáticos. O uso do 'this' é proibido aqui.
    public static void setEstudioPadrao(String novoEstudio) {
        estudioPadrao = novoEstudio;
    }

    // Métodos Getters e Setters para encapsulamento
    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }
}
```

### Associação

A **associação** no Java é o recurso utilizado para mapear os relacionamentos do mundo real para o código computacional, definindo como as classes interagem e se conectam, representando relações de "tem um" ou "pertence a" (ex: um jogador tem um time, ou um departamento tem pessoas).

Abaixo estão os pilares de como construir essas relações:

### Arrays com Objetos

Ao criarmos um array para tipos de referência (como um array da classe `Jogador`), o array não guarda os objetos diretamente. O que ele guarda em cada uma de suas posições são os **endereços de memória (referências)** que apontam para os objetos reais alocados na memória. É como se o array fosse um controle remoto com vários botões, onde cada botão aponta para uma televisão (objeto) diferente.

###  Associação Unidirecional

Acontece quando apenas um dos lados do relacionamento "conhece" o outro, limitando a navegação no código apenas a essa direção.

- **Muitos para um:** Ocorre quando vários objetos estão associados a um único objeto de outro tipo. Por exemplo, vários jogadores pertencem a um time, mas o time não lista seus jogadores. No código, a classe `Jogador` teria um atributo do tipo `Time`, permitindo acessar o time a partir do jogador, mas não o contrário.
- **Um para muitos:** É a relação inversa, onde um objeto contém múltiplos objetos de outro tipo. Por exemplo, uma classe `Escola` possui um array de objetos `Professor`, mas o `Professor` não possui referência para a `Escola` em que trabalha.

### Associação Bidirecional

Ocorre quando **ambas as classes envolvidas no relacionamento se conhecem e possuem referências mútuas**. Usando o mesmo exemplo, a classe `Jogador` terá um atributo `Time`, e a classe `Time` terá um array (ou lista) contendo os `Jogador`es que pertencem a ele. O grande cuidado na associação bidirecional é a **integridade dos dados em memória**: você como desenvolvedor precisa garantir que, ao atribuir um time a um jogador, você também insira esse jogador dentro do array pertencente àquele time, garantindo que ambos os lados apontem para as referências corretas.

---

**Exemplo de código (Associação Bidirecional envolvendo Arrays com Objetos):**

``` Java
// Classe Jogador
public class Jogador {
    private String nome;
    private Time time; // Relacionamento Muitos para Um

    public Jogador(String nome) {
        this.nome = nome;
    }

    public void imprimir() {
        System.out.println("Jogador: " + this.nome);
        if (this.time != null) {
            System.out.println("Time: " + this.time.getNome());
        }
    }

    public void setTime(Time time) {
        this.time = time;
    }
}
```

``` Java
// Classe Time
public class Time {
    private String nome;
    private Jogador[] jogadores; // Relacionamento Um para Muitos (Array com Objetos)

    public Time(String nome) {
        this.nome = nome;
    }

    public void imprimir() {
        System.out.println("Time: " + this.nome);
        if (this.jogadores != null) {
            for (Jogador jogador : jogadores) {
                System.out.println("- " + jogador.getNome());
            }
        }
    }

    public void setJogadores(Jogador[] jogadores) {
        this.jogadores = jogadores;
    }

    public String getNome() {
        return nome;
    }
}
```

``` Java
// Classe Executável (Teste)
public class AssociacaoTeste {
    public static void main(String[] args) {

        Jogador jogador1 = new Jogador("Pelé");
        Jogador jogador2 = new Jogador("Cafu");

        Time time = new Time("Seleção Brasileira");

        // Criando o Array de Objetos para passar para o time
        Jogador[] jogadores = {jogador1, jogador2};

        // --- Garantindo a integridade Bidirecional ---

        // 1. O Jogador agora conhece o Time
        jogador1.setTime(time);
        jogador2.setTime(time);

        // 2. O Time agora conhece os Jogadores
        time.setJogadores(jogadores);

        // Impressão
        System.out.println("--- Dados do Jogador ---");
        jogador1.imprimir(); // Imprime: Pelé e o time Seleção Brasileira

        System.out.println("\n--- Dados do Time ---");
        time.imprimir(); // Imprime: Seleção Brasileira e os jogadores Pelé e Cafu
    }
}
```

### Leitura de dados no console

A leitura de dados digitados pelo usuário no console em Java é feita utilizando a classe **`Scanner`**, que pertence ao pacote `java.util`.

Para capturar a entrada do teclado, você precisa instanciar um objeto dessa classe passando **`System.in`** como argumento no construtor.

A classe `Scanner` oferece diversos métodos úteis que já realizam a conversão da entrada do usuário para o tipo de dado desejado:

- **`nextLine()`:** Lê a linha inteira digitada pelo usuário, incluindo espaços em branco (ideal para textos e nomes compostos).
- **`next()`:** Lê apenas a primeira palavra digitada, parando a captura assim que encontra o primeiro espaço em branco.
- **Leitura de primitivos:** Existem métodos diretos como `nextInt()`, `nextBoolean()`, `nextDouble()`, entre outros, que capturam o valor e já o convertem automaticamente para o tipo numérico ou lógico correspondente.
- **Leitura de caractere (`char`):** O Java não possui um método direto como `nextChar()`. Portanto, para ler apenas um caractere, utiliza-se a combinação `next().charAt(0)`, que lê a primeira palavra digitada e extrai apenas a letra na posição zero.

**Exemplo de Código:**

Abaixo, um exemplo prático interagindo com o usuário para preencher um cadastro simples:

```
import java.util.Scanner; // Importação obrigatória da classe

public class LeituraDadosConsole {
    public static void main(String[] args) {

        // Instanciando o Scanner para ler a entrada do teclado
        Scanner entrada = new Scanner(System.in);

        System.out.println("Digite o seu nome completo:");
        // Lê toda a linha digitada
        String nome = entrada.nextLine();

        System.out.println("Digite a sua idade:");
        // Lê a entrada e converte automaticamente para int
        int idade = entrada.nextInt();

        System.out.println("Digite seu sexo (M ou F):");
        // Pega a primeira palavra e captura apenas o caractere da posição 0
        char sexo = entrada.next().charAt(0);

        System.out.println("\n--- Relatório Final ---");
        System.out.println("Nome: " + nome);
        System.out.println("Idade: " + idade);
        System.out.println("Sexo: " + sexo);
    }
}
```

### Herança

A **herança** é um dos recursos mais poderosos da Orientação a Objetos. Ela permite que uma classe (subclasse) herde as características (atributos) e os comportamentos (métodos) de outra classe (superclasse). A herança é utilizada para representar um relacionamento do tipo **"é um"**. Por exemplo, um `Funcionário` _é uma_ `Pessoa`, o que significa que, no código, a classe `Funcionario` estenderia (`extends`) a classe `Pessoa`, herdando tudo o que uma pessoa tem (como nome, CPF) e adicionando suas próprias características especializadas (como salário). É importante destacar que a herança cria um **forte acoplamento** entre as classes, devendo ser utilizada com cuidado, principalmente para estender funcionalidades ou viabilizar o polimorfismo.

O **uso do `super`** é a forma como a subclasse faz referência direta ao objeto da superclasse (a classe pai). Ele é extremamente útil na **sobrescrita de métodos**, permitindo que você aproveite e execute a lógica do método da classe pai (por exemplo, `super.imprimir()`) e depois complemente com a lógica específica da classe filha.

O **modificador `protected`** é um nível de acesso criado especialmente para facilitar o trabalho com herança. Quando um atributo ou método é declarado como `protected`, ele **fica diretamente acessível para todas as suas subclasses (independentemente de estarem em pacotes diferentes)**, além de permanecer visível para qualquer outra classe que esteja dentro do **mesmo pacote**.

Na **Herança com Construtores**, o Java impõe uma regra estrita: se a superclasse possui um construtor que exige argumentos, **todas as subclasses são obrigadas a chamar esse construtor** para garantir que o objeto "pai" seja criado corretamente. Essa chamada é feita através do `super(argumentos)` e **deve ser obrigatoriamente a primeira linha executável** do construtor da subclasse. Se não houver construtores customizados, o compilador do Java insere implicitamente uma chamada `super()` vazia.

A **Sequência de inicialização** torna-se mais complexa quando a herança está envolvida, ocorrendo na seguinte ordem estrita:

1. Bloco estático da **superclasse** (executado quando a JVM carrega a classe).
2. Bloco estático da **subclasse**.
3. Alocação de memória e inicialização com valores padrão para os atributos da **superclasse**.
4. Bloco de inicialização de instância (não-estático) da **superclasse**.
5. Construtor da **superclasse**.
6. Alocação de memória e inicialização com valores padrão para os atributos da **subclasse**.
7. Bloco de inicialização de instância (não-estático) da **subclasse**.
8. Construtor da **subclasse**.

**Exemplo de código:**

Abaixo, um código prático reunindo todos esses conceitos de Herança, `protected`, `super`, Construtores e Blocos de Inicialização:

``` Java
// --- CLASSE PAI (SUPERCLASSE) ---
public class Pessoa {
    // protected: visível para as subclasses e pacotes iguais
    protected String nome;

    // 1. Bloco Estático da Superclasse
    static {
        System.out.println("1. Bloco Estático de Pessoa");
    }

    // 4. Bloco de Instância da Superclasse
    {
        System.out.println("4. Bloco de Instância de Pessoa");
    }

    // 5. Construtor da Superclasse
    public Pessoa(String nome) {
        System.out.println("5. Construtor de Pessoa");
        this.nome = nome;
    }

    public void imprimir() {
        System.out.println("Nome da pessoa: " + this.nome);
    }
}
```

```Java
// --- CLASSE FILHA (SUBCLASSE) ---
// Uso da herança (extends)
public class Funcionario extends Pessoa {
    private double salario;

    // 2. Bloco Estático da Subclasse
    static {
        System.out.println("2. Bloco Estático de Funcionario");
    }

    // 7. Bloco de Instância da Subclasse
    {
        System.out.println("7. Bloco de Instância de Funcionario");
    }

    // 8. Construtor da Subclasse
    public Funcionario(String nome, double salario) {
        // Uso do super() para chamar o construtor da classe pai.
        // OBRIGATORIAMENTE DEVE SER A PRIMEIRA LINHA!
        super(nome);
        System.out.println("8. Construtor de Funcionario");
        this.salario = salario;
    }

    // Sobrescrita do método da superclasse
    @Override
    public void imprimir() {
        // O modificador protected nos permite acessar 'this.nome' diretamente
        // Mas podemos usar super.imprimir() para aproveitar o comportamento do pai
        super.imprimir();
        System.out.println("Salário do funcionário: " + this.salario);
    }
}
```

```Java
// --- CLASSE DE EXECUÇÃO ---
public class HerancaTeste {
    public static void main(String[] args) {
        System.out.println("--- Iniciando o Sistema ---");

        // Dispara toda a sequência de inicialização (1 a 8 descrita nos comentários)
        Funcionario func = new Funcionario("Luffy", 5000.0);

        System.out.println("\n--- Imprimindo Dados ---");
        // Chama o método sobrescrito, que primeiro chama a impressão do pai (super),
        // e depois imprime os dados específicos do filho.
        func.imprimir();
    }
}
```

### **Sobrescrita do método toString**

No Java, todas as classes são filhas da classe `Object`, e essa classe padrão fornece um método chamado `toString()`. Quando você tenta imprimir uma variável de referência de um objeto diretamente, o comportamento padrão desse método é retornar o nome do pacote, o nome da classe e uma representação do endereço de memória (hashcode). Para que a impressão do objeto seja legível para seres humanos e mostre os dados reais dos atributos, é necessário **sobrescrever** o método `toString()` dentro da sua classe, alterando o seu comportamento. Ao fazer a sobrescrita, você deve utilizar a anotação `@Override` para garantir a segurança da operação e seguir regras rígidas: o nome, a quantidade de parâmetros e o tipo de retorno devem ser os mesmos, e o modificador de acesso não pode ser mais restritivo do que o original (público).

```
public class Anime {
    private String nome;
    private int episodios;

    public Anime(String nome, int episodios) {
        this.nome = nome;
        this.episodios = episodios;
    }

    // Sobrescrita do método toString herdado de Object
    @Override
    public String toString() {
        return "Anime: " + this.nome + " | Episódios: " + this.episodios;
    }

    public static void main(String[] args) {
        Anime anime = new Anime("One Piece", 1000);
        // Agora imprimirá o texto formatado ao invés do endereço de memória
        System.out.println(anime);
    }
}
```

---

### **Modificador final (Tipos primitivos, tipos referência, classes e métodos)**

O modificador `final` é utilizado para definir constantes e limitar a herança ou alteração de comportamentos, atuando de formas diferentes dependendo de onde é aplicado:

- **Tipos Primitivos:** Quando aplicado a uma variável primitiva, ela se torna uma **constante**, o que significa que, uma vez que o valor é atribuído, ele nunca mais poderá ser alterado. A convenção de nomenclatura para constantes é usar letras maiúsculas separadas por underline (`_`) e, geralmente, elas vêm acompanhadas do modificador `static`.
- **Tipos de Referência:** Quando aplicado a um objeto (variável de referência), o modificador garante que a **referência de memória seja imutável**. Ou seja, você não pode reatribuir um novo objeto (usar `new` novamente) para essa variável, mas os dados internos (atributos) desse objeto ainda podem ser alterados.
- **Classes:** Uma classe marcada como `final` **não pode ser estendida** por nenhuma outra classe, bloqueando completamente a herança. A classe `String` do Java é um exemplo de classe final, garantindo que seu comportamento não seja modificado por terceiros.
- **Métodos:** Um método marcado como `final` em uma superclasse **não pode ser sobrescrito** por suas subclasses, garantindo que aquele comportamento específico seja mantido inalterado em toda a hierarquia.

```
// 1. Classe Final: Nenhuma classe pode dar 'extends' nela
public final class ConfiguracaoSistema {

    // 2. Tipo Primitivo Final (Constante): Valor imutável
    public static final int VELOCIDADE_MAXIMA = 250;

    // 3. Tipo Referência Final: A referência não muda, mas os dados internos sim
    public final Comprador compradorPadrao = new Comprador("William");

    // 4. Método Final: Não poderia ser sobrescrito se esta classe permitisse herança
    public final void exibirConfiguracao() {
        System.out.println("Velocidade: " + VELOCIDADE_MAXIMA);

        // Permitido: alterar dados internos do objeto final
        compradorPadrao.setNome("DevDojo");

        // PROIBIDO: compradorPadrao = new Comprador("Outro");
    }
}
```

---

### **Enumeração (Construtores, atributos, sobrescrita de métodos e buscas)**

As enumerações (`enum`) são um tipo especial de classe utilizadas para **forçar a escolha de valores dentro de uma quantidade limitada de opções**, trazendo extrema segurança de tipagem para o código.

- **Construtores e Atributos:** Uma enumeração pode ter atributos para guardar valores específicos (como um valor numérico para o banco de dados ou um nome formatado para relatórios). Para isso, é necessário criar um construtor, mas **o construtor de uma enumeração é sempre privado** e executado implicitamente pela própria enumeração no momento de sua criação.
- **Sobrescrita de Métodos:** Enums permitem a criação de métodos abstratos que **obrigam cada constante da enumeração a prover a sua própria implementação específica** (ex: um cálculo de desconto diferente para débito e crédito).
- **Buscas:** É possível criar métodos estáticos dentro do `enum` para buscar uma constante específica baseada em um de seus atributos. O Java também disponibiliza o método `values()` que retorna um array com todos os tipos da enumeração, facilitando a iteração para buscas.

```
public enum TipoPagamento {
    // Constantes chamando o construtor implicitamente
    DEBITO(1, "Cartão de Débito") {
        @Override
        public double calcularDesconto(double valor) {
            return valor * 0.10; // 10% de desconto
        }
    },
    CREDITO(2, "Cartão de Crédito") {
        @Override
        public double calcularDesconto(double valor) {
            return valor * 0.05; // 5% de desconto
        }
    };

    private final int id;
    private final String descricao;

    // Construtor é privado por padrão
    TipoPagamento(int id, String descricao) {
        this.id = id;
        this.descricao = descricao;
    }

    // Método abstrato forçando a implementação em cada constante
    public abstract double calcularDesconto(double valor);

    public int getId() { return id; }
    public String getDescricao() { return descricao; }

    // Método de busca customizado
    public static TipoPagamento buscarPorId(int id) {
        for (TipoPagamento tipo : values()) {
            if (tipo.getId() == id) {
                return tipo;
            }
        }
        return null;
    }
}
```

---

### **Classes Abstratas (Regras e métodos abstratos)**

Classes abstratas são criadas para atuar como **templates (moldes genéricos)** e possuem uma regra fundamental: **elas nunca podem ser instanciadas diretamente** (você não pode usar `new` nelas). Elas existem exclusivamente para ter suas funcionalidades estendidas por subclasses concretas. O verdadeiro poder dessas classes reside nos **métodos abstratos**. Um método abstrato é declarado sem corpo (sem chaves) e serve como um contrato: ele **obriga todas as subclasses concretas a proverem a implementação** (a lógica) daquele método. Uma classe abstrata pode conter métodos normais (com corpo) e métodos abstratos, mas uma classe concreta nunca pode ter um método abstrato. Além disso, uma classe nunca pode ser marcada como `abstract` e `final` ao mesmo tempo, pois seus propósitos são opostos.

```
// Classe abstrata: serve apenas como molde, não pode instanciar com 'new'
public abstract class Funcionario {
    protected String nome;
    protected double salario;

    public Funcionario(String nome, double salario) {
        this.nome = nome;
        this.salario = salario;
    }

    // Método abstrato: sem corpo. Força as filhas a implementarem
    public abstract void calcularBonus();

    // Método concreto: as filhas apenas herdam
    public void imprimir() {
        System.out.println("Nome: " + nome + " | Salário: " + salario);
    }
}

// Subclasse concreta
public class Desenvolvedor extends Funcionario {

    public Desenvolvedor(String nome, double salario) {
        super(nome, salario);
    }

    // Obrigatório prover o corpo do método abstrato
    @Override
    public void calcularBonus() {
        this.salario += this.salario * 0.10; // Bônus de 10%
    }
}
```

---

### **Interfaces (Múltiplas implementações, atributos e métodos estáticos)**

As interfaces funcionam como os contratos mais rigorosos da orientação a objetos, promovendo baixo acoplamento. Por padrão, antes do Java 8, todos os métodos em uma interface eram implicitamente `public` e `abstract`. A diferença crucial entre uma classe abstrata e uma interface é que **uma classe pode implementar múltiplas interfaces** simultaneamente, contornando a restrição de herança múltipla do Java.

- **Métodos Concretos (Default):** A partir do Java 8, para evitar quebra de código em sistemas antigos ao adicionar novos métodos, as interfaces ganharam os métodos `default`, que permitem adicionar implementações com corpo diretamente na interface.
- **Atributos:** Todos os atributos declarados dentro de uma interface são, por padrão e de forma redundante, **constantes** (`public static final`).
- **Métodos Estáticos:** Também introduzidos no Java 8, métodos estáticos em interfaces pertencem estritamente à própria interface e não podem ser sobrescritos pelas classes que a implementam, devendo ser chamados usando o nome da interface.

```
public interface DataLoader {

    // Atributo: é implicitamente public static final
    int MAX_DATA_SIZE = 1000;

    // Método abstrato: implicitamente public abstract
    void load();

    // Método default: possui corpo e é herdado pelas classes que implementam
    default void checkPermission() {
        System.out.println("Checando permissões de forma genérica...");
    }

    // Método estático: pertence apenas à interface, não pode ser sobrescrito
    static void retrieveMaxDataSize() {
        System.out.println("Tamanho máximo suportado: " + MAX_DATA_SIZE);
    }
}

public interface DataRemover {
    void remove();
}

// Uma classe implementando MÚLTIPLAS interfaces
public class DatabaseLoader implements DataLoader, DataRemover {

    @Override
    public void load() {
        System.out.println("Carregando dados do banco de dados...");
    }

    @Override
    public void remove() {
        System.out.println("Removendo dados do banco de dados...");
    }

    public static void main(String[] args) {
        DatabaseLoader db = new DatabaseLoader();
        db.load();
        db.remove();

        // Chamada do método default
        db.checkPermission();

        // Chamada do método estático diretamente pela Interface
        DataLoader.retrieveMaxDataSize();
    }
}
```
### Polimorfismo

**Polimorfismo e Funcionamento**

O **polimorfismo** (que significa "múltiplas formas") é considerado um dos pilares mais importantes da programação orientada a objetos,. Ele permite que uma **variável de referência de um tipo mais genérico (como uma superclasse ou interface) faça referência a um objeto de um tipo mais específico (uma subclasse)**,.

Fazendo uma analogia com o mundo real, a variável de referência atua como um controle remoto, enquanto o objeto instanciado na memória é a própria televisão,. A regra fundamental do polimorfismo é que, ao acionar um comportamento (método) através de uma referência genérica, **quem executa a ação é sempre o objeto real e mais específico que está alocado na memória**,. Isso garante que a versão correta do método, sobrescrita pela subclasse, seja executada.

---

**Parâmetros Polimórficos**

A utilização de parâmetros polimórficos serve para evitar a repetição de código e métodos sobrecarregados. Em vez de criar um método específico para cada subclasse (como `calcularImpostoComputador(Computador c)` e `calcularImpostoTomate(Tomate t)`), você cria um **único método genérico que recebe a superclasse como parâmetro** (ex: `calcularImposto(Produto produto)`),.

Essa abordagem deixa o código extremamente dinâmico e extensível: se no futuro uma nova subclasse for criada (como `Televisao`), **o método genérico continuará funcionando perfeitamente sem precisar de nenhuma alteração**, pois a nova classe passa no teste "é um" da superclasse,.

---

**Cast e `instanceof`**

O uso do polimorfismo traz uma restrição estrutural: ao utilizar a referência de uma superclasse, **você perde o acesso aos atributos e métodos que são exclusivos da subclasse** (como a `dataValidade` de um `Tomate` sendo acessada por uma referência de `Produto`),.

Para recuperar esse acesso, você precisa realizar um **cast** (fazer a referência voltar a apontar especificamente para o tipo da subclasse),. Contudo, forçar o cast diretamente é perigoso e pode gerar exceções de execução. Para garantir a segurança, você deve utilizar o operador **`instanceof`**, que **avalia e confirma se o objeto alocado na memória é realmente uma instância daquela subclasse específica** antes de realizar o cast e executar a lógica,.

---

**Programação Orientada a Interfaces**

A programação orientada a interfaces é uma técnica de design onde você **desacopla o seu código passando a depender de contratos (abstrações) ao invés de classes concretas**,,.

Na prática, isso significa que a sua variável de referência deve ser sempre do tipo da interface. Por exemplo, em vez de declarar `RepositorioBancoDeDados repo = new RepositorioBancoDeDados()`, você declara `Repositorio repo = new RepositorioBancoDeDados()`. Se no futuro os requisitos mudarem e você precisar salvar os dados em um arquivo, **basta alterar apenas a instância do objeto** para `new RepositorioArquivo()`. O restante do sistema continuará funcionando de forma idêntica e sem quebras, pois todas as implementações respeitam o mesmo contrato definido pela interface,.

---

**Exemplo de código:**

O código abaixo integra todos os conceitos acima: programação orientada a interfaces no repositório, parâmetros polimórficos para o cálculo de impostos, e o uso de `instanceof` e cast para acessar métodos específicos de subclasses.

```
// 1. Programação Orientada a Interface (Contrato genérico)
public interface Repositorio {
    void salvar();
}

// Implementações concretas
public class RepositorioBancoDeDados implements Repositorio {
    @Override
    public void salvar() {
        System.out.println("Salvando no banco de dados...");
    }
}

public class RepositorioArquivo implements Repositorio {
    @Override
    public void salvar() {
        System.out.println("Salvando no arquivo...");
    }
}

// -------------------------------------------------------------

// Superclasse abstrata genérica
public abstract class Produto {
    protected String nome;
    protected double valor;

    public Produto(String nome, double valor) {
        this.nome = nome;
        this.valor = valor;
    }

    public abstract double calcularImposto();

    public String getNome() { return nome; }
    public double getValor() { return valor; }
}

// Subclasses concretas
public class Computador extends Produto {
    public Computador(String nome, double valor) {
        super(nome, valor);
    }

    @Override
    public double calcularImposto() {
        return this.valor * 0.20; // 20% de imposto
    }
}

public class Tomate extends Produto {
    private String dataValidade; // Atributo exclusivo da subclasse

    public Tomate(String nome, double valor, String dataValidade) {
        super(nome, valor);
        this.dataValidade = dataValidade;
    }

    @Override
    public double calcularImposto() {
        return this.valor * 0.05; // 5% de imposto
    }

    // Método exclusivo da subclasse
    public String getDataValidade() {
        return dataValidade;
    }
}

// -------------------------------------------------------------

// Classe utilitária com Parâmetros Polimórficos
public class CalculadoraImposto {

    // 2. Parâmetro Polimórfico: Recebe a superclasse 'Produto'
    public static void calcularImposto(Produto produto) {
        System.out.println("Relatório de Imposto do Produto: " + produto.getNome());

        // 3. Polimorfismo: O método executado será o do objeto real em memória
        double imposto = produto.calcularImposto();
        System.out.println("Imposto a pagar: R$ " + imposto);

        // 4. Uso do instanceof e Cast seguro
        if (produto instanceof Tomate) {
            // Se o objeto em memória for um Tomate, faz o cast para acessar métodos exclusivos
            Tomate tomate = (Tomate) produto;
            System.out.println("Atenção, produto perecível! Validade: " + tomate.getDataValidade());

            /* Nota: No Java 16+ (Pattern Matching para instanceof), poderia ser feito assim:
               if (produto instanceof Tomate tomate) {
                   System.out.println("Validade: " + tomate.getDataValidade());
               }
            */
        }
    }
}

// -------------------------------------------------------------

// Classe Executável
public class MainTeste {
    public static void main(String[] args) {

        // Polimorfismo aplicado às referências e objetos
        Produto prod1 = new Computador("MacBook", 10000);
        Produto prod2 = new Tomate("Tomate Siciliano", 10, "15/12/2026");

        // Executando métodos com parâmetros polimórficos
        CalculadoraImposto.calcularImposto(prod1);
        System.out.println("-------------------------");
        CalculadoraImposto.calcularImposto(prod2);
        System.out.println("-------------------------");

        // Aplicando a Programação Orientada a Interfaces
        // É possível trocar facilmente a implementação sem alterar a variável 'repo'
        Repositorio repo = new RepositorioBancoDeDados();
        repo.salvar(); // Executa o método no banco de dados

        repo = new RepositorioArquivo();
        repo.salvar(); // Executa a alteração no arquivo
    }
}
```

## **Tratamento de Exceções**

### **Diferença entre Errors, RuntimeException e Exception** 
As exceções representam condições anormais e fluxos inesperados na sua aplicação. No Java, todos esses problemas derivam da classe global `Throwable`, que se ramifica em duas grandes vertentes:

- **Errors:** Representam problemas críticos de infraestrutura a nível da JVM (Java Virtual Machine), como falta de memória (`OutOfMemoryError`) ou o estouro da pilha de métodos por recursividade infinita (`StackOverflowError`). São erros irrecuperáveis em tempo de execução, fazendo com que o programa pare de funcionar.
- **RuntimeException (Unchecked Exceptions):** São as chamadas exceções não-checadas. Geralmente indicam falhas de lógica do próprio programador que poderiam ser evitadas, como acessar um método de um objeto nulo (`NullPointerException`) ou acessar uma posição inexistente num array (`ArrayIndexOutOfBoundsException`). O Java **não obriga** que essas exceções sejam tratadas ou declaradas para o programa compilar.
- **Exception (Checked Exceptions):** São exceções checadas pelo compilador. Elas representam problemas operacionais fora do controle direto da aplicação, como ler um arquivo deletado ou um banco de dados inativo. Nesse cenário, o Java **obriga o desenvolvedor a realizar um tratamento prévio** (ou lançar a exceção adiante) para que o código seja capaz de compilar.

---

### **Lançamento de exceções (unchecked e checked)** 
Quando uma regra de negócio falha, você pode criar e "jogar" uma exceção utilizando a palavra-chave `throw new` seguida da instância da exceção.

- Ao lançar uma **unchecked exception** (filha de `RuntimeException`), você não é obrigado a fazer com que o método avise o resto do código sobre esse risco.
- Porém, ao lançar uma **checked exception**, você é obrigado a avisar a todos que usarem aquele método adicionando a palavra-chave **`throws` na assinatura do método**, servindo como um alerta para quem for chamá-lo de que é obrigatório lidar com essa exceção.

---

### **Blocos de tratamento: Múltiplas exceções, Multi-catch em linha e Bloco finally**

- **Múltiplas exceções:** Ao tentar recuperar fluxos em um bloco `try`, você pode possuir vários `catch` distintos para dar respostas exclusivas a cada falha. A principal regra é **as exceções mais específicas sempre devem vir primeiro**. Se uma exceção genérica (como `Exception` ou `RuntimeException`) for colocada no primeiro bloco `catch`, o Java exibirá um erro de compilação, pois devido ao polimorfismo, ela capturaria todos os erros e faria os blocos inferiores nunca serem alcançados.
- **Multi-catch em linha:** Para evitar repetição de códigos de tratamentos iguais, o Java permite juntar várias exceções na mesma linha utilizando o pipe (`|`). A regra vital dessa funcionalidade é que **as exceções separadas pelo pipe não podem pertencer à mesma linha de herança** (não podem ter relação de pai e filho).
- **Bloco finally:** É a última cláusula de um tratamento, com a principal característica de que o seu código **sempre será executado, independentemente da operação ter sucesso, falhar com exceção ou até mesmo encontrar um comando `return` dentro do `try`**. Sua principal função é garantir o fechamento de recursos do sistema operacional alocados (arquivos, rede, conexões de banco) evitando lentidões e estouro de memória.

---

### **Try-with-resources** 

Para evitar a verbosidade de declarar, inicializar, e fechar recursos manuais usando o `finally`, o Java criou a sintaxe _try-with-resources_. Nela, você instancia os objetos diretamente dentro dos parênteses do bloco `try`, e **o Java se encarrega de chamar automaticamente o fechamento** deles. Para que isso seja possível, a classe que está sendo instanciada precisa obrigatoriamente **implementar as interfaces `Closeable` ou `AutoCloseable`**. Uma curiosidade é que caso você tenha múltiplos recursos declarados nessa estrutura, o Java os fechará na **ordem inversa de declaração**.

---

### **Exceções customizadas** 

Quando a linguagem não provê uma exceção que faça sentido para o seu negócio (ex: usuário tentando logar com a senha incorreta), é possível criar as suas próprias. Para isso, basta criar uma classe cujo nome termina em `Exception` e **estender a classe `Exception`** (se quiser forçar o desenvolvedor a tratar) ou **estender `RuntimeException`** (se quiser que seja opcional). Posteriormente, usa-se a sobrescrita do construtor de string com `super(mensagem)` para associar a mensagem de erro específica.

---

### **Exceções e regras de sobrescrita** 

Ao utilizar herança e sobrescrever um método em uma classe filha, surgem regras estritas referentes às `Checked Exceptions`:

1. A classe filha **não é obrigada** a declarar as exceções que a superclasse lança, podendo remover o comando `throws` do método.
2. Se decidir declarar, a classe filha só pode lançar **exatamente as mesmas exceções do pai ou classes filhas (mais específicas) das exceções do pai**.
3. O Java **proíbe** que o método sobrescrito lance superclasses (exceções mais genéricas) das exceções declaradas originalmente ou adicione checked exceptions completamente novas ao contrato.
4. Essas proibições não se aplicam a exceções do tipo _RuntimeException_, que podem ser declaradas livremente na assinatura.

---

**Exemplo Prático e Completo de Código:**

Abaixo, um código integrando o lançamento, exceções customizadas, polimorfismo em tratamentos múltiplos e automação de fechamento de recursos:

```
import java.io.Closeable;
import java.io.IOException;

// 1. Criando Exceções Customizadas
// Extendemos Exception (Checked) para forçar o tratamento obrigatório
class SaldoInsuficienteException extends Exception {
    public SaldoInsuficienteException(String mensagem) {
        super(mensagem);
    }
}

// 2. Criando um recurso que será fechado automaticamente (AutoCloseable/Closeable)
class ConexaoBancaria implements Closeable {
    public void processar(double valor) throws IOException, SaldoInsuficienteException {
        System.out.println("Processando operação de valor: " + valor);

        // 3. Lançamento de Exceções Baseado em Lógica de Negócio
        if (valor == 0) {
            // Unchecked Exception: não precisa estar no 'throws'
            throw new IllegalArgumentException("O valor de saque não pode ser zero.");
        }
        if (valor > 1000) {
            // Checked Exception Customizada: deve ser obrigatoriamente declarada no 'throws'
            throw new SaldoInsuficienteException("O saldo atual é menor do que o solicitado.");
        }
    }

    @Override
    public void close() {
        // Garantia de liberação de recurso externo
        System.out.println("Fechando conexão do banco de forma automática.");
    }
}

// Classe de Domínio e Subclasse (Para testar sobrescrita)
class Transacao {
    public void iniciar(double valor) throws IOException, SaldoInsuficienteException {
        // Código pai
    }
}

class TransacaoPix extends Transacao {
    // 4. Regras de Sobrescrita:
    // Posso não lançar exceções, lançar as mesmas ou lançar exceções mais específicas.
    // Proibido adicionar Checked Exceptions não definidas na Superclasse (Pai).
    @Override
    public void iniciar(double valor) throws SaldoInsuficienteException {
        System.out.println("Iniciando transação via PIX.");
    }
}

// --- CLASSE EXECUTÁVEL ---
public class ControleDeExcecoes {
    public static void main(String[] args) {

        System.out.println("--- Testando Sistema Bancário ---");

        // 5. Try-with-resources: fecha os recursos automaticamente dispensando try-finally manual.
        try (ConexaoBancaria banco = new ConexaoBancaria()) {

            banco.processar(2000.0); // Isso forçará a checked exception de saldo

        } catch (IllegalArgumentException | SaldoInsuficienteException e) {
            // 6. Multi-catch em linha: pegando exceções que NÃO estão na mesma linha de herança.
            System.out.println("Falha de Negócio/Validação: " + e.getMessage());

        } catch (IOException e) {
            System.out.println("Falha de comunicação IO com o banco: " + e.getMessage());

        } catch (Exception e) {
            // 7. Múltiplas Exceções: A classe Exception por ser mais genérica
            // deve obrigatoriamente estar no último bloco Catch.
            System.out.println("Erro grave desconhecido no sistema: " + e.getMessage());

        } finally {
            // 8. Bloco Finally executado de qualquer forma para consolidar ou enviar métricas.
            // Nota: O fechamento (close) da classe ocorrerá logicamente ANTES da execução deste bloco.
            System.out.println("Bloco finally acionado: Sistema rodou de forma prevista.");
        }
    }
}
```