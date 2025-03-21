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

### 2. Instrumento

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
### 5. Carro
### 6. Moto
### 7. Celular
### 8. Flor
### 9. Livro
### 10.Time














