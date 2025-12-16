# 🐾 AmigoFiel - Pet Shop Manager

> Sistema de gerenciamento via console para Pet Shops, focado em controle de serviços, estoque e agendamentos.

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Console App](https://img.shields.io/badge/Console_App-4D4D4D?style=for-the-badge&logo=windows-terminal&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-green)

## 📄 Sobre o Projeto

O **AmigoFiel** é uma aplicação Java baseada em CLI (Interface de Linha de Comando) desenvolvida para simular o ecossistema de gestão de uma loja.

O objetivo do projeto foi aplicar conceitos fundamentais de **Programação Orientada a Objetos (POO)** para resolver problemas reais de negócio, como baixa automática de estoque após uma venda e validação de agendamentos.

## ✨ Funcionalidades

O sistema possui um menu interativo que permite:

* 🐶 **Gestão de Animais:** Cadastro completo com nome, espécie, raça e dados do proprietário.
* 🚿 **Catálogo de Serviços:** Registro de serviços especializados (Banho, Tosa, Vacinação) com preços definidos.
* 📦 **Controle de Estoque:** Cadastro de produtos e monitoramento de quantidade disponível.
* 💰 **Sistema de Vendas:** Realiza a venda de produtos, calculando o valor total e **deduzindo automaticamente** a quantidade do estoque.
* 📅 **Agendamento Inteligente:** Vincula um animal a um serviço específico em data e hora marcadas.

## 🛠️ Tecnologias e Conceitos

O projeto foi construído utilizando Java puro, focando na estruturação lógica sem dependência de frameworks externos:

* **Java Collections (`ArrayList`):** Para manipulação dinâmica das listas de clientes, produtos e agendamentos em memória.
* **POO (Polimorfismo e Herança):** Estruturação das classes de Serviços (Banho, Tosa, Vacina).
* **Tratamento de Dados:** Uso de `Scanner` para entrada de dados e validação de tipos (prevenção de erros de digitação).
* **Lógica de Negócio:** Validação de estoque insuficiente antes de efetivar uma venda.

## 📂 Estrutura das Classes

O projeto está organizado nas seguintes entidades principais:

* `Main.java`: Classe principal que gerencia o fluxo do menu e a interação com o usuário.
* `Animal.java`: Representação dos pets clientes.
* `Produto.java`: Controle de itens vendáveis e estoque.
* `Servico.java`: Classe base para os serviços oferecidos.
* `Agenda.java`: Entidade associativa que liga Cliente + Serviço + Data.

## 🚀 Como Executar

### Pré-requisitos
* Ter o [Java JDK](https://www.oracle.com/java/technologies/downloads/) instalado.

### Passo a Passo

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/amigofiel.git](https://github.com/seu-usuario/amigofiel.git)
    ```

2.  **Acesse a pasta do projeto:**
    ```bash
    cd amigofiel
    ```

3.  **Compile o código:**
    ```bash
    javac amigofiel/*.java
    ```

4.  **Execute a aplicação:**
    ```bash
    java amigofiel.Main
    ```

## 📸 Exemplo de Uso (Console)

```text
Escolha uma opção:
1 - Cadastrar Animal
2 - Cadastrar Serviço
3 - Agendar Serviço
4 - Cadastrar Produto
5 - Vender Produto
6 - Sair
> 5

Lista de produtos disponíveis:
1. Ração Premium - R$ 150.0 - Estoque: 10
Selecione um produto: 1
Digite a quantidade: 2
Total a pagar: R$ 300.0
Venda realizada com sucesso!
