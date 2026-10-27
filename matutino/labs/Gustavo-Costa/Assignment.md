**Gustavo Costa
RA: 22653426
Email: gustavo.cs@sempreceub.com**
---



##### **Assignment**



###### **Seção I**



1. Problema computacional é uma tarefa que precisa ser resolvida, através de um computador, descrita por entradas, processamento de dados e saída esperada. Algoritmo é uma sequencial finita de passos que resolve todas as possibilidades de um problema. Código-fonte é o algoritmo escrito em uma linguagem de programação como o Java.

2. O javac lê o código-fonte, confere a sintaxe e os tipos para verificar se há erros e ao final gera um bytecode no arquivo .class. A Java Virtual Machine (JVM) executa o bytecode gerado e traduz para a linguagem de máquina em que está rodando, por isso a linguagem Java consegue rodar em diferentes sistemas operacionais.

3. O main é o ponto de partida do programa, ao rodar o public class a JVM procura o método "public static void main(String\[] args)" e começa a execução por ele. Sem o main a classe não pode ser executada diretamente.

4. arquivo `.java` → `javac` → arquivo `.class` → JVM → programa em execução.

5. Na declaração escolhermos o tipo da variável e o nome que daremos a ela. Inicializar é atribuir o primeiro valor a ela. Uma variável declarada e não inicializada não pode ser usada e na hora de compilar apresenta um erro.

6. É de tipagem forte porque toda variável tem um tipo definido na declaração, o compilador não deixa misturar tipos incompatíveis sem conversão.



7\. int idade
double altura
char letraDaTurma
String nomeCompleto
boolean statusDeMatricula (matriculado ou não).



8\. Quando uma variável é declarada usando char o valor atribuído a ela deve vir entre aspas simples, ao colocar aspas duplas é referente à uma String então o compilador acusa "incompatible types: String cannot be converted to char".

&#x20;   Correção: 

&#x09;1 --> char resposta = 'S';

&#x09;2 --> String resposta = "S";



9\. hii
   world!



10\. A saída esperada é 2 porque como as variáveis são declaradas como inteiro o programa desconsidera o que vem depois do ponto então 2.5 passa a ser 2.


11\. Resultado: 103. Ao utilizar o x + y sem parênteses o programa concatena as variáveis então x + y gera 103.



12\. Resultado: 13. Os parênteses fazem a soma acontecer antes de concatenar com o restante do println.



13\. 2. Ao colar o 5 e o 2 sem "." (5.0 e 2.0) o programa primeiro calcula a divisão com 5 e 2 sendo inteiros e só depois ele atribui o tipo double a essa variável. Portanto primeiro chega-se ao resultado 2 e só depois ele passa a ser do tipo double.



14\. x = 20
    y = 10

&#x20;   O y recebe uma "cópia de x", portanto alterar o x depois não altera o valor de y.


15\. public class OlaCurso {

&#x20;   public static void main(String\[] args) {

&#x20;       System.out.print("Engenharia de ");

&#x20;       System.out.println("Software");

&#x20;  }

}



16\. public class Q16Matricula {

&#x20;   public static void main(String\[] args) {

&#x20;       

&#x20;       String nome = "Gustavo Costa";

&#x20;       int semestre = 1;

&#x20;       boolean matriculado = true;

&#x20;       

&#x20;       System.out.printf("Nome: %s\\n", nome);

&#x20;       System.out.printf("Semestre: %d\\n", semestre);

&#x20;       System.out.printf("Matriculado: %b\\n", matriculado);

&#x20;  }

}



17\. public class Q17CartaoProduto {

&#x20;   public static void main(String\[] args) {

&#x20;       

&#x20;       String descricao = "Camiseta gato miau";

&#x20;       int codigo = 13131313;

&#x20;       double preco = 100.00;

&#x20;       String categoria = "Roupas";

&#x20;       boolean disponivel = true;



&#x20;       System.out.println("==============Produto==============");

&#x20;       System.out.println("Descrição: " + descricao);

&#x20;       System.out.println("Código: " + codigo);

&#x20;       System.out.printf("Preço: R$ %.2f\\n", preco);

&#x20;       System.out.println("Categoria: " + categoria);

&#x20;       System.out.println("Disponível: " + disponivel);

&#x20;       System.out.println("===================================");

&#x20;  }

}



18\. import java.util.Scanner;



