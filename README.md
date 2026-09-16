# ☕ Curso de Java

Repositório destinado aos estudos e exercícios do **Curso de Java**, acompanhando a evolução desde os fundamentos da linguagem até conceitos avançados, Programação Orientada a Objetos, programação funcional, persistência de dados e desenvolvimento de interfaces gráficas com JavaFX.

---

## 🎯 Objetivo

Construir uma base sólida em **Java**, desenvolvendo gradualmente conhecimentos sobre:

* Lógica de programação
* Sintaxe e fundamentos da linguagem
* Estruturas de controle
* Programação Orientada a Objetos
* Coleções e estruturas de dados
* Tratamento de exceções
* Manipulação de arquivos
* Interfaces
* Generics
* Programação funcional
* Expressões Lambda
* JPA e Hibernate
* Desenvolvimento de interfaces com JavaFX

O curso será acompanhado por **exercícios, exemplos práticos e projetos**, permitindo aplicar os conceitos estudados ao longo do aprendizado.

---

# 📚 Conteúdo do Curso

## 01 — Introdução à Java

Primeiros conceitos da linguagem e preparação do ambiente.

### Conteúdos

* O que é Java
* Características da linguagem
* JDK, JRE e JVM
* Instalação e configuração do Java
* Compilação e execução
* Estrutura básica de um programa
* `main`
* `System.out.println()`
* Variáveis
* Tipos primitivos
* Entrada de dados
* `Scanner`
* Operadores

### Exemplo

```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite seu nome: ");
        String nome = scanner.nextLine();

        System.out.println("Olá, " + nome + "!");

        scanner.close();
    }
}
```

---

# 02 — Estrutura Sequencial

Execução de comandos em sequência.

### Conteúdos

* Variáveis
* Tipos de dados
* Atribuição
* Operadores aritméticos
* Operadores relacionais
* Operadores lógicos
* Entrada e saída de dados
* Conversão de tipos
* Casting

---

# 03 — Estrutura Condicional

Controle do fluxo de execução do programa.

### Conteúdos

* `if`
* `else`
* `else if`
* Operador ternário
* `switch`
* `case`
* `default`
* `break`

### Exemplo

```java
if (idade >= 18) {
    System.out.println("Maior de idade");
} else {
    System.out.println("Menor de idade");
}
```

---

# 04 — Estruturas Repetitivas

Execução repetida de determinados blocos de código.

### Conteúdos

* `while`
* `do while`
* `for`
* `break`
* `continue`
* Loops aninhados

### Exemplo

```java
for (int i = 0; i < 10; i++) {
    System.out.println(i);
}
```

---

# 05 — Tópicos Básicos sobre Java

Aprofundamento dos fundamentos da linguagem.

### Conteúdos

* Funções e métodos
* Parâmetros
* Retorno
* Escopo
* Modificadores
* `static`
* `final`
* `String`
* `StringBuilder`
* `Math`
* Datas básicas
* Convenções de código
* Organização de projetos

---

# 06 — Introdução à Programação Orientada a Objetos

Introdução aos principais conceitos da POO.

### Conteúdos

* Classes
* Objetos
* Atributos
* Métodos
* Estado
* Comportamento
* Instanciação
* Referências
* `new`

### Exemplo

```java
public class Conta {

    String titular;
    double saldo;

    void depositar(double valor) {
        saldo += valor;
    }
}
```

---

# 07 — Construtores, `this`, Sobrecarga e Encapsulamento

Aprofundamento da construção e organização de classes.

### Conteúdos

* Construtores
* Construtor padrão
* Construtores personalizados
* Palavra-chave `this`
* Sobrecarga de métodos
* Sobrecarga de construtores
* Modificadores de acesso
* `private`
* `public`
* `protected`
* Getters
* Setters
* Encapsulamento

### Exemplo

```java
public class Produto {

    private String nome;
    private double preco;

    public Produto(String nome, double preco) {
        this.nome = nome;
        this.preco = preco;
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }
}
```

---

# 08 — Comportamento de Memória, Arrays e Listas

Entendimento de como objetos e variáveis são armazenados e manipulados.

### Conteúdos

* Memória
* Stack
* Heap
* Tipos primitivos
* Tipos referência
* Referências
* Garbage Collector
* Arrays
* Vetores
* Matrizes
* `List`
* `ArrayList`

### Exemplo

```java
List<String> nomes = new ArrayList<>();

nomes.add("João");
nomes.add("Maria");
nomes.add("Carlos");

for (String nome : nomes) {
    System.out.println(nome);
}
```

---

# 09 — Data e Hora

Manipulação de datas, horários e períodos.

### Conteúdos

