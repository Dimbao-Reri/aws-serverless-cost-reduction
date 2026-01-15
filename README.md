# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 15 de Janeiro de 2026  
**Empresa:** Abstergo Industries  
**Responsável:** Paulo Leandro  

---

## 1. Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa **Abstergo Industries**, realizado por Paulo Leandro. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar a **diminuição de custos imediatos**. 

> "Transformamos um custo fixo de infraestrutura em um investimento variável que cresce apenas conforme o sucesso das vendas da distribuidora."

---

## 2. Descrição do Projeto
O projeto de implementação foi dividido em 3 etapas estratégicas, focadas em uma arquitetura moderna e econômica:

### **Etapa 1: Armazenamento e Data Lake**
* **Ferramenta:** `Amazon S3 (Simple Storage Service)`
* **Foco:** Armazenamento de dados escalável e de baixo custo.
* **Caso de Uso:** Centralização de arquivos CSV e JSON (vendas, lotes e notas fiscais). A utilização da classe **S3 Intelligent-Tiering** permite que o sistema mova automaticamente dados antigos para camadas mais baratas, reduzindo gastos sem intervenção manual.

### **Etapa 2: Processamento e Limpeza (ETL)**
* **Ferramenta:** `AWS Glue`
* **Foco:** Integração, limpeza e preparação de dados Serverless.
* **Caso de Uso:** Padronização de dados de diferentes farmácias. O Glue elimina a necessidade de servidores ligados 24/7; a empresa paga apenas pelo tempo de execução da limpeza dos dados, evitando ociosidade de hardware.

### **Etapa 3: Análise de Dados e BI**
* **Ferramenta:** `Amazon Athena`
* **Foco:** Análise de dados interativa usando SQL padrão.
* **Caso de Uso:** Extração de insights rápidos (ex: ranking de vendas por farmácia). Por ser uma ferramenta sem servidor, paga-se apenas pela quantidade de dados varridos em cada consulta, eliminando custos de manutenção de bancos de dados complexos.

---

## 3. Resumo para o Diretor (Diferencial Competitivo)
A arquitetura proposta adota o modelo **100% Serverless**. Isso significa que a empresa não terá custos fixos com servidores. Se não houver processamento de dados em um determinado dia, o custo operacional de computação será **zero**, garantindo que o orçamento de TI seja investido apenas onde há geração real de valor para a distribuição.

---

## 4. Conclusão
A implementação na Abstergo Industries visa otimizar a gestão de dados com baixo custo operacional, aumentando a eficiência e produtividade. 

Além da economia, a arquitetura foca na **blindagem dos ativos digitais**. Os dados no Amazon S3 são protegidos por criptografia **AES-256** e o acesso é controlado pelo **AWS IAM** (Princípio do Menor Privilégio). Essa estrutura garante total conformidade com a **LGPD**, oferecendo segurança e auditabilidade para a expansão da distribuidora.

---

## 5. Anexos: Referências Técnicas

| Etapa | Ferramenta | Links de Referência |
| :--- | :--- | :--- |
| **1** | **Amazon S3** | [Visão Geral](https://aws.amazon.com/pt/s3/) \| [Documentação](https://docs.aws.amazon.com/pt_br/s3/index.html) \| [Intelligent-Tiering](https://aws.amazon.com/pt/s3/storage-classes/intelligent-tiering/) |
| **2** | **AWS Glue** | [Visão Geral](https://aws.amazon.com/pt/glue/) \| [Documentação](https://docs.aws.amazon.com/pt_br/glue/index.html) \| [Custos de ETL](https://aws.amazon.com/pt/glue/pricing/) |
| **3** | **Amazon Athena** | [Visão Geral](https://aws.amazon.com/pt/athena/) \| [Documentação](https://docs.aws.amazon.com/pt_br/athena/index.html) \| [Preço por Consulta](https://aws.amazon.com/pt/athena/pricing/) |

---

**Assinatura:** Paulo Leandro  
*Analista de Dados*
