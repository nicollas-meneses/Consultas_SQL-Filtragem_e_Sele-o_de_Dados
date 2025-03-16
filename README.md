# 📌 Consultas SQL - Filtragem e Seleção de Dados

## 📖 Descrição
Este projeto contém consultas SQL que realizam operações de filtragem e seleção de dados em diferentes tabelas. O foco está em consultas para recuperar informações de estados, países e alunos com base em critérios específicos.

## 📌 Funcionalidades
- Selecionar estados cujo país seja de código 2 e tenham a letra "A" no nome.
- Buscar apenas os países que começam com a letra "C".
- Filtrar alunos que possuem sobrenome "Silva", tenham mais de 18 anos e não morem na cidade de código 1.

## 🚀 Consultas SQL
### 1️⃣ Estados que pertencem ao país de código 2 e contêm "A" no nome:
```sql
SELECT *
FROM ESTADOS
WHERE PAIS = 2 AND NOME LIKE '%A%';
```

### 2️⃣ Países que começam com a letra "C":
```sql
SELECT PAIS AS PAISES
FROM PAIS
WHERE NOME LIKE 'C%';
```

### 3️⃣ Alunos com sobrenome "Silva", idade maior que 18 e que não moram na cidade 1:
```sql
SELECT *
FROM ALUNOS
WHERE NOME LIKE '%SILVA%'
  AND IDADE > 18
  AND CIDADE <> 1;
```

## 🛠 Tecnologias Utilizadas
- **Banco de Dados Relacional (SQL)**
- **MySQL** (ou compatível, como PostgreSQL, SQL Server)

## 📝 Como Utilizar
1. Certifique-se de ter um banco de dados compatível.
2. Copie e cole as consultas em seu gerenciador SQL.
3. Execute as consultas e veja os resultados filtrados conforme os critérios definidos.

---
**© 2025 - Desenvolvido por Nicollas Meneses**

