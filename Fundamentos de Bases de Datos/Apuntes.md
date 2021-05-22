![badge](imgs/badge.webp)

# Fundamentos de Bases de Datos

[TOC]

# Indice

* [Módulo 1: Bienvenida, conceptos básicos y Contexto Histórico de las Bases de Datos](#Bienvenida, conceptos básicos y Contexto Histórico de las Bases de Datos)
* [Módulo 2: Introducción a las Bases de Datos Relacionales](#Introducción a las Bases de Datos Relacionales)
  * [Historia de las RDB](#Historia de las RDB)
  * [Entidades y Atributos](#Entidades y Atributos)
  * Entidades de Platzi Blog
  * Relaciones
  * Múltiples Muchos
  * Diagrama ER
  * Diagrama Físico: Tipos de Datos y Constraints
  * Diagrama Físico: Normalizando Platziblog
  * Formas Normales en DB Relacionales

* Módulo 3: RDBMS (MySQL) o Cómo Hacer lo Anterior de Manera Práctica





## Bienvenida, conceptos básicos y Contexto Histórico de las Bases de Datos

Profesor: Israel Vázquez[^1].

¿Qué son las bases de datos? Complementan la arquitectura de Vonn Newman.

Se dividen en dos:

**Relacionales:** SQL Server (Microsoft), SQL (Oracle). Versiones Open soucre: PostgreSQL, neo4j, MariaDB.

**No relacionales:** MemcacheDB, Cassandra (Facebook), DynamoDBM, elasticsearch, BigQuery, MongoDB.

**Autoadministrados:** Se instala en mi PC/Servidor, me encargo de actualizaciones, mantenimiento, etc.

**Administrados:** Servicios que se ofertan. No se instala ni hace mantenimiento. 



[^1]: https://www.linkedin.com/in/israel-baurel-v%C3%A1zquez-morales/

## Introducción a las Bases de Datos Relacionales

### Historia de las RDB

> Surgen de la necesidad de conservar la información más allá de la memoria RAM. En la arquitectura de Vonn Newman se contempla la RAM y el procesamiento de datos, pero no el guardado de datos persistente (se apaga la PC, se inicia y se conservan los datos).
>
> Una primera aproximación fueron las bases de datos basadas en archivos: guardar datos separados por comas (texto plano) fácil de guardar pero no de recuperar ordenadamente. Hay necesidad de algo más estructurado:
>
> **[Edgar Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd)**: Inventor de Bases de Datos Relacionales.
>
> Inventó el **[álgebra relacional](https://www.geeksforgeeks.org/introduction-of-relational-algebra-in-dbms/)**. Cómo tenemos datos que se pueden empezar a mezclar y unir a través de diferentes propiedades y características.

**[12 Reglas de Codd](https://en.wikipedia.org/wiki/Codd%27s_12_rules)[^2]: **

[^2]: https://www.mindmeister.com/es/1079684487/las-12-reglas-de-codd-del-modelo-relacional?fullscreen=1#

### Entidades y Atributos

