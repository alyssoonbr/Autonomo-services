# 2. Requisitos Não Funcionais

## 2.1 Objetivo

Os requisitos não funcionais definem as características, restrições e padrões de qualidade que o Autonomo Services deverá atender.

Enquanto os requisitos funcionais descrevem **o que o sistema deve fazer**, os requisitos não funcionais descrevem **como o sistema deve funcionar**.

Os requisitos serão organizados de acordo com os principais aspectos técnicos e de qualidade do sistema.

---

# 2.2 Desempenho

## RNF-001 — Tempo de resposta

O sistema deverá apresentar tempo de resposta adequado nas operações realizadas pelos usuários.

As operações comuns, como consultas, cadastro de clientes, criação de orçamentos e acesso ao dashboard, deverão apresentar resposta preferencialmente inferior a 2 segundos em condições normais de utilização.

---

## RNF-002 — Processamento de operações

O sistema deverá processar operações de forma eficiente, evitando processamento desnecessário que possa comprometer a experiência do usuário.

---

## RNF-003 — Carregamento das páginas

As páginas da aplicação deverão ser desenvolvidas visando reduzir o tempo de carregamento e melhorar a experiência do usuário.

---

# 2.3 Segurança

## RNF-004 — Autenticação

O sistema deverá possuir mecanismo seguro de autenticação para permitir o acesso somente a usuários autorizados.

---

## RNF-005 — Senhas

As senhas dos usuários não deverão ser armazenadas em texto puro.

As credenciais deverão utilizar mecanismos adequados de hash e proteção.

---

## RNF-006 — Controle de acesso

O sistema deverá controlar o acesso às funcionalidades de acordo com o perfil e as permissões do usuário.

---

## RNF-007 — Isolamento dos dados

Os dados de uma empresa deverão permanecer isolados dos dados pertencentes a outras empresas.

Um usuário de uma empresa não deverá conseguir acessar informações pertencentes a outra empresa sem autorização.

---

## RNF-008 — Proteção de dados

O sistema deverá adotar mecanismos para proteger dados de clientes, empresas, usuários, orçamentos, pagamentos e ordens de serviço contra acessos não autorizados.

---

## RNF-009 — Comunicação segura

A comunicação entre cliente, aplicação e serviços externos deverá utilizar protocolos seguros de comunicação.

---

# 2.4 Disponibilidade

## RNF-010 — Disponibilidade do sistema

O sistema deverá permanecer disponível durante os períodos previstos para utilização pelos usuários.

---

## RNF-011 — Tratamento de falhas

O sistema deverá tratar falhas de forma controlada, evitando interrupções desnecessárias e apresentando mensagens adequadas ao usuário.

---

## RNF-012 — Recuperação

O sistema deverá possuir mecanismos que permitam a recuperação das informações em situações de falha.

---

# 2.5 Escalabilidade

## RNF-013 — Crescimento de usuários

A arquitetura deverá permitir o crescimento do número de empresas e usuários sem exigir uma reestruturação completa do sistema.

---

## RNF-014 — Crescimento de dados

O sistema deverá ser projetado considerando o crescimento gradual da quantidade de clientes, orçamentos, pagamentos, agendamentos e ordens de serviço armazenados.

---

## RNF-015 — Expansão de módulos

A arquitetura deverá permitir a inclusão de novos módulos e funcionalidades sem comprometer os módulos existentes.

---

# 2.6 Usabilidade

## RNF-016 — Interface intuitiva

A interface deverá ser simples e intuitiva, permitindo que profissionais com diferentes níveis de conhecimento tecnológico utilizem o sistema.

---

## RNF-017 — Responsividade

A aplicação deverá possuir interface responsiva, permitindo sua utilização em computadores, tablets e dispositivos móveis.

---

## RNF-018 — Feedback das operações

O sistema deverá informar ao usuário o resultado das operações realizadas.

Exemplos:

- cadastro realizado com sucesso;
- orçamento criado;
- pagamento confirmado;
- agendamento realizado;
- erro durante uma operação.

---

## RNF-019 — Mensagens de erro

As mensagens de erro deverão ser claras e compreensíveis, evitando apresentar informações técnicas desnecessárias ao usuário final.

