# Desafio Banco em POO

Este projeto é uma aplicação simples de um sistema bancário desenvolvido em Python, utilizando conceitos de Programação Orientada a Objetos (POO). O objetivo é demonstrar o uso de classes, herança, encapsulamento e polimorfismo em um contexto prático.

## Estrutura do Código

### Classes Principais

1. **Cliente**: Representa um cliente do banco, com atributos como endereço e contas associadas. Possui métodos para realizar transações e adicionar contas.
   - **PessoaFisica**: Subclasse de `Cliente`, adiciona atributos específicos como nome, data de nascimento e CPF.

2. **Conta**: Representa uma conta bancária genérica, com atributos como saldo, número, agência e histórico de transações. Possui métodos para saque e depósito.
   - **ContaCorrente**: Subclasse de `Conta`, adiciona limites de saque e número máximo de saques permitidos.

3. **Historico**: Armazena o histórico de transações realizadas em uma conta.

4. **Transacao**: Classe abstrata que define a estrutura básica de uma transação. Possui subclasses:
   - **Saque**: Representa uma operação de saque.
   - **Deposito**: Representa uma operação de depósito.

### Funções Auxiliares

- **menu**: Exibe o menu principal para interação com o usuário.
- **filtrar_cliente**: Busca um cliente pelo CPF.
- **recuperar_conta_cliente**: Recupera a conta associada a um cliente.
- **depositar**: Realiza a operação de depósito.
- **sacar**: Realiza a operação de saque.
- **exibir_extrato**: Exibe o extrato de uma conta.
- **criar_cliente**: Cria um novo cliente.
- **criar_conta**: Cria uma nova conta para um cliente.
- **listar_contas**: Lista todas as contas cadastradas.

### Função Principal

A função `main` gerencia o fluxo principal do programa, permitindo que o usuário interaja com o sistema por meio de um menu.

## Como Executar

1. Certifique-se de ter o Python instalado em sua máquina.
2. Execute o arquivo `desafio_bancoem_POO.py`.
3. Siga as instruções exibidas no menu para realizar operações bancárias.

## Funcionalidades

- Criar clientes e contas.
- Realizar depósitos e saques.
- Exibir extratos.
- Listar contas cadastradas.

## Observações

Este projeto é uma implementação básica e não possui persistência de dados. Todas as informações são armazenadas em memória durante a execução do programa.
