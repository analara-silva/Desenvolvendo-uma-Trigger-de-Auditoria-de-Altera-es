# Projeto: Trigger de Auditoria de Alterações

 **Obejetivo:** 
 Os alunos vão trabalhar juntos para criar uma trigger que registre automaticamente as alterações em uma tabela de um banco de dados, de modo a monitorar inserções, atualizações e exclusões.

 #
### **Passo a passo:**

**1.Introdução:** 
+ Faça a leitura do material.

**2.Divisão em Grupos:**
+ Cada grupo ficará responsável por uma parte da trigger, como explicação ou implementação de uma parte do código (inserção, atualização, exclusão).

**3.Tarefa:**
+ Crie um banco de dados fictício, como um sistema de gerenciamento de produtos (ou qualquer área de interesse).


+ A tabela principal pode ser produtos e a tabela de auditoria pode ser auditoria_produtos (que irá armazenar informações sobre a operação realizada, a data, o tipo de operação, o ID do produto e o valor alterado).

+ **Cada grupo deve:**

    - **Grupo 1:** Criar a tabela produtos e a tabela auditoria_produtos.

   - **Grupo 2:** Criar a trigger para capturar inserções na tabela produtos.

   - **Grupo 3:** Criar a trigger para capturar atualizações na tabela produtos.

   - **Grupo 4:** Criar a trigger para capturar exclusões na tabela produtos.

**4.Execução:**
Cada grupo deve implementar sua parte e testar as triggers com algumas operações no banco de dados (inserir, atualizar e excluir produtos).

**5.Discussão:**
Após a implementação, cada grupo apresenta seu código e explica como sua parte da trigger funciona.
 #

**Faço parte do grupo 1 e aqui está a resolução:**

` CREATE TABLE produtos (
id_produto INT PRIMARY KEY AUTO_INCREMENT,
nome VARCHAR (100) NOT NULL,
descricao VARCHAR (150) NOT NULL,
quantidade INT NOT NULL,
valor INT NOT NULL
);`
 
`CREATE TABLE auditoria_produto (
id_auditoria INT PRIMARY KEY AUTO_INCREMENT,
nome VARCHAR (100) NOT NULL,
descricao VARCHAR (150) NOT NULL,
quantidade INT NOT NULL,
valor INT NOT NULL,
data DATE NOT NULL
)`

#