public class Q18Operacoes {

&#x20;   

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       

&#x20;       System.out.print("Digite o primeiro número: ");

&#x20;       int a = sc.nextInt();

&#x20;       System.out.print("Digite o segundo número: ");

&#x20;       int b = sc.nextInt();



&#x20;       System.out.println("Soma: " + (a + b));

&#x20;       System.out.println("Subtração: " + (a - b));   

&#x20;       System.out.println("Multiplicação: " + (a \* b));



&#x20;       sc.close();

&#x20;   }

}



19\. import java.util.Scanner;



public class Q19Idade {

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);



&#x20;       System.out.print("Digite o ano de nascimento: ");

&#x20;       int anoNascimento = sc.nextInt(); 

&#x20;       System.out.print("Digite o ano atual: ");

&#x20;       int anoAtual = sc.nextInt();



&#x20;       int idade = anoAtual - anoNascimento;

&#x20;       System.out.println("Idade: " + idade);



&#x20;       sc.close();

&#x20;   }

}



20\. import java.util.Scanner;



public class Q20AreaCirculo {



&#x20;   static final double PI = 3.14159;

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);



&#x20;       System.out.print("Digite o raio do círculo: ");

&#x20;       double raio = sc.nextDouble();



&#x20;       double area = PI \* raio \* raio;

&#x20;       System.out.printf("Área do círculo: %.2f\\n", area);



&#x20;       sc.close();

&#x20;   }

}



21\. import java.util.Scanner;



public class Q21MaiorQue100 {

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);



&#x20;       System.out.print("Digite um número: ");

&#x20;       int numero = sc.nextInt();

&#x20;       

&#x20;       if (numero>100) {

&#x20;           System.out.println("O número é maior que 100.");

&#x20;       } else if (numero==100){

&#x20;           System.out.println("O número é igual a 100.");

&#x20;       } else {

&#x20;           System.out.println("O número é menor que 100.");

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

22. import java.util.Scanner;



public class Q22CelsiusToFahrenheit {

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       

&#x20;       System.out.print("Digite a temperatura em Celsius: ");

&#x20;       double celsius = sc.nextDouble();

&#x20;       double fahrenheit = (celsius \* 9/5) + 32;

&#x20;       

&#x20;       System.out.printf("%.1f C= %.1f F", celsius, fahrenheit);

&#x20;       sc.close();

&#x20;   }

}



23\. public class Q23MediaPonderada {

&#x20;  public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       

&#x20;       System.out.print("Digite a primeira nota: ");

&#x20;       double nota1 = sc.nextDouble();

&#x20;       System.out.print("Digite o peso da primeira nota: ");

&#x20;       double peso1 = sc.nextDouble();

&#x20;       

&#x20;       System.out.print("Digite a segunda nota: ");

&#x20;       double nota2 = sc.nextDouble();

&#x20;       System.out.print("Digite o peso da segunda nota: ");

&#x20;       double peso2 = sc.nextDouble();

&#x20;       

&#x20;       System.out.print("Digite a terceira nota: ");

&#x20;       double nota3 = sc.nextDouble(); 

&#x20;       System.out.print("Digite o peso da terceira nota: ");

&#x20;       double peso3 = sc.nextDouble(); 



&#x20;       double mediaPonderada = (nota1 \* peso1 + nota2 \* peso2 + nota3 \* peso3) / (peso1 + peso2 + peso3);

&#x20;       System.out.printf("Média ponderada: %.2f\\n", mediaPonderada);

&#x20;      

&#x20;       sc.close();

&#x20;   } 

}



24\. import java.util.Scanner;



public class Q24SaqueTroco {

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       

&#x20;       System.out.print("Digite o valor do saque: ");

&#x20;       int saque = sc.nextInt();

&#x20;       int notas50 = saque / 50;

&#x20;       int troco = saque % 50;

&#x20;       

&#x20;       System.out.printf("Notas de 50: %d%n", notas50);

&#x20;       System.out.printf("Troco: %d%n", troco);

&#x20;       

&#x20;       sc.close();

&#x20;   }

}



25\. import java.util.Scanner;



public class Q25TemperaturaBooleans {

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);



&#x20;       System.out.print("Temperatura: ");

&#x20;       double temperatura = sc.nextDouble();



&#x20;       boolean abaixoDeZero = temperatura < 0;

&#x20;       boolean igualAZero = temperatura == 0;

&#x20;       boolean acimaDe30 = temperatura > 30;



&#x20;       System.out.println("Abaixo de zero: " + abaixoDeZero);

&#x20;       System.out.println("Igual a zero: " + igualAZero);

&#x20;       System.out.println("Acima de 30: " + acimaDe30);



&#x20;       sc.close();

&#x20;   }

}

&#x20;     

