# SQL Terminology

## **Level 1: RDBMS Architecture & Ecosystem**

* Base de données
* Database
* SGBD
* Instance
* SQL
* SQL déclaratif
* T-SQL (Transact-SQL)
* SQL Server Management Studio (SSMS)

## **Level 2: Data Modeling Foundations**

* Modèle EA
* Schema
* Schéma relationnel
* Table
* Ligne
* Colonne
* Champ
* Attribut
* Enregistrement
* Cardinalité
* One-to-One
* One-to-Many
* Many-to-Many
* Normalization
* Denormalization

## **Level 3: Primitive Data Types**

* BIT
* TINYINT
* SMALLINT
* BIGINT
* DECIMAL
* NUMERIC
* FLOAT
* REAL
* money
* CHAR
* VARCHAR
* NCHAR / NVARCHAR (Unicode)
* TEXT (DÉPRÉCIÉ)
* NTEXT (DÉPRÉCIÉ)
* TIME
* SMALLDATETIME
* DATETIME / DATETIME2
* VARBINARY
* XML data type
* UNIQUEIDENTIFIER

## **Level 4: Data Definition Language (DDL) & Constraints**

* DDL (Data Definition Language)
* CREATE TABLE
* ALTER TABLE
* DROP TABLE
* TRUNCATE TABLE
* CONSTRAINT
* PRIMARY KEY
* UNIQUE
* NOT NULL
* DEFAULT
* CHECK
* IDENTITY
* Auto-incrémentation

## **Level 5: Data Manipulation (DML) & Retrieval (DRL)**

* DML (Data Manipulation Language)
* DRL (Data Retrieval Language)
* SELECT
* FROM
* INSERT INTO
* VALUES
* DELETE FROM
* OUTPUT
* INSERTED
* DELETED
* DUAL

## **Level 6: Query Filtering, Logic & Built-in Functions**

* WHERE
* AND
* OR
* IN
* BETWEEN
* LIKE
* Wildcard
* IS (NOT) NULL
* Précédence des opérateurs
* Modulo
* ORDER BY
* ASC
* DESC
* DISTINCT
* Alias
* CASE...WHEN...THEN...ELSE...END
* COALESCE
* NULLIF
* CAST
* CONVERT
* ABS
* LEN
* LOWER
* UPPER
* LTRIM / RTRIM
* SUBSTRING
* CHARINDEX
* REPLACE
* REPLICATE
* Concaténation
* GETDATE()
* DATEADD / DATEDIFF
* DATEPART

## **Level 7: Aggregation & Grouping**

* COUNT
* SUM
* AVG
* MIN
* MAX
* GROUP BY
* HAVING

## **Level 8: Relational Mechanics & Joins**

* Intégrité référentielle
* FOREIGN KEY
* ON DELETE / ON UPDATE (CASCADE, SET NULL, SET DEFAULT, NO ACTION)
* Jointures horizontales / verticales
* INNER JOIN
* LEFT OUTER JOIN
* RIGHT OUTER JOIN
* FULL OUTER JOIN
* CROSS JOIN
* SELF-JOIN
* EQUI-JOIN
* NON EQUI-JOIN
* Produit cartésien

## **Level 9: Advanced Querying & Set Operations**

* Sous-requêtes (Subqueries - Scalaire, Multi-valeur, Tabulaire, Corrélée)
* EXISTS
* ANY
* ALL
* UNION [ALL]
* INTERSECT
* EXCEPT
* MINUS
* WITH
* CTE (Common Table Expression)
* Fusion de données (MERGE)
* MERGE INTO
* CUBE / ROLLUP
* OLAP (CUBE OLAP)

## **Level 10: Transactions, Concurrency & State**

* ACID (Atomique, Cohérente, Isolée, Durable)
* BEGIN TRANSACTION
* COMMIT
* ROLLBACK
* AUTO-COMMIT
* Verrous (Locks)
* DEADLOCK

## **Level 11: Programmability & Automation**

* View
* User-Defined Function (UDF)
* SQL Server Procedure
* Trigger

## **Level 12: Engine Architecture, Storage & Administration**

* Parser
* Query Optimizer
* Query Processor
* Query Executor
* Execution Plan
* Storage Engine
* Database Manager
* SQL Manager
* SQL Server Agent
* Page (8 KB)
* Extent
* Index
* Clustered / Non-Clustered Index
* .mdf (data file)
* .ndf (data file)
* .ldf (log file)
* ROWVERSION
* Collation
* SET
* Backup
* Recovery Model
* Log Shipping
* Mirroring
* Replication