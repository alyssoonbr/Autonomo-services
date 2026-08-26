# 1. Visão do Produto



## 1.1 Identificação



**Nome do projeto:** Autonomo Services



**Tipo:** SaaS — Software as a Service



**Categoria:** Gestão de serviços



**Status:** Em planejamento e desenvolvimento do MVP



\---

# 1. Visão do Produto

## 1.1 Identificação

**Nome do projeto:** Autonomo Services

**Tipo:** SaaS — Software as a Service

**Categoria:** Gestão de serviços

**Status:** Em planejamento e desenvolvimento do MVP

---

## 1.2 Descrição do Produto

O Autonomo Services é uma plataforma SaaS destinada a profissionais autônomos e pequenas empresas que trabalham com prestação de serviços.

A plataforma tem como objetivo centralizar o gerenciamento de clientes, orçamentos, aprovações, pagamentos, agendamentos e ordens de serviço em um único sistema.

O sistema será desenvolvido inicialmente como uma aplicação web responsiva, permitindo sua utilização em computadores, tablets e dispositivos móveis.

---

## 1.3 Problema

Profissionais que trabalham com prestação de serviços frequentemente utilizam diferentes ferramentas para administrar suas atividades.

É comum encontrar situações como:

* Clientes controlados principalmente pelo WhatsApp;
* Orçamentos feitos em papel, mensagens ou planilhas;
* Agenda separada do controle dos serviços;
* Pagamentos controlados manualmente;
* Dificuldade para acompanhar orçamentos aprovados;
* Dificuldade para controlar serviços pendentes;
* Falta de histórico organizado dos serviços realizados;
* Risco de executar um serviço sem receber o pagamento;
* Dificuldade para acompanhar vários serviços simultaneamente.

Esses problemas podem resultar em perda de tempo, desorganização, esquecimentos e prejuízos financeiros.

O Autonomo Services busca centralizar essas atividades em uma única plataforma.

---

## 1.4 Solução Proposta

O Autonomo Services permitirá que o profissional gerencie o ciclo de prestação de serviços desde a criação do orçamento até a conclusão do serviço.

O fluxo principal será:

```text
Prestador
    ↓
Cadastra cliente
    ↓
Cria orçamento
    ↓
Envia link para o cliente
    ↓
Cliente visualiza
    ↓
Cliente aprova ou recusa
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

O cliente poderá acessar o orçamento através de um link público enviado pelo prestador, sem precisar criar uma conta na plataforma.

---

## 1.5 Público-Alvo

O público-alvo inicial será composto por profissionais autônomos e pequenas empresas que realizam serviços externos ou atendimentos sob demanda.

### Exemplos de segmentos

* Eletricistas;
* Encanadores;
* Técnicos de ar-condicionado;
* Vidraceiros;
* Marceneiros;
* Instaladores;
* Técnicos de informática;
* Assistências técnicas;
* Empresas de manutenção;
* Oficinas;
* Outros profissionais que trabalham com prestação de serviços.

O produto será desenvolvido de forma genérica para que diferentes segmentos possam utilizar o mesmo núcleo da plataforma.

---

## 1.6 Usuários do Sistema

### Prestador

É o profissional ou empresa que contrata e utiliza o Autonomo Services.

Entre suas principais atividades estarão:

* Cadastrar clientes;
* Criar orçamentos;
* Enviar orçamentos;
* Acompanhar aprovações;
* Controlar pagamentos;
* Realizar agendamentos;
* Criar ordens de serviço;
* Acompanhar serviços;
* Finalizar serviços;
* Consultar histórico.

### Cliente

É a pessoa que recebe um orçamento enviado pelo prestador.

O cliente poderá:

* Acessar o orçamento através do link;
* Visualizar os serviços e valores;
* Aprovar o orçamento;
* Recusar o orçamento;
* Realizar o pagamento quando aplicável;
* Consultar informações relacionadas ao serviço.

O cliente não precisará criar uma conta na plataforma para acessar o orçamento.

---

## 1.7 Proposta de Valor

O Autonomo Services busca oferecer ao profissional uma maneira simples de administrar seus serviços desde o orçamento até o pagamento e execução.

A proposta central do produto é:

> **"Gerencie seus serviços desde o orçamento até o pagamento e execução em um único lugar."**

A plataforma também busca reduzir o risco financeiro do prestador ao permitir diferentes políticas de pagamento.

---

## 1.8 Políticas de Pagamento

Cada empresa poderá definir como deseja receber pelos serviços.

### 1.8.1 Pagamento 100% Antecipado

Fluxo:

```text
Aprovação
    ↓
Pagamento
    ↓
Agendamento
    ↓