* `LocalDate`
* `LocalTime`
* `LocalDateTime`
* `Instant`
* `Duration`
* `Period`
* `DateTimeFormatter`
* Conversões
* Operações com datas

### Exemplo

```java
LocalDate hoje = LocalDate.now();

System.out.println(hoje);
```

---

# 10 — Enumerações e Composição

Representação de estados e relacionamento entre objetos.

### Enumerações

* `enum`
* Constantes
* Atributos em enums
* Métodos em enums

### Composição

* Relacionamento entre objetos
* Associação
* Composição de objetos
* Modelagem de classes

### Exemplo

```java
public enum StatusPedido {
    AGUARDANDO,
    PROCESSANDO,
    ENVIADO,
    ENTREGUE
}
```

---

# 11 — Herança e Polimorfismo

Estudo de relacionamentos entre classes e comportamentos diferentes para uma mesma interface.

### Conteúdos

* Herança
* `extends`
* `super`
* Classes base
* Classes derivadas
* Métodos sobrescritos
* `@Override`
* Polimorfismo
* Upcasting
* Downcasting
* Classes abstratas
* Métodos abstratos

### Exemplo

```java
public class Animal {

    public void emitirSom() {
        System.out.println("Som");
    }
}
```

```java
public class Cachorro extends Animal {

    @Override
    public void emitirSom() {
        System.out.println("Au au!");
    }
}
```

---

# 12 — Tratamento de Exceções

Controle de erros durante a execução dos programas.

### Conteúdos

* Exceções
* `try`
* `catch`
* `finally`
* `throw`
* `throws`
* Exceções checked
* Exceções unchecked
* Criação de exceções personalizadas

### Exemplo

```java
try {

    int resultado = 10 / 0;

} catch (ArithmeticException e) {

    System.out.println("Erro: divisão por zero.");

}
```

---

# 13 — Trabalhando com Arquivos

Manipulação de arquivos e diretórios.

### Conteúdos

* Arquivos
* Diretórios
* Caminhos
* Leitura
* Escrita
* `File`
* `Path`
* `Files`
* Streams de arquivos
* Leitura de texto
* Escrita de texto

### Exemplo

```java
Path caminho = Paths.get("arquivo.txt");

Files.writeString(
    caminho,
    "Olá, Java!"
);
```

---

# 14 — Interfaces

Definição de contratos para classes.

### Conteúdos

* Interfaces
* `implements`
* Métodos abstratos
* Métodos `default`
* Métodos `static`
* Polimorfismo através de interfaces
* Interfaces funcionais

### Exemplo

```java
public interface Pagamento {

    void pagar(double valor);
}
```

---

# 15 — Generics, Set e Map

Estruturas de dados e tipagem genérica.

### Generics

* Tipos genéricos
* Classes genéricas
* Métodos genéricos
* `<?>`
* `extends`
* `super`

### Set

* `Set`
* `HashSet`
* `TreeSet`
* Elementos únicos

### Map

* `Map`
* `HashMap`
* `TreeMap`
* Chave e valor
* Iteração sobre mapas

### Exemplo

```java
Map<String, Integer> usuarios = new HashMap<>();

usuarios.put("Joao", 21);
usuarios.put("Maria", 25);

System.out.println(
    usuarios.get("Joao")
);
```

---

# 16 — Programação Funcional e Expressões Lambda

Introdução ao paradigma funcional dentro do Java.

### Conteúdos

* Programação funcional
* Expressões Lambda
* Interfaces funcionais
* `Predicate`
* `Consumer`
* `Function`
* `Supplier`
* Method Reference
* `Stream`
* `filter`
* `map`
* `reduce`
* `forEach`

### Exemplo

```java
List<Integer> numeros = List.of(
    1, 2, 3, 4, 5
);

numeros.stream()
       .filter(n -> n % 2 == 0)
       .forEach(System.out::println);
```

---

# 17 — Mapeamento Objeto-Relacional com JPA e Hibernate

Persistência de objetos Java em bancos de dados relacionais.

### Conteúdos

* Banco de dados relacional
* ORM
* JPA
* Hibernate
* Entidades
* `@Entity`
* `@Id`
* `@GeneratedValue`
* Relacionamentos
* `@OneToOne`
* `@OneToMany`
* `@ManyToOne`
* `@ManyToMany`
* Persistência
* Consultas
* Transações

### Exemplo

```java
@Entity
public class Cliente {

    @Id
    @GeneratedValue
    private Long id;

    private String nome;

    // getters e setters
}
```

---

# 18 — JavaFX

Desenvolvimento de interfaces gráficas utilizando JavaFX.

### Conteúdos

