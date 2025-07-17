# 🛠️ Plano de Desenvolvimento (PDI) - 6 meses

**Objetivo:** Consolidando conhecimentos práticos e teóricos em arquitetura, microsserviços, Java, mensageria, cloud e práticas de desenvolvimento.

---

## 📌 Visão Geral do Plano

- **Mês 1-2:** Consolidação **Java, Spring, SQL/PLSQL, Git**.
- **Mês 2-3:** **ORM, Migration, REST, Design Patterns**.
- **Mês 3-4:** **Arquitetura de microsserviços e Multi Tenancy**.
- **Mês 4-5:** **Mensageria (Kafka), Processamento baseado em eventos**.
- **Mês 5-6:** **Docker, Kubernetes, AWS, Observabilidade**.
- **Durante todo o período:** Prática em **projetos internos, PRs, mentorias, blog técnico e pair programming**.

---

## 🗂️ Plano Detalhado

### 📌 Mês 1-2: Consolidação Java, Spring, SQL/PLSQL, Git

✅ **Java + Spring Framework**  
- **Exemplo de estudo:** Criar uma *API de cadastro de usuários* com Spring Boot, realizando operações CRUD, utilizando testes unitários (JUnit, Mockito) e boas práticas de clean code.
- 📘 Livro: *Effective Java* (Joshua Bloch).
- 🎓 Curso: *Spring Framework Expert* (Udemy).

✅ **SQL e PLSQL (Oracle/Postgres)**  
- **Exemplo de estudo:** Criar procedures para cálculos de relatórios mensais de vendas e geração de resumo por cliente, testando em Postgres.

✅ **Git e GitFlow**  
- **Exemplo de estudo:** Simular workflow de time real usando GitHub, praticando rebase, squash, pull requests e tags de release.

---

### 📌 Mês 2-3: ORM, Migration, REST, Design Patterns

✅ **ORM e JPA/Hibernate**  
- **Exemplo de estudo:** Criar um *projeto de biblioteca* com entidades Livro, Autor e Empréstimo, praticando mapeamentos ManyToMany, OneToMany e Lazy/Eager loading.

✅ **Migration com Liquibase/Flyway**  
- **Exemplo de estudo:** Versão inicial de banco com tabelas de produto e cliente, adicionando migrations de alterações em tabelas e criação de índices.

✅ **REST e HTTP**  
- **Exemplo de estudo:** Criar uma *API REST de gerenciamento de tarefas* com DTOs, validação e boas práticas de status codes.

✅ **Design Patterns**  
- **Exemplo de estudo:** Refatorar partes do projeto de tarefas utilizando Strategy para regras de prioridade, Builder para construção de objetos complexos, e Factory para criação de serviços.

---

### 📌 Mês 3-4: Arquitetura de microsserviços e Multi Tenancy

✅ **Microsserviços**  
- **Exemplo de estudo:** Criar *um sistema de pedidos*:
    - Serviço de pedidos (Order Service)
    - Serviço de pagamento (Payment Service)
    - Comunicação entre eles via REST inicialmente, preparando para migração futura para mensageria.
    - Usar Spring Cloud Config para configuração centralizada.

✅ **Multi Tenancy**  
- **Exemplo de estudo:** Adaptar o sistema de pedidos para suportar múltiplas lojas (tenants), utilizando *Schema-per-tenant* ou *Discriminator column* via Hibernate.

✅ **Documentação:** Diagramar a arquitetura no Excalidraw ou Lucidchart.

---

### 📌 Mês 4-5: Mensageria (Kafka), Processamento baseado em eventos

✅ **Kafka**  
- **Exemplo de estudo:** No *sistema de pedidos*:
    - Após o pedido ser criado, enviar evento “PedidoCriado” em um tópico Kafka.
    - Serviço de pagamento consome o evento para processar o pagamento.
    - Criar consumidores escaláveis e simular reprocessamento.

✅ **Event-Driven Processing**  
- **Exemplo de estudo:** Implementar *Envio de notificações de pedidos* utilizando Kafka ou outra fila (RabbitMQ como fallback), integrando com o serviço de pedidos.

---

### 📌 Mês 5-6: Docker, Kubernetes, AWS, Observabilidade

✅ **Docker & Kubernetes**  
- **Exemplo de estudo:** Containerizar o *sistema de pedidos e pagamentos* usando Docker Compose para rodar os serviços localmente.
- Criar um cluster local no Minikube:
    - Deploy dos serviços
    - Configuração de ingress
    - Health checks e escalabilidade básica.

✅ **AWS & Observabilidade**  
- **Exemplo de estudo (Projeto Prático):** *Controle de estoque distribuído*:
    - **Serviço A:** Cadastro e atualização de estoque, hospedado em uma Lambda exposta via API Gateway.
    - **Serviço B:** Processamento de pedidos, rodando em ECS.
    - **Serviço C:** Processamento de pagamento utilizando SQS para fila e Lambda para consumir.
    - Persistência em **RDS (Postgres)**.
    - Logs e métricas via **CloudWatch**.
    - Adicional: Exportar métricas para **Prometheus** e visualizar no **Grafana** local para treino de monitoramento.

---

## 🚀 Práticas Complementares

✅ **Projeto PDI Pessoal**
- Escolha entre:
    - **Sistema de pedidos e pagamentos** ou
    - **Controle de estoque distribuído na AWS**
- Desenvolver o projeto utilizando:
    - Spring Boot + JPA/Hibernate
    - Liquibase/Flyway
    - API REST
    - Kafka para fluxo de eventos
    - Docker e Kubernetes
    - AWS (S3, Lambda, ECS, RDS)
    - Observabilidade com Prometheus, Grafana, CloudWatch
    - GitFlow para versionamento e simulação de ciclo real de desenvolvimento.

✅ **Code Reviews & Pair Programming**
- Participar de PRs complexos e revisões em equipe.

✅ **Blog Técnico**
- Publicar aprendizados de cada módulo no Medium/Notion ou GitHub Pages.

✅ **Mentorias**
- Sessões de feedback mensal com seniors/tech leads.

✅ **Certificações (opcional):**
- AWS Developer Associate
- Spring Professional Certification
- Kafka Developer Certification

---

## 🧭 Fechamento

✅ Consolidação sólida em **Java, Spring, SQL, Git**  
✅ Experiência prática em **REST, Design Patterns, Microsserviços e Multi Tenancy**  
✅ Hands-on com **Kafka, Event-Driven, Docker, Kubernetes e AWS**  
✅ Projeto real e apresentável no PDI  
✅ Avanço em visão arquitetural, comunicação e liderança técnica

---
