# Certificação Azure DP-900 - Data Fundamentals
Repositório para conter minhas anotações e auxiliar nos estudos para a certificação Azure Data Fundamentals
## Considerações iniciais

### O que é a certificação DP-900
É uma certificação oferecida pela Microsoft da série "900", ou seja, as certificações fundamentais. Para obter a certificação é necessário passar no exame DP-900, composto por XXXX questões


### A quem se destina
A certificação Azure DP-900 é voltada para todos os profissionais que utilizam dados na nuvem da Azure, incluindo desenvolvedores, administradores de banco de dados (DBAs), Engenheiro sde dados, Analistas de Dados, entre outros.

### Quais são os tópicos abordados
Conceitos básicos de dados, dados relacionais, dados não-relacionais, Big Data e análise de dados.

### Habilidades medidas
- Descrever os principais conceitos de dados (25-30%)
- Identificar considerações sobre dados relacionais no Azure (20-25%)
- Descrever considerações sobre o trabalho com dados não relacionais no Azure (15-20%)
- Descrever uma carga de trabalho de análise no Azure (25% – 30%)

### Anotações

---

# Roteiro 1/4 - Descrever os principais conceitos de dados
## Módulo 1 - Explore os principais conceitos de dados

### 1. Introdução
Objetivos de aprendizagem:

- Identificar formatos de dados comuns;
- Descrever as opções para armazenar dados em arquivos;
- Descrever as opções para armazenar dados em bancos de dados
- Descrever as características das soluções de processamento de dados transacionais
- Descrever as características de soluções de processamento de dados analíticos


### 2. Identificar formatos de dados comuns

* **Dados** - são uma coleção de fatos (números, descrições e observações) usados para registrar informações.
* **Entidades** - são as estruturas de dados que organizam as informações. Ex: Clientes, produtos, pedidos, etc.
* **Atributos** - são as características das entidades. Ex.: um cliente [*entidade*] pode ter um nome, endereço, nº de telefone, etc[*atributos*].


Podemos classificar os dados como estruturados, semiestruturados ou não estruturados.

**Dados Estruturados**
* Obedecem a um esquema fixo - Todos os dados têm os mesmos campos ou propriedades.
* Normalmente se organizam em uma ou mais tabelas (esquema tabular):
	* cada linha representa uma instancia
	* cada coluna representa um atributo.
* geralmente são armazenados em um banco de dados relacional. (detalhado mais adiante)


[colar imagem das tabelas]

**Dados Semiestruturados**

Ex: JSON


**Dados não-estruturados**

Ex: fotos, videos e e-mails

### 3. Armazenamento de arquivos
[...]

## Módulo 2 - Explorar funções e serviços de dados

[...]

---

# Roteiro 2/4 - Explorar dados relacionais no Azure

# Roteiro 3/4 - Explorar dados relacionais no Azure

# Roteiro 4/4 - Descrever os principais conceitos de dados
## Módulo 1 - Explorar os conceitos básicos do data warehousing em grande escala 
### 1. Introdução


As soluções de armazenamento de dados em grande escala combinam armazenamento de dados convencional usado para dar suporte à BI (business intelligence) com técnicas usadas para as chamadas análises de "big data". Uma solução de armazenamento de dados convencional normalmente envolve a cópia de dados transacionais armazenados em um banco de dados relacional com um esquema otimizado para consultar e construir modelos multidimensionais. As soluções de processamento de Big Data, por outro lado, são usadas com grandes volumes de dados em vários formatos, que são carregados em lote ou capturados em fluxos em tempo real e armazenados em um data lake a partir do qual mecanismos de processamento distribuído, como o Apache Spark, são usados para processá-lo.

* As soluções de armazenamento de dados em grande escala são uma combinação entre armazenamento de dados convencional(utilizado para BI) e técnicas de Big Data.
* Armazenamento de dados convencional - cópia de dados transacionais de um banco de dados relacional utilizando um esquema otimizado para consultas e modelos multidimensionais.
* Processamento de Big Data:
	* Usa grandes volumes de dados em vários formatos;
	* em lote(batch) ou fluxo em tempo real(streaming);
	* armazenados em um data lake;
	* processamento distribuído, Ex.: Apache Spark.

Objetivos de aprendizagem

1. Identificar elementos comuns de uma solução em larga escala de data warehousing
2. Descrever os principais recursos de pipelines de ingestão de dados
3. Identificar os tipos comuns de armazenamento de dados analíticos e os serviços do Azure relacionados
4. Provisionar o Azure Synapse Analytics e usá-lo para ingerir, processar e consultar dados

### 2. Descrever uma arquitetura de data warehousing
A arquitetura de um Data Warehouse em larga escala pode variar, bem como as tecnologias utilizadas, mas em geral inclui os seguintes elementos:

[*colocar figura*] 

**1. Ingestão e processamento de Dados**

* Corresponde à "entrada" dos dados em um data lake ou data warehouse;
* Os dados podem ser provenientes de bancos de dados transacionais, arquivos, fluxos em tempo real(streaming), entre outros;
* Os dados são limpos, filtrados e reestruturados(otimizados) para análises em processos de ETL ou ELT.
* **ETL** (**E**xtração, **T**ransformação e carga[**L**oad]) - os dados são transformados **antes** de serem carregados;
* **ELT** (**E**xtração, carga[**L**oad] e **T**ransformação) - Os dados primeiro são copiados e **depois** transformados.
* O processamento de dados geralmente é feito em sistemas distribuídos ( podem processar grandes volumes de dados em paralelo usando clusters de vários nós)
	* Os dados podem ser provenientes de lotes estáticos (**Batch**) ou fluxo de dados em tempo real(**Streaming**)
	
[*OBS: Qual a real diferença prática entre ETL e ELT? processamento? armazenamento? desempenho?*]

**2. Armazenamento de dados analíticos**

Podem ser:

* **Data Warehouses** - estruturas relacionais
* **Data lakes** - baseados em sistemas de arquivos
* Arquiteturas Híbridas - **Data lakehouses** ou *banco de dados lake*;

**3. Modelo de dados Analíticos**

**4. Visualização de dados**


---



Materiais para estudo:

Detalhes sobre a certificação: https://docs.microsoft.com/pt-br/certifications/azure-data-fundamentals/
Detalhes sobre o exame: https://docs.microsoft.com/pt-br/certifications/exams/dp-900