Execução
```

Nesse modelo, o serviço somente poderá avançar para o agendamento após a confirmação do pagamento.

### 1.8.2 Pagamento com Sinal

Fluxo:


Aprovação
    ↓
Pagamento da entrada
    ↓
Agendamento
    ↓
Execução
    ↓
Pagamento do restante


Nesse modelo, o prestador recebe uma entrada antes da execução e o restante será pago conforme as condições definidas pela empresa.

### 1.8.3 Pagamento após o Serviço

Fluxo:

```text
Aprovação
    ↓
Agendamento
    ↓
Execução
    ↓
Pagamento
```

Nesse modelo, o pagamento será realizado após a execução do serviço.

---

## 1.9 Escopo do MVP

O MVP terá como objetivo validar o fluxo principal de gestão de serviços.

### Empresa e Autenticação

* Cadastro da empresa;
* Cadastro do usuário administrador;
* Login;
* Configurações básicas da empresa.

### Clientes

* Cadastro;
* Edição;
* Consulta;
* Histórico.

### Orçamentos

* Criação;
* Edição;
* Itens;
* Valores;
* Descontos;
* Validade;
* Status;
* Link público.

### Aprovação

* Visualização pelo cliente;
* Aprovação;
* Recusa;
* Registro da ação.

### Pagamentos

* Definição da política de pagamento;
* Controle de entrada;
* Controle do saldo;
* Status do pagamento;
* Registro do pagamento.

### Agenda

* Agendamento;
* Data;
* Horário;
* Cliente;
* Serviço;
* Endereço;
* Status.

### Ordem de Serviço

* Criação;
* Informações do serviço;
* Observações;
* Fotos;
* Materiais utilizados;
* Status;
* Conclusão.

### Dashboard

* Resumo dos orçamentos;
* Resumo dos pagamentos;
* Próximos agendamentos;
* Serviços em andamento;
* Serviços concluídos.

---

## 1.10 Fora do Escopo do MVP

As funcionalidades abaixo não farão parte da primeira versão:

* Aplicativo mobile nativo;
* Integração automática com WhatsApp;
* Controle avançado de estoque;
* Gestão de fornecedores;
* Gestão avançada de equipes;
* Comissões;
* Financeiro avançado;
* Gestão específica de oficinas;
* Gestão de veículos;
* Controle avançado de peças;
* Emissão de documentos fiscais;
* Contabilidade;
* Inteligência Artificial;
* Marketplace de prestadores;
* Sistema de busca pública de profissionais.

Essas funcionalidades poderão ser avaliadas após a validação do MVP.

---

## 1.11 Visão de Evolução do Produto

Após a validação do MVP, o Autonomo Services poderá evoluir para uma plataforma modular de gestão empresarial.

Possíveis módulos futuros:

```text
Autonomo Services
│
├── Gestão de Serviços
├── Orçamentos
├── Ordens de Serviço
├── Pagamentos
├── Agenda
├── Clientes
├── WhatsApp
├── Estoque
├── Fornecedores
├── Equipes
├── Financeiro
├── Oficina
└── Inteligência Artificial
```

A arquitetura do sistema deverá permitir a inclusão de novos módulos sem comprometer o funcionamento do núcleo existente.

---

## 1.12 Premissas

O projeto considera inicialmente as seguintes premissas:

1. O prestador possui acesso à internet;
2. O sistema será utilizado principalmente através de navegador;
3. O cliente receberá o orçamento através de um link;
4. O cliente não precisará criar uma conta para visualizar o orçamento;
5. Os pagamentos online serão realizados através de um serviço externo de pagamento;
6. O sistema não armazenará diretamente dados sensíveis de cartão;
7. A empresa poderá escolher sua política de pagamento;
8. O sistema será desenvolvido como uma plataforma multiempresa;
9. Cada empresa deverá acessar somente seus próprios dados.

---

## 1.13 Critérios de Sucesso do MVP

O MVP será considerado funcional quando um prestador conseguir realizar o fluxo completo de um serviço:

```text
Cadastrar empresa
        ↓
Cadastrar cliente
        ↓
Criar orçamento
        ↓
Enviar link
        ↓
Cliente acessa
        ↓
Cliente aprova
        ↓
Pagamento conforme política
        ↓
Agendamento
        ↓
Ordem de Serviço
        ↓
Execução
        ↓
