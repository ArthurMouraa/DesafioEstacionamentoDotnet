# Desafio Estacionamento C#

Este é um projeto de console que simula o gerenciamento de um estacionamento. O aplicativo permite cadastrar, remover, listar veículos e calcular o valor total a ser pago com base no tempo de permanência.

O projeto foi desenvolvido como parte de um desafio para aprimorar habilidades em C# e programação orientada a objetos.

---

## Funcionalidades Implementadas

O aplicativo de estacionamento oferece as seguintes opções no menu principal:

* **Cadastrar veículo:** Permite registrar a entrada de um novo veículo no estacionamento, validando o formato da placa (padrão `LLL-NNNN`).
* **Remover veículo:** Permite registrar a saída de um veículo. O programa solicita a placa e a quantidade de horas que o veículo permaneceu, calculando o valor total a ser pago.
* **Listar veículos:** Exibe a lista de todos os veículos que estão atualmente estacionados.
* **Encerrar:** Encerra a aplicação.

---
## Requisitos do Sistema
-  .NET SDK
-  versão .NET 8.0.
-  IDE de sua prefereência. 

## Como Rodar o Projeto

Para executar este projeto, você precisará ter o **.NET SDK** instalado em sua máquina. O projeto foi configurado para rodar na versão **.NET 8.0**.

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/ArthurMouraa/DesafioEstacionamentoDotnet.git](https://github.com/ArthurMouraa/DesafioEstacionamentoDotnet.git)
    ```

2.  **Navegue até o diretório do projeto:**
    ```bash
    cd DesafioEstacionamentoDotnet/DesafioFundamentos
    ```

3.  **Execute a aplicação:**
    ```bash
    dotnet run
    ```

O aplicativo de console será iniciado, e você poderá interagir com o menu principal.

---

## Estrutura do Código

A lógica principal do programa está contida na classe `Estacionamento`, que gerencia a lista de veículos e as operações de entrada, saída e listagem.

* `AdicionarVeiculo()`: Utiliza **Expressões Regulares (Regex)** para validar o formato da placa e evita o cadastro de veículos duplicados.
* `RemoverVeiculo()`: Calcula o valor total com base no preço por hora e no preço inicial. Usa **`int.TryParse()`** para garantir que a entrada de horas seja um número válido.
* `ListarVeiculos()`: Verifica se a lista de veículos está vazia com o método **`.Any()`**, exibindo uma mensagem adequada.

Este projeto demonstra o uso de conceitos essenciais da linguagem C# e boas práticas de validação de dados.
