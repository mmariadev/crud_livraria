# Pesquisa sobre Prepared Statements.

## O que é um Prepared Statement
    Um Prepared Statement é uma técnica de execução de comandos SQL em que a estrutura da consulta é enviada ao banco de dados separadamente dos valores que ela vai usar.\ Em vez de montar o comando SQL completo já com os dados dentro, você primeiro define um "modelo" da consulta,\ com espaços reservados, nomeados de placeholders, e sendo representados por ?, no lugar dos valores que ainda serão informados.\ Só depois desses espaços serem definidos é que os dados reais são enviados e associados a eles. Essa técnica separa a estrutura da consulta, ou seja o SQL, dos dados reais, a entrada do usuário,\ o que muda completamente a forma como o banco interpreta a informação recebida.
## O problema de inserir dados do usuário direto no SQL

## O que é SQL Injection

## Como Prepared Statements protegem contra SQL Injection

## O processo de preparação, associação e execução (no PHP com MySQLi)

## Vantagens adicionais dos Prepared Statements

## Aplicação ao projeto crud_livraria