* Introdução ao JavaFX
* `Stage`
* `Scene`
* Layouts
* `Button`
* `Label`
* `TextField`
* `TableView`
* Eventos
* CSS
* FXML
* Controllers
* Organização de aplicações JavaFX

### Exemplo

```java
public class Main extends Application {

    @Override
    public void start(Stage stage) {

        Label label = new Label("Olá, JavaFX!");

        Scene scene = new Scene(
            new StackPane(label),
            400,
            300
        );

        stage.setTitle("Minha aplicação");
        stage.setScene(scene);
        stage.show();
    }
}
```

---

# 🧪 Exercícios

Durante o curso serão desenvolvidos exercícios para praticar cada conceito.

Exemplos:

* Calculadoras
* Sistemas de cadastro
* Menus de terminal
* Sistemas bancários
* Manipulação de arquivos
* Sistemas utilizando POO
* Projetos com coleções
* Sistemas utilizando banco de dados
* Aplicações gráficas

---

# 🚀 Projetos

Ao longo do curso, os conhecimentos serão utilizados em projetos progressivamente mais complexos.

### 🏦 Projeto 01 — Sistema Bancário

Aplicação executada no terminal contendo:

* Login
* Cadastro
* Conta bancária
* Depósitos
* Saques
* Transferências
* Menu interativo
* Tratamento de erros

### 📁 Projeto 02 — Gerenciador de Arquivos

Aplicação para:

* Criar arquivos
* Ler arquivos
* Editar arquivos
* Excluir arquivos
* Listar diretórios

### 🗄️ Projeto 03 — Sistema com Banco de Dados

Aplicação utilizando:

* Java
* JPA
* Hibernate
* Banco de dados relacional

### 🖥️ Projeto 04 — Aplicação JavaFX

Aplicação gráfica utilizando:

* JavaFX
* FXML
* CSS
* Controllers
* Banco de dados

---

# 📂 Organização do Repositório

```text
curso-java/
│
├── 01-introducao-java/
│   ├── exemplos/
│   └── exercicios/
│
├── 02-estrutura-sequencial/
│   ├── exemplos/
│   └── exercicios/
│
├── 03-estrutura-condicional/
│   ├── exemplos/
│   └── exercicios/
│
├── 04-estrutura-repetitiva/
│   ├── exemplos/
│   └── exercicios/
│
├── 05-topicos-basicos/
│
├── 06-introducao-poo/
│
├── 07-construtores-this-sobrecarga-encapsulamento/
│
├── 08-memoria-arrays-listas/
│
├── 09-data-hora/
│
├── 10-enumeracoes-composicao/
│
├── 11-heranca-polimorfismo/
│
├── 12-excecoes/
│
├── 13-arquivos/
│
├── 14-interfaces/
│
├── 15-generics-set-map/
│
├── 16-programacao-funcional-lambda/
│
├── 17-jpa-hibernate/
│
├── 18-javafx/
│
└── projetos/
    ├── sistema-bancario/
    ├── gerenciador-arquivos/
    ├── sistema-banco-dados/
    └── aplicacao-javafx/
```

---

# 🛠️ Tecnologias

Durante o curso serão utilizadas tecnologias e ferramentas do ecossistema Java, incluindo:

* **Java**
* **JDK**
* **Git**
* **GitHub**
* **JPA**
* **Hibernate**
* **SQL**
* **JavaFX**
* **Maven**

---

# 📈 Progresso

* [ ] Introdução à Java
* [ ] Estrutura Sequencial
* [ ] Estrutura Condicional
* [ ] Estruturas Repetitivas
* [ ] Tópicos Básicos
* [ ] Introdução à POO
* [ ] Construtores, `this`, Sobrecarga e Encapsulamento
* [ ] Memória, Arrays e Listas
* [ ] Data e Hora
* [ ] Enumerações e Composição
* [ ] Herança e Polimorfismo
* [ ] Tratamento de Exceções
* [ ] Trabalhando com Arquivos
* [ ] Interfaces
* [ ] Generics, Set e Map
* [ ] Programação Funcional e Lambda
* [ ] JPA e Hibernate
* [ ] JavaFX

---

# 🎯 Objetivo Final

Ao concluir o curso, o objetivo é ser capaz de desenvolver aplicações Java utilizando desde os fundamentos da linguagem até conceitos avançados de **Programação Orientada a Objetos, coleções, programação funcional, persistência de dados e interfaces gráficas**.

> **Aprender programação é praticar, errar, entender o erro e tentar novamente.**

---

## 📌 Status

🚧 **Em desenvolvimento**

Este repositório será atualizado conforme o conteúdo do curso for estudado e novos exercícios e projetos forem desenvolvidos.