---

# 2.7 Manutenibilidade

## RNF-020 — Organização do código

O código deverá ser organizado de forma modular, seguindo padrões que facilitem manutenção e evolução do sistema.

---

## RNF-021 — Separação de responsabilidades

Os componentes do sistema deverão possuir responsabilidades bem definidas, evitando concentração excessiva de regras em uma única parte da aplicação.

---

## RNF-022 — Documentação técnica

As principais decisões técnicas e arquiteturais do sistema deverão ser documentadas.

---

## RNF-023 — Testabilidade

A arquitetura deverá permitir a criação e execução de testes automatizados para as principais funcionalidades do sistema.

---

# 2.8 Compatibilidade

## RNF-024 — Navegadores

A aplicação deverá funcionar nos principais navegadores modernos utilizados pelos usuários.

---

## RNF-025 — Dispositivos

A interface deverá adaptar-se a diferentes tamanhos de tela e dispositivos.

---

# 2.9 Banco de Dados e Integridade

## RNF-026 — Integridade dos dados

O sistema deverá garantir a integridade dos dados armazenados no banco de dados.

---

## RNF-027 — Consistência

As operações que alteram informações relacionadas deverão manter os dados consistentes.

---

## RNF-028 — Backup

O ambiente de produção deverá possuir mecanismos de backup periódico dos dados.

---

## RNF-029 — Recuperação de dados

Deverá existir um procedimento para recuperação dos dados a partir dos backups disponíveis em caso de falha.

---

# 2.10 Auditoria e Rastreabilidade

## RNF-030 — Registro de operações importantes

O sistema deverá registrar operações relevantes realizadas pelos usuários.

Exemplos:

- criação de orçamento;
- alteração de orçamento;
- aprovação;
- recusa;
- registro de pagamento;
- alteração de agendamento;
- alteração de ordem de serviço.

---

## RNF-031 — Identificação do usuário

Quando aplicável, operações importantes deverão permitir identificar o usuário responsável pela ação.

---

## RNF-032 — Histórico

O sistema deverá manter histórico das principais alterações realizadas nos registros relevantes.

---

# 2.11 Integrações

## RNF-033 — Integração com serviços externos

A arquitetura deverá permitir integração com serviços externos utilizados pela plataforma.

Exemplos:

- gateways de pagamento;
- serviços de envio de mensagens;
- serviços de e-mail;
- serviços de armazenamento;
- APIs externas.

---

## RNF-034 — Tratamento de falhas de integração

Falhas em serviços externos deverão ser tratadas de forma controlada, evitando inconsistências nos dados internos da plataforma.

---

# 2.12 Segurança e Privacidade

## RNF-035 — Princípio do menor privilégio

Os usuários deverão possuir somente as permissões necessárias para executar suas atividades dentro do sistema.

---

## RNF-036 — Proteção de informações sensíveis

Informações sensíveis deverão receber mecanismos adicionais de proteção conforme sua natureza.

---

## RNF-037 — Sessões de usuário

O sistema deverá possuir mecanismos para controlar sessões autenticadas e impedir acessos indevidos.

---

# 2.13 Arquitetura e Evolução

## RNF-038 — Arquitetura modular

A arquitetura deverá permitir evolução independente dos principais módulos da aplicação sempre que tecnicamente viável.

---

## RNF-039 — Separação entre apresentação e regras de negócio

A aplicação deverá manter separadas as responsabilidades relacionadas à interface, regras de negócio, persistência e integração.

---

## RNF-040 — Extensibilidade

O sistema deverá ser projetado de forma que novos segmentos de negócio possam ser adicionados futuramente sem necessidade de reconstrução completa da plataforma.

---

## RNF-041 — Evolução tecnológica

A arquitetura deverá permitir a evolução das tecnologias utilizadas sem comprometer as regras de negócio e os dados existentes.

---

# 2.14 Resumo

Os requisitos não funcionais estabelecem os principais critérios de qualidade e restrições técnicas do Autonomo Services.

Eles deverão orientar as decisões relacionadas à arquitetura, segurança, banco de dados, API, infraestrutura e implementação do sistema.

**Total inicial:** 41 requisitos não funcionais.
