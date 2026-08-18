# Pesquisa sobre Prepared Statements.

## O que é um Prepared Statement
Um Prepared Statement é uma técnica de execução de comandos SQL em que a estrutura da consulta é enviada ao banco de dados separadamente dos valores que ela vai usar. Em vez de montar o comando SQL completo já com os dados dentro, você primeiro define um "modelo" da consulta, com espaços reservados, nomeados de placeholders, e sendo representados por ?, no lugar dos valores que ainda serão informados. Só depois desses espaços serem definidos é que os dados reais são enviados e associados a eles. Essa técnica separa a estrutura da consulta, ou seja o SQL, dos dados reais, a entrada do usuário, o que muda completamente a forma como o banco interpreta a informação recebida.
## O problema de inserir dados do usuário direto no SQL
Quando os dados vindos de um formulário, como $_POST ou $_GET são conectados diretamente dentro do texto do comando SQL, o banco de dados recebe tudo como um único bloco de texto, ou seja, ele não tem como distinguir "isto é uma instrução que devo executar" de "isto é apenas um valor que devo armazenar ou comparar". E aplicando na prática, isso significa que qualquer caractere especial do SQL como as aspas, ponto e vírgula, palavras-chave como OR, DROP, UNION digitado pelo usuário passa a ser interpretado pelo banco como parte do comando, e não como um dado inofensivo. Isso abre uma brecha grave de segurança, porque o comportamento da consulta passa a depender do que a pessoa digitou e não do que o programador pretendia.
## O que é SQL Injection

## Como Prepared Statements protegem contra SQL Injection

## O processo de preparação, associação e execução (no PHP com MySQLi)

## Vantagens adicionais dos Prepared Statements

## Aplicação ao projeto crud_livraria