Conclusão
```

O principal objetivo da primeira versão será validar se profissionais realmente utilizam a plataforma para administrar seus serviços.

---

## 1.14 Objetivo de Negócio

O objetivo inicial do projeto é desenvolver e validar uma solução SaaS capaz de gerar valor para profissionais autônomos e pequenas empresas.

Após a validação do produto, o objetivo será transformar a solução em um serviço comercial escalável, permitindo sua utilização por diferentes segmentos de prestação de serviços.

O sucesso do projeto não será medido apenas pela quantidade de funcionalidades desenvolvidas, mas principalmente pela capacidade do sistema de resolver problemas reais dos usuários.


## 1.2 Descrição do Produto



O Autonomo Services é uma plataforma SaaS destinada a profissionais autônomos e pequenas empresas que trabalham com prestação de serviços.



A plataforma tem como objetivo centralizar o gerenciamento de clientes, orçamentos, aprovações, pagamentos, agendamentos e ordens de serviço em um único sistema.



O sistema será desenvolvido inicialmente como uma aplicação web responsiva, permitindo sua utilização em computadores, tablets e dispositivos móveis.



\---



## 1.3 Problema



Profissionais que trabalham com prestação de serviços frequentemente utilizam diferentes ferramentas para administrar suas atividades.



É comum encontrar situações como:



\- clientes controlados principalmente pelo WhatsApp;

\- orçamentos feitos em papel, mensagens ou planilhas;

\- agenda separada do controle dos serviços;

\- pagamentos controlados manualmente;

\- dificuldade para acompanhar orçamentos aprovados;

\- dificuldade para controlar serviços pendentes;

\- falta de histórico organizado dos serviços realizados;

\- risco de executar um serviço sem receber o pagamento;

\- dificuldade para acompanhar vários serviços simultaneamente.



Esses problemas podem resultar em perda de tempo, desorganização, esquecimentos e prejuízos financeiros.



O Autonomo Services busca centralizar essas atividades em uma única plataforma.



\---



## 1.4 Solução Proposta



O Autonomo Services permitirá que o profissional gerencie o ciclo de prestação de serviços desde a criação do orçamento até a conclusão do serviço.



O fluxo principal será:



```text

Prestador

  ↓

Cadastra cliente

  ↓

Cria orçamento

  ↓

Envia link para o cliente

  ↓

Cliente visualiza

  ↓

Cliente aprova ou recusa

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



O cliente poderá acessar o orçamento através de um link público enviado pelo prestador, sem precisar criar uma conta na plataforma.



---



## 1.5 Público-Alvo



O público-alvo inicial será composto por profissionais autônomos e pequenas empresas que realizam serviços externos ou atendimentos sob demanda.



### Exemplos de segmentos



- Eletricistas;

\- Encanadores;

\- Técnicos de ar-condicionado;

\- Vidraceiros;

\- Marceneiros;

\- Instaladores;

\- Técnicos de informática;

\- Assistências técnicas;

\- Empresas de manutenção;

\- Oficinas;

\- Outros profissionais que trabalham com prestação de serviços.



O produto será desenvolvido de forma genérica para que diferentes segmentos possam utilizar o mesmo núcleo da plataforma.



\---



## 1.6 Usuários do Sistema



### Prestador



É o profissional ou empresa que contrata e utiliza o Autonomo Services.



Entre suas principais atividades estarão:



\- cadastrar clientes;

\- criar orçamentos;

\- enviar orçamentos;

\- acompanhar aprovações;

\- controlar pagamentos;

\- realizar agendamentos;

\- criar ordens de serviço;

\- acompanhar serviços;

\- finalizar serviços;

\- consultar histórico.



### Cliente



É a pessoa que recebe um orçamento enviado pelo prestador.



O cliente poderá:



\- acessar o orçamento através do link;

\- visualizar os serviços e valores;

\- aprovar o orçamento;

\- recusar o orçamento;

\- realizar o pagamento quando aplicável;

\- consultar informações relacionadas ao serviço.



O cliente não precisará criar uma conta na plataforma para acessar o orçamento.



\---



## 1.7 Proposta de Valor



O Autonomo Services busca oferecer ao profissional uma maneira simples de administrar seus serviços desde o orçamento até o pagamento e execução.



A proposta central do produto é:



> **"Gerencie seus serviços desde o orçamento até o pagamento e execução em um único lugar."**



A plataforma também busca reduzir o risco financeiro do prestador ao permitir diferentes políticas de pagamento.



\---



## 1.8 Políticas de Pagamento



Cada empresa poderá definir como deseja receber pelos serviços.



### 1.8.1 Pagamento 100% antecipado



Fluxo:



```text

Aprovação

&#x20;  ↓

Pagamento

&#x20;  ↓

Agendamento

&#x20;  ↓

Execução

```



Nesse modelo, o serviço somente poderá avançar para o agendamento após a confirmação do pagamento.



### 1.8.2 Pagamento com sinal



Fluxo:



```text

Aprovação

&#x20;  ↓

Pagamento da entrada

&#x20;  ↓

Agendamento

&#x20;  ↓

Execução

&#x20;  ↓

Pagamento do restante

```



Nesse modelo, o prestador recebe uma entrada antes da execução e o restante será pago conforme as condições definidas pela empresa.



### 1.8.3 Pagamento após o serviço



Fluxo:



