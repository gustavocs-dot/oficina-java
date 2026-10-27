**Gustavo Costa**\
**RA:** 22653426\
**Email:** gustavo.cs@sempreceub.com

---

# Assignment

## Seção I

**1.** Problema computacional é uma tarefa que precisa ser resolvida, através de um computador, descrita por entradas, processamento de dados e saída esperada. Algoritmo é uma sequencial finita de passos que resolve todas as possibilidades de um problema. Código-fonte é o algoritmo escrito em uma linguagem de programação como o Java.

**2.** O javac lê o código-fonte, confere a sintaxe e os tipos para verificar se há erros e ao final gera um bytecode no arquivo .class. A Java Virtual Machine (JVM) executa o bytecode gerado e traduz para a linguagem de máquina em que está rodando, por isso a linguagem Java consegue rodar em diferentes sistemas operacionais.

**3.** O main é o ponto de partida do programa, ao rodar o public class a JVM procura o método `public static void main(String[] args)` e começa a execução por ele. Sem o main a classe não pode ser executada diretamente.

**4.** arquivo `.java` → `javac` → arquivo `.class` → JVM → programa em execução.

**5.** Na declaração escolhermos o tipo da variável e o nome que daremos a ela. Inicializar é atribuir o primeiro valor a ela. Uma variável declarada e não inicializada não pode ser usada e na hora de compilar apresenta um erro.

**6.** É de tipagem forte porque toda variável tem um tipo definido na declaração, o compilador não deixa misturar tipos incompatíveis sem conversão.

**7.**

- `int idade`
- `double altura`
- `char letraDaTurma`
- `String nomeCompleto`
- `boolean statusDeMatricula` (matriculado ou não).

**8.** Quando uma variável é declarada usando char o valor atribuído a ela deve vir entre aspas simples, ao colocar aspas duplas é referente à uma String então o compilador acusa "incompatible types: String cannot be converted to char".

Correção:

1. `char resposta = 'S';`
2. `String resposta = "S";`

**9.**

```
hii
world!
```

**10.** A saída esperada é 2 porque como as variáveis são declaradas como inteiro o programa desconsidera o que vem depois do ponto então 2.5 passa a ser 2.

**11.** Resultado: 103. Ao utilizar o x + y sem parênteses o programa concatena as variáveis então x + y gera 103.

**12.** Resultado: 13. Os parênteses fazem a soma acontecer antes de concatenar com o restante do println.

**13.** 2. Ao colar o 5 e o 2 sem "." (5.0 e 2.0) o programa primeiro calcula a divisão com 5 e 2 sendo inteiros e só depois ele atribui o tipo double a essa variável. Portanto primeiro chega-se ao resultado 2 e só depois ele passa a ser do tipo double.

**14.**

- x = 20
- y = 10

O y recebe uma "cópia de x", portanto alterar o x depois não altera o valor de y.

**15.**

```java
public class OlaCurso {
    public static void main(String[] args) {
        System.out.print("Engenharia de ");
        System.out.println("Software");
    }
}
```

**16.**

```java
public class Q16Matricula {
    public static void main(String[] args) {

        String nome = "Gustavo Costa";
        int semestre = 1;
        boolean matriculado = true;

        System.out.printf("Nome: %s\n", nome);
        System.out.printf("Semestre: %d\n", semestre);
        System.out.printf("Matriculado: %b\n", matriculado);
    }
}
```

**17.**

```java
public class Q17CartaoProduto {
    public static void main(String[] args) {

        String descricao = "Camiseta gato miau";
        int codigo = 13131313;
        double preco = 100.00;
        String categoria = "Roupas";
        boolean disponivel = true;

        System.out.println("==============Produto==============");
        System.out.println("Descrição: " + descricao);
        System.out.println("Código: " + codigo);
        System.out.printf("Preço: R$ %.2f\n", preco);
        System.out.println("Categoria: " + categoria);
        System.out.println("Disponível: " + disponivel);
        System.out.println("===================================");
    }

}
```

**18.**

```java
import java.util.Scanner;

public class Q18Operacoes {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite o primeiro número: ");
        int a = sc.nextInt();
        System.out.print("Digite o segundo número: ");
        int b = sc.nextInt();

        System.out.println("Soma: " + (a + b));
        System.out.println("Subtração: " + (a - b));
        System.out.println("Multiplicação: " + (a * b));

        sc.close();
    }
}
```

**19.**

```java
import java.util.Scanner;

public class Q19Idade {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite o ano de nascimento: ");
        int anoNascimento = sc.nextInt();
        System.out.print("Digite o ano atual: ");
        int anoAtual = sc.nextInt();

        int idade = anoAtual - anoNascimento;
        System.out.println("Idade: " + idade);

        sc.close();
    }
}
```

**20.**

```java
import java.util.Scanner;

public class Q20AreaCirculo {

    static final double PI = 3.14159;
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite o raio do círculo: ");
        double raio = sc.nextDouble();

        double area = PI * raio * raio;
        System.out.printf("Área do círculo: %.2f\n", area);

        sc.close();
    }
}
```

**21.**

```java
import java.util.Scanner;

public class Q21MaiorQue100 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite um número: ");
        int numero = sc.nextInt();

        if (numero>100) {
            System.out.println("O número é maior que 100.");
        } else if (numero==100){
            System.out.println("O número é igual a 100.");
        } else {
            System.out.println("O número é menor que 100.");
        }
        sc.close();
    }
}
```

**22.**

```java
import java.util.Scanner;

public class Q22CelsiusToFahrenheit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite a temperatura em Celsius: ");
        double celsius = sc.nextDouble();
        double fahrenheit = (celsius * 9/5) + 32;

        System.out.printf("%.1f C= %.1f F", celsius, fahrenheit);
        sc.close();
    }
}
```

**23.**

```java
import java.util.Scanner;

public class Q23MediaPonderada {
   public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite a primeira nota: ");
        double nota1 = sc.nextDouble();
        System.out.print("Digite o peso da primeira nota: ");
        double peso1 = sc.nextDouble();

        System.out.print("Digite a segunda nota: ");
        double nota2 = sc.nextDouble();
        System.out.print("Digite o peso da segunda nota: ");
        double peso2 = sc.nextDouble();

        System.out.print("Digite a terceira nota: ");
        double nota3 = sc.nextDouble();
        System.out.print("Digite o peso da terceira nota: ");
        double peso3 = sc.nextDouble();

        double mediaPonderada = (nota1 * peso1 + nota2 * peso2 + nota3 * peso3) / (peso1 + peso2 + peso3);
        System.out.printf("Média ponderada: %.2f\n", mediaPonderada);

        sc.close();
    }
}
```

**24.**

```java
import java.util.Scanner;

public class Q24SaqueTroco {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite o valor do saque: ");
        int saque = sc.nextInt();
        int notas50 = saque / 50;
        int troco = saque % 50;

        System.out.printf("Notas de 50: %d%n", notas50);
        System.out.printf("Troco: %d%n", troco);

        sc.close();
    }
}
```

**25.**

```java
import java.util.Scanner;

public class Q25TemperaturaBooleans {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Temperatura: ");
        double temperatura = sc.nextDouble();

        boolean abaixoDeZero = temperatura < 0;
        boolean igualAZero = temperatura == 0;
        boolean acimaDe30 = temperatura > 30;

        System.out.println("Abaixo de zero: " + abaixoDeZero);
        System.out.println("Igual a zero: " + igualAZero);
        System.out.println("Acima de 30: " + acimaDe30);

        sc.close();
    }
}
```
