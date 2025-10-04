# 📊 Projeto: Modelagem Dimensional Universitária – Foco no Professor

## 🎯 Objetivo

Este projeto tem como objetivo transformar um modelo relacional de banco de dados universitário em um **modelo dimensional** no formato **esquema em estrela (star schema)**, com foco exclusivo na análise de dados relacionados aos **professores**.

---

## 🧩 Contexto

O modelo relacional original contempla diversas entidades acadêmicas, como alunos, disciplinas, cursos, departamentos e professores. No entanto, para fins analíticos, o projeto se concentra apenas nas informações relevantes para o **desempenho e atuação dos professores**, excluindo dados sobre alunos e pré-requisitos curriculares.

---

## 🛠️ Metodologia

A modelagem seguiu os seguintes passos:

1. **Análise do modelo relacional original**
2. **Definição da tabela fato**: `Ensino`, que centraliza os dados de ensino dos professores.
3. **Criação das tabelas dimensão**:
   - `Dim_Professor`
   - `Dim_Curso`
   - `Dim_Disciplina`
   - `Dim_Departamento`
   - `Dim_Data` (criada para permitir análises temporais)
4. **Exclusão de entidades não relacionadas ao foco analítico**, como `Aluno`, `Matriculado` e `Pré-Requisitos`.

---

## 🧠 Resultado

O resultado é um modelo dimensional que permite análises como:

- Quais disciplinas são ministradas por quais professores
- Em quais cursos e departamentos
- Em quais períodos e modalidades
- Distribuição de carga horária por professor

---

## 🖼️ Imagens do Projeto

### 📌 Modelo Relacional de Partida

![Modelo Relacional](imagens/imagem_modelo_relacional.png)

### ⭐ Modelo Dimensional Finalizado (Star Schema)

![Modelo Estrela](imagens/imagem_modelo_estrela.png)

---

## 📁 Estrutura do Projeto

