# Autonomo Services

> Plataforma SaaS de gestão de serviços para profissionais autônomos e pequenas empresas.

## 📌 Sobre o projeto

O Autonomo Services é uma plataforma SaaS desenvolvida para ajudar profissionais autônomos e pequenas empresas a gerenciar todo o ciclo de seus serviços.

A plataforma permite centralizar clientes, orçamentos, aprovações, pagamentos, agendamentos e ordens de serviço em um único sistema.

O objetivo é reduzir a dependência de papel, planilhas, anotações e diferentes ferramentas utilizadas no dia a dia.

---

## 🎯 Problema

Profissionais que trabalham com serviços externos frequentemente utilizam diferentes ferramentas para administrar seus negócios.

É comum encontrar situações como:

- clientes controlados pelo WhatsApp;
- orçamentos feitos em papel ou planilhas;
- agenda separada;
- pagamentos controlados manualmente;
- dificuldade para acompanhar orçamentos aprovados;
- dificuldade para controlar serviços pendentes;
- falta de histórico dos serviços realizados;
- risco de executar um serviço sem receber o pagamento.

O Autonomo Services busca centralizar essas atividades em uma única plataforma.

---

## 💡 Solução

A plataforma permite que o profissional:

1. Cadastre seus clientes;
2. Crie orçamentos;
3. Gere um link público do orçamento;
4. Envie o orçamento ao cliente;
5. Permita que o cliente aprove ou recuse o orçamento;
6. Realize o pagamento conforme a política definida pela empresa;
7. Agende o serviço;
8. Gere uma ordem de serviço;
9. Acompanhe a execução;
10. Finalize o serviço;
11. Controle os pagamentos e o histórico do cliente.

---

## 🔄 Fluxo principal

```text
Cliente
   ↓
Orçamento
   ↓
Link público
   ↓
Cliente visualiza
   ↓
Aprovação
   ↓
Política de pagamento
   ↓
Pagamento / Entrada / Agendamento
   ↓
Agendamento
   ↓
Ordem de Serviço
   ↓
Execução
   ↓
Conclusão
```

---

## 💳 Políticas de pagamento

O sistema permitirá que cada empresa escolha como deseja trabalhar.

### 1. Pagamento 100% antecipado

```text
Aprovação
   ↓
Pagamento
   ↓
Agendamento
   ↓
Serviço
```

### 2. Pagamento com sinal

```text
Aprovação
   ↓
Entrada
   ↓
Agendamento
   ↓
Serviço
   ↓
Pagamento do restante
```

### 3. Pagamento após o serviço

```text
Aprovação
   ↓
Agendamento
   ↓
Serviço
   ↓
Pagamento
```

---

## 👥 Público-alvo

O primeiro público do projeto será composto por profissionais autônomos e pequenas empresas que trabalham com atendimento e execução de serviços.

Exemplos:

- Eletricistas;
- Encanadores;
- Técnicos de ar-condicionado;
- Vidraceiros;
- Marceneiros;
- Instaladores;
- Técnicos de informática;
- Assistências técnicas;
- Empresas de manutenção;
- Oficinas.

O sistema será desenvolvido inicialmente de forma genérica para que diferentes segmentos possam utilizar o mesmo núcleo da plataforma.

---

## 🚀 MVP

A primeira versão do sistema terá:

- [ ] Cadastro de empresa;
- [ ] Autenticação;
- [ ] Cadastro de clientes;
- [ ] Criação de orçamentos;
- [ ] Itens de orçamento;
- [ ] Link público do orçamento;
- [ ] Aprovação ou recusa do orçamento;
- [ ] Políticas de pagamento;
- [ ] Controle de pagamentos;
- [ ] Agendamento;
- [ ] Ordem de serviço;
- [ ] Dashboard;
- [ ] Histórico do cliente.

---

## 🔮 Funcionalidades futuras

Após a validação do MVP, poderão ser desenvolvidos módulos adicionais:

- Integração com WhatsApp;
- Estoque;
- Controle de fornecedores;
- Gestão de equipes;
- Comissões;
- Financeiro avançado;
- Módulo específico para oficinas;
- Gestão de veículos;
- Controle de peças;
- Emissão de documentos fiscais;
- Aplicativo mobile;
- Automação;
- Inteligência Artificial;
- Integrações com serviços externos.

---

## 🏗️ Arquitetura do projeto

A documentação completa do projeto será organizada em:

```text
docs/
│
├── 00-contexto/
├── 01-visao-do-produto/
├── 02-requisitos/
├── 03-regras-de-negocio/
├── 04-atores/
├── 05-casos-de-uso/
├── 06-fluxos/
├── 07-uml/
├── 08-modelo-de-dominio/
├── 09-arquitetura/
├── 10-banco-de-dados/
├── 11-api/
├── 12-seguranca/
└── 13-plano-de-implementacao/
```

---

## 📚 Documentação

A documentação será construída durante o desenvolvimento do projeto.

- Visão do Produto
- Requisitos
- Regras de Negócio
- Atores
- Casos de Uso
- Fluxos
- UML
- Modelo de Domínio
- Arquitetura
- Banco de Dados
- API
- Segurança
- Plano de Implementação

---

## 🛠️ Tecnologias

As tecnologias definitivas serão definidas durante a etapa de arquitetura e implementação.

A proposta inicial considera:

- TypeScript;
- Next.js;
- PostgreSQL;
- ORM;
- API REST;
- Git/GitHub.

---

## 📈 Objetivo do projeto

O objetivo inicial é desenvolver um MVP funcional capaz de atender o fluxo completo:

> **Cliente → Orçamento → Aprovação → Pagamento → Agendamento → Serviço → Conclusão**

Após a validação do MVP com usuários reais, o produto poderá evoluir para diferentes segmentos de serviços.

---

## 📄 Status

🚧 Projeto em fase de planejamento e documentação.

A implementação será iniciada após a definição dos requisitos, regras de negócio, modelos e arquitetura do sistema.