```text

Aprovação

&#x20;  ↓

Agendamento

&#x20;  ↓

Execução

&#x20;  ↓

Pagamento

```



Nesse modelo, o pagamento será realizado após a execução do serviço.



\---



## 1.9 Escopo do MVP



O MVP terá como objetivo validar o fluxo principal de gestão de serviços.



### Empresa e autenticação



\- Cadastro da empresa;

\- Cadastro do usuário administrador;

\- Login;

\- Configurações básicas da empresa.



### Clientes



\- Cadastro;

\- Edição;

\- Consulta;

\- Histórico.



### Orçamentos



\- Criação;

\- Edição;

\- Itens;

\- Valores;

\- Descontos;

\- Validade;

\- Status;

\- Link público.



### Aprovação



\- Visualização pelo cliente;

\- Aprovação;

\- Recusa;

\- Registro da ação.



### Pagamentos



\- Definição da política de pagamento;

\- Controle de entrada;

\- Controle do saldo;

\- Status do pagamento;

\- Registro do pagamento.



### Agenda



\- Agendamento;

\- Data;

\- Horário;

\- Cliente;

\- Serviço;

\- Endereço;

\- Status.



### Ordem de Serviço



\- Criação;

\- Informações do serviço;

\- Observações;

\- Fotos;

\- Materiais utilizados;

\- Status;

\- Conclusão.



### Dashboard



\- Resumo dos orçamentos;

\- Resumo dos pagamentos;

\- Próximos agendamentos;

\- Serviços em andamento;

\- Serviços concluídos.



\---



## 1.10 Fora do Escopo do MVP



As funcionalidades abaixo não farão parte da primeira versão:



\- Aplicativo mobile nativo;

\- Integração automática com WhatsApp;

\- Controle avançado de estoque;

\- Gestão de fornecedores;

\- Gestão avançada de equipes;

\- Comissões;

\- Financeiro avançado;

\- Gestão específica de oficinas;

\- Gestão de veículos;

\- Controle avançado de peças;

\- Emissão de documentos fiscais;

\- Contabilidade;

\- Inteligência Artificial;

\- Marketplace de prestadores;

\- Sistema de busca pública de profissionais.



Essas funcionalidades poderão ser avaliadas após a validação do MVP.



\---



## 1.11 Visão de Evolução do Produto



Após a validação do MVP, o Autonomo Services poderá evoluir para uma plataforma modular de gestão empresarial.



Possíveis módulos futuros:



```text

Autonomo Services

│

├── Gestão de Serviços

├── Orçamentos

├── Ordens de Serviço

├── Pagamentos

├── Agenda

├── Clientes

├── WhatsApp

├── Estoque

├── Fornecedores

├── Equipes

├── Financeiro

├── Oficina

└── Inteligência Artificial

```



A arquitetura do sistema deverá permitir a inclusão de novos módulos sem comprometer o funcionamento do núcleo existente.



\---



## 1.12 Premissas



O projeto considera inicialmente as seguintes premissas:



1\. O prestador possui acesso à internet;

2\. O sistema será utilizado principalmente através de navegador;

3\. O cliente receberá o orçamento através de um link;

4\. O cliente não precisará criar uma conta para visualizar o orçamento;

5\. Os pagamentos online serão realizados através de um serviço externo de pagamento;

6\. O sistema não armazenará diretamente dados sensíveis de cartão;

7\. A empresa poderá escolher sua política de pagamento;

8\. O sistema será desenvolvido como uma plataforma multiempresa;

9\. Cada empresa deverá acessar somente seus próprios dados.



\---



## 1.13 Critérios de Sucesso do MVP



O MVP será considerado funcional quando um prestador conseguir realizar o fluxo completo de um serviço:



```text

Cadastrar empresa

&#x20;      ↓

Cadastrar cliente

&#x20;      ↓

Criar orçamento

&#x20;      ↓

Enviar link

&#x20;      ↓

Cliente acessa

&#x20;      ↓

Cliente aprova

&#x20;      ↓

Pagamento conforme política

&#x20;      ↓

Agendamento

&#x20;      ↓

Ordem de Serviço

&#x20;      ↓

Execução

&#x20;      ↓

Conclusão

```



O principal objetivo da primeira versão será validar se profissionais realmente utilizam a plataforma para administrar seus serviços.



\---



## 1.14 Objetivo de Negócio



O objetivo inicial do projeto é desenvolver e validar uma solução SaaS capaz de gerar valor para profissionais autônomos e pequenas empresas.



Após a validação do produto, o objetivo será transformar a solução em um serviço comercial escalável, permitindo sua utilização por diferentes segmentos de prestação de serviços.



O sucesso do projeto não será medido apenas pela quantidade de funcionalidades desenvolvidas, mas principalmente pela capacidade do sistema de resolver problemas reais dos usuários.









