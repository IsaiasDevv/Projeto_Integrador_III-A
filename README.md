# 🛒 Projeto Integrador III-A — Migração de Arquitetura Monolítica para Microsserviços

Este repositório contém o projeto desenvolvido para a disciplina **Projeto Integrador III-A**, do curso de **Análise e Desenvolvimento de Sistemas** da **PUC Goiás – CEAD**.  
O trabalho aborda a migração de uma aplicação monolítica para uma arquitetura distribuída baseada em microsserviços, considerando desempenho, segurança e escalabilidade.

---

## 📌 Objetivo Geral
Propor e documentar uma solução completa para migrar a aplicação monolítica da empresa fictícia **TechStore** para uma arquitetura distribuída de microsserviços.

---

## 🎯 Objetivos Específicos
- Analisar limitações do sistema monolítico atual  
- Identificar módulos principais do sistema  
- Propor microsserviços independentes  
- Estabelecer comunicação entre serviços (REST, gRPC, mensageria)  
- Criar uma estratégia de migração gradual e segura  
- Implementar mecanismos de Segurança da Informação (CID)  
- Criar diagramas UML da arquitetura atual e da nova arquitetura  

---

## 🏢 Cenário Base — TechStore
A **TechStore** é uma loja virtual de produtos eletrônicos que utiliza um sistema monolítico.  
Com o crescimento da demanda, foram identificados problemas como:

- Alto acoplamento  
- Baixa escalabilidade  
- Lentidão em picos de acesso  
- Falhas generalizadas em caso de erros  
- Dificuldade de manutenção  

---

## 🧱 Arquitetura Atual — Monolítica
O sistema atual utiliza:

- Código único  
- Banco de dados centralizado  
- Implantação unificada  
- Dependência total entre módulos  

Problemas:

- Baixa performance  
- Risco elevado de falhas  
- Evolução complexa  
- Manutenção difícil  

---

## 🧩 Arquitetura Proposta — Microsserviços
Os serviços definidos são:

- **Auth Service** — Usuários, login e tokens JWT  
- **Product Service** — Catálogo e estoque  
- **Order Service** — Processamento de pedidos  
- **Payment Service** — Transações financeiras  
- **Notification Service** — E-mails, SMS e notificações  
- **API Gateway** — Roteamento e autenticação central  

### Tecnologias e padrões:
- REST e gRPC  
- RabbitMQ ou Kafka  
- Bancos de dados independentes  
- Observabilidade e monitoramento  
- Escalabilidade horizontal  

---

## 🔄 Estratégia de Migração em 8 Fases
1. Análise completa do monolito  
2. Definição dos microsserviços  
3. Implementação do API Gateway  
4. Extração do Auth Service  
5. Migração de Produtos  
6. Criação do Order Service  
7. Implementação do Payment Service  
8. Desativação total do monolito  

---

## 🔐 Segurança da Informação — CID
### 🔒 Confidencialidade
- JWT  
- HTTPS/TLS  
- Criptografia em repouso  
- RBAC  
- Cofre de credenciais  

### 🧭 Integridade
- Hash seguro de senhas  
- Logs e trilhas de auditoria  
- Assinatura digital  
- Validação de dados  
- Consistência distribuída (SAGA)  

### ⚙ Disponibilidade
- Escalabilidade horizontal  
- Balanceamento de carga  
- Replicação de banco  
- Circuit breaker  
- Retry e timeout  
- Mensageria resiliente  
- Monitoramento contínuo  

---

## 📂 Estrutura do Repositório
