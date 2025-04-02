# EXERCICIO 1
## Coletar 10 figuras contendo dois ou mais objetos de uma mesma classe. 
### 1. Video Games
![image](https://github.com/user-attachments/assets/f9e9caf0-62b1-4131-b6cf-39ddb8c5313e)

### 2. Instrumentos
![image](https://github.com/user-attachments/assets/78c34faa-545d-4b3b-b3ee-007b00ef2e02)


### 3. Pessoas
![image](https://github.com/user-attachments/assets/cab411fc-ac7d-4889-b63d-b48c2385f3df)

### 4. Animais
![image](https://github.com/user-attachments/assets/d7e8f539-d6f0-4900-aa91-d55b9180fb6a)

### 5. Carros
![image](https://github.com/user-attachments/assets/781b8e7b-e904-4552-9ab8-df2c5ba7940a)

### 6. Motos

![image](https://github.com/user-attachments/assets/92923174-cfee-4d0f-b12c-6ac4c45dca67)

### 7. Celulares
![image](https://github.com/user-attachments/assets/2b57e528-1d0c-4599-bd29-e34e5eec3141)

### 8. Flores

![image](https://github.com/user-attachments/assets/efff3310-2002-4b88-9278-89a71bbc3deb)

### 9. Livros

![image](https://github.com/user-attachments/assets/ed773fd0-7daf-41ed-acc7-ecd555713142)


### 10. Times

![image](https://github.com/user-attachments/assets/4c911abd-f51f-4094-a413-a9fd04a0e231)


# EXERCICIO 2 

## Modelar via UML ou outra ferramenta cada classe do item 1, com três métodos e três atributos. 

![image](https://github.com/user-attachments/assets/77d4e8c2-a4c0-4f3e-a9c8-2fd1e4093726)


# EXERCICIO 2 (utilizar o IntelliJ IDEA 2024.3.4)
## Implementar, usando a Linguagem Java, as classes modeladas no item 2.
### 1. Video Game

package org.example;
import java.util.Scanner;

public class Videogame {
    // Atributos
    private boolean ligar;
    private boolean desligar;
    private boolean jogar;
    private String nome;
    private int ano;
    private String cor;

    // Métodos setters
    public void setNome(String nome) {
        this.nome = nome;
    }

    public void setAno(int ano) {
        this.ano = ano;
    }

    public void setCor(String cor) {
        this.cor = cor;
    }

    // Métodos de ação
    public void Ligar() {
        ligar = true;
        System.out.println(nome + " está ligado.");
    }

    public void Desligar() {
        desligar = true;
        System.out.println(nome + " está desligado.");
    }

    public void Jogar() {
        jogar = true;
        System.out.println(nome + " está jogando.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Videogame videoGame = new Videogame();

        System.out.print("Digite o nome do VideoGame: ");
        videoGame.setNome(scanner.nextLine());

        System.out.print("Digite o ano de lançamento: ");
        videoGame.setAno(scanner.nextInt());
        scanner.nextLine();  // Limpar o buffer

        System.out.print("Digite a cor do VideoGame: ");
        videoGame.setCor(scanner.nextLine());

        System.out.println("\nAções do VideoGame:");
        videoGame.Ligar();
        videoGame.Jogar();
        videoGame.Desligar();

        scanner.close();
    }
}


### 2. Instrumento

package org.example;
import java.util.Scanner;

public class Instrumento {
    private String nome;
    private String tipo;
    private String fabricante;

    public void setNome(String nome) {
        this.nome = nome;
    }

    public void setIdade(String tipo) {
        this.tipo = tipo;
    }

    public void setEmail(String email) {
        this.fabricante= fabricante;
    }


    public void Andar() {
        System.out.println(nome + " tocar");
    }


    public void Estudar() {
        System.out.println(nome + " afinar");
    }


    public void Programar() {
        System.out.println(nome + " desafinar");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Instrumento instrumento = new Instrumento();

        System.out.print("Digite o Nome: ");
        instrumento.setNome(scanner.nextLine());

        System.out.print("Digite o Tipo: ");
       instrumento.setIdade(scanner.next());
        scanner.nextLine();

        System.out.print("Digite o Fabricante : ");
        instrumento.setEmail(scanner.nextLine());

        System.out.println("\nAções do Instrumento:");
        instrumento.Andar();
        instrumento.Estudar();
        instrumento.Programar();

        scanner.close();
    }
}

### 3. Pessoa

package org.example;
import java.util.Scanner;

public class Pessoa {
    private String nome;
    private int idade;
    private String email;

    public void setNome(String nome) {
        this.nome = nome;
    }

    public void setIdade(int idade) {
        this.idade = idade;
    }

    public void setEmail(String email) {
        this.email = email;
    }


    public void Andar() {
        System.out.println(nome + " andou");
    }


    public void Estudar() {
        System.out.println(nome + " Estudou");
    }


    public void Programar() {
        System.out.println(nome + " Programando");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Pessoa pessoa = new Pessoa();

        System.out.print("Digite o Nome: ");
        pessoa.setNome(scanner.nextLine());

        System.out.print("Digite a Idade: ");
        pessoa.setIdade(scanner.nextInt());
        scanner.nextLine();

        System.out.print("Digite o Email : ");
        pessoa.setEmail(scanner.nextLine());

        System.out.println("\nAções da Pessoa:");
        pessoa.Andar();
        pessoa.Estudar();
        pessoa.Programar();

        scanner.close();
    }
}

### 4. Animal

package org.example;
import java.util.Scanner;

public class Animal {
    // Atributos
    private boolean correr;
    private boolean comer;
    private boolean dormir;
    private String especie;
    private double peso;
    private int idade;

    // Métodos setters
    public void setEspecie(String especie) {
        this.especie = especie;
    }

    public void setPeso(double peso) {
        this.peso = peso;
    }

    public void setIdade(int idade) {
        this.idade = idade;
    }

    // Métodos de ação
    public void Correr() {
        correr = true;
        System.out.println(especie + " está correndo.");
    }

    public void Comer() {
        comer = true;
        System.out.println(especie + " está comendo.");
    }

    public void Dormir() {
        dormir = true;
        System.out.println(especie + " está dormindo.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Animal animal = new Animal();

        System.out.print("Digite a espécie do animal: ");
        animal.setEspecie(scanner.nextLine());

        System.out.print("Digite o peso do animal (em kg): ");
        animal.setPeso(scanner.nextDouble());

        System.out.print("Digite a idade do animal: ");
        animal.setIdade(scanner.nextInt());

        System.out.println("\nAções do Animal:");
        animal.Correr();
        animal.Comer();
        animal.Dormir();

        scanner.close();
    }
}


### 5. Carro

package org.example;
import java.util.Scanner;

public class Carro {
    // Atributos
    private boolean ligar;
    private boolean acelerar;
    private boolean frear;
    private String modelo;
    private int ano;
    private String cor;

    // Métodos setters
    public void setModelo(String modelo) {
        this.modelo = modelo;
    }

    public void setAno(int ano) {
        this.ano = ano;
    }

    public void setCor(String cor) {
        this.cor = cor;
    }

    // Métodos de ação
    public void Ligar() {
        ligar = true;
        System.out.println(modelo + " está ligado.");
    }

    public void Acelerar() {
        acelerar = true;
        System.out.println(modelo + " está acelerando.");
    }

    public void Frear() {
        frear = true;
        System.out.println(modelo + " está freando.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Carro carro = new Carro();

        System.out.print("Digite o modelo do carro: ");
        carro.setModelo(scanner.nextLine());

        System.out.print("Digite o ano de fabricação do carro: ");
        carro.setAno(scanner.nextInt());
        scanner.nextLine();  // Limpar o buffer

        System.out.print("Digite a cor do carro: ");
        carro.setCor(scanner.nextLine());

        System.out.println("\nAções do Carro:");
        carro.Ligar();
        carro.Acelerar();
        carro.Frear();

        scanner.close();
    }
}

### 6. Moto
package org.example;
import java.util.Scanner;

public class Moto {
    // Atributos
    private boolean ligar;
    private boolean acelerar;
    private boolean frear;
    private String modelo;
    private int ano;
    private String cor;

    // Métodos setters
    public void setModelo(String modelo) {
        this.modelo = modelo;
    }

    public void setAno(int ano) {
        this.ano = ano;
    }

    public void setCor(String cor) {
        this.cor = cor;
    }

    // Métodos de ação
    public void Ligar() {
        ligar = true;
        System.out.println(modelo + " está ligado.");
    }

    public void Acelerar() {
        acelerar = true;
        System.out.println(modelo + " está acelerando.");
    }

    public void Frear() {
        frear = true;
        System.out.println(modelo + " está freando.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Moto moto = new Moto();

        System.out.print("Digite o modelo da moto: ");
        moto.setModelo(scanner.nextLine());

        System.out.print("Digite o ano de fabricação da moto: ");
        moto.setAno(scanner.nextInt());
        scanner.nextLine();  // Limpar o buffer

        System.out.print("Digite a cor da moto: ");
        moto.setCor(scanner.nextLine());

        System.out.println("\nAções da Moto:");
        moto.Ligar();
        moto.Acelerar();
        moto.Frear();

        scanner.close();
    }
}

### 7. Celular

import java.util.Scanner;

public class Celular {
    // Atributos
    private boolean ligar;
    private boolean desligar;
    private boolean fotografar;
    private String modelo;
    private int ano;
    private String cor;

    // Métodos setters
    public void setModelo(String modelo) {
        this.modelo = modelo;
    }

    public void setAno(int ano) {
        this.ano = ano;
    }

    public void setCor(String cor) {
        this.cor = cor;
    }

    // Métodos de ação
    public void Ligar() {
        ligar = true;
        System.out.println(modelo + " está ligado.");
    }

    public void Desligar() {
        desligar = true;
        System.out.println(modelo + " está desligado.");
    }

    public void Fotografar() {
        fotografar = true;
        System.out.println(modelo + " está tirando uma foto.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Celular celular = new Celular();

        System.out.print("Digite o modelo do celular: ");
        celular.setModelo(scanner.nextLine());

        System.out.print("Digite o ano de fabricação do celular: ");
        celular.setAno(scanner.nextInt());
        scanner.nextLine();  // Limpar o buffer

        System.out.print("Digite a cor do celular: ");
        celular.setCor(scanner.nextLine());

        System.out.println("\nAções do Celular:");
        celular.Ligar();
        celular.Fotografar();
        celular.Desligar();

        scanner.close();
    }
}

### 8. Flor
import java.util.Scanner;

public class Flor {
    // Atributos
    private boolean regar;
    private boolean florescer;
    private boolean murchar;
    private String nome;
    private String cor;
    private String aroma;

    // Métodos setters
    public void setNome(String nome) {
        this.nome = nome;
    }

    public void setCor(String cor) {
        this.cor = cor;
    }

    public void setAroma(String aroma) {
        this.aroma = aroma;
    }

    // Métodos de ação
    public void Regar() {
        regar = true;
        System.out.println(nome + " foi regada.");
    }

    public void Florescer() {
        florescer = true;
        System.out.println(nome + " está florescendo.");
    }

    public void Murchar() {
        murchar = true;
        System.out.println(nome + " está murchando.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Flor flor = new Flor();

        System.out.print("Digite o nome da flor: ");
        flor.setNome(scanner.nextLine());

        System.out.print("Digite a cor da flor: ");
        flor.setCor(scanner.nextLine());

        System.out.print("Digite o aroma da flor: ");
        flor.setAroma(scanner.nextLine());

        System.out.println("\nAções da Flor:");
        flor.Regar();
        flor.Florescer();
        flor.Murchar();

        scanner.close();
    }
}

### 9. Livro
import java.util.Scanner;

public class Livro {
    // Atributos
    private boolean avaliar;
    private boolean emprestar;
    private boolean abrirPagina;
    private String titulo;
    private String autor;
    private int ano;

    // Métodos setters
    public void setTitulo(String titulo) {
        this.titulo = titulo;
    }

    public void setAutor(String autor) {
        this.autor = autor;
    }

    public void setAno(int ano) {
        this.ano = ano;
    }

    // Métodos de ação
    public void Avaliar() {
        avaliar = true;
        System.out.println("Você avaliou o livro: " + titulo);
    }

    public void Emprestar() {
        emprestar = true;
        System.out.println("Você emprestou o livro: " + titulo);
    }

    public void AbrirPagina() {
        abrirPagina = true;
        System.out.println("Você abriu uma página do livro: " + titulo);
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Livro livro = new Livro();

        System.out.print("Digite o título do livro: ");
        livro.setTitulo(scanner.nextLine());

        System.out.print("Digite o autor do livro: ");
        livro.setAutor(scanner.nextLine());

        System.out.print("Digite o ano de publicação do livro: ");
        livro.setAno(scanner.nextInt());

        System.out.println("\nAções com o Livro:");
        livro.Avaliar();
        livro.Emprestar();
        livro.AbrirPagina();

        scanner.close();
    }
}


### 10.Time

import java.util.Scanner;

public class Time {
    // Atributos
    private boolean ganhar;
    private boolean empatar;
    private boolean perder;
    private String nome;
    private String pais;
    private int titulos;

    // Métodos setters
    public void setNome(String nome) {
        this.nome = nome;
    }

    public void setPais(String pais) {
        this.pais = pais;
    }

    public void setTitulos(int titulos) {
        this.titulos = titulos;
    }

    // Métodos de ação
    public void Ganhar() {
        ganhar = true;
        System.out.println(nome + " ganhou um jogo.");
    }

    public void Empatar() {
        empatar = true;
        System.out.println(nome + " empatou um jogo.");
    }

    public void Perder() {
        perder = true;
        System.out.println(nome + " perdeu um jogo.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Time time = new Time();

        System.out.print("Digite o nome do time: ");
        time.setNome(scanner.nextLine());

        System.out.print("Digite o país do time: ");
        time.setPais(scanner.nextLine());

        System.out.print("Digite o número de títulos do time: ");
        time.setTitulos(scanner.nextInt());

        System.out.println("\nAções do Time:");
        time.Ganhar();
        time.Empatar();
        time.Perder();

        scanner.close();
    }
}















