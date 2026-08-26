# 3. Regras de Negócio

## 3.1 Objetivo

As regras de negócio definem as condições, restrições e comportamentos que deverão ser respeitados pelo Autonomo Services durante a execução de suas funcionalidades.

As regras descritas neste documento deverão orientar a implementação dos casos de uso, fluxos, modelo de domínio, banco de dados e API da plataforma.

---

# 3.2 Identificação das Regras

As regras de negócio serão identificadas utilizando o padrão:

**RN-XXX**

Onde:

- **RN** significa Regra de Negócio;
- **XXX** representa o número sequencial da regra.

---

# 3.3 Empresa e Isolamento de Dados

## RN-001 — Isolamento entre empresas

Cada empresa deverá possuir seus próprios dados dentro da plataforma.

Uma empresa não poderá visualizar, alterar ou excluir informações pertencentes a outra empresa.

---

## RN-002 — Associação dos registros à empresa

Os principais registros do sistema deverão estar associados à empresa responsável por eles.

Exemplos:

- usuários;
- clientes;
- orçamentos;
- itens de orçamento;
- pagamentos;
- agendamentos;
- ordens de serviço.

---

## RN-003 — Acesso aos dados

Um usuário somente poderá acessar informações pertencentes à empresa à qual está associado, respeitando suas permissões.

---

## RN-004 — Exclusão de dados

A exclusão de registros deverá respeitar as dependências existentes entre os dados e não deverá provocar inconsistências no histórico da empresa.

---

# 3.4 Clientes

## RN-005 — Cadastro de cliente

Um cliente deverá estar associado a uma empresa antes de ser utilizado em um orçamento ou serviço.

---

## RN-006 — Identificação do cliente

O sistema deverá permitir identificar o cliente por informações cadastradas pela empresa.

---

## RN-007 — Histórico do cliente

Os serviços, orçamentos e demais registros relacionados ao cliente deverão permanecer associados ao seu histórico.

---

# 3.5 Orçamentos

## RN-008 — Criação de orçamento

Um orçamento deverá estar associado obrigatoriamente a:

- uma empresa;
- um cliente;
- um responsável pela criação;
- pelo menos um item ou descrição de serviço;
- um valor.

---

## RN-009 — Identificação do orçamento

Cada orçamento deverá possuir uma identificação única dentro do sistema.

---

## RN-010 — Status do orçamento

O orçamento deverá possuir um status que represente sua situação atual.

Os principais status serão:

- Rascunho;
- Enviado;
- Visualizado;
- Aguardando aprovação;
- Aprovado;
- Recusado;
- Expirado;
- Cancelado.

---

## RN-011 — Link público

O sistema poderá gerar um link público para que o cliente visualize o orçamento sem necessidade de possuir uma conta na plataforma.

---

## RN-012 — Segurança do link público

O link público deverá utilizar um identificador ou mecanismo que impeça a descoberta simples de outros orçamentos.

---

## RN-013 — Alteração do orçamento

Um orçamento já aprovado não deverá ser alterado livremente.

Caso seja necessário modificar valores, itens ou condições relevantes após a aprovação, deverá ser necessário um novo processo de aprovação.

---

# 3.6 Aprovação do Orçamento

## RN-014 — Aprovação pelo cliente

O cliente poderá aprovar ou recusar um orçamento através do link público disponibilizado pela empresa.

---

## RN-015 — Registro da aprovação

Quando o cliente aprovar um orçamento, o sistema deverá registrar a aprovação e atualizar o status do orçamento.

---

## RN-016 — Registro da recusa

Quando o cliente recusar um orçamento, o sistema deverá registrar a recusa e atualizar o status do orçamento.

---

## RN-017 — Orçamento aprovado

A aprovação do orçamento não deverá ser considerada, por si só, como autorização para execução do serviço.

A continuidade do processo deverá respeitar a política de pagamento definida pela empresa.

---

# 3.7 Políticas de Pagamento

Cada empresa poderá definir uma política de pagamento para determinar em qual momento o pagamento deverá ocorrer em relação à execução do serviço.

O sistema deverá suportar três políticas principais.

---

## RN-018 — Política 100% antecipado

Na política de pagamento 100% antecipado, o fluxo deverá seguir:

**Aprovação → Pagamento → Agendamento → Serviço**

O serviço somente poderá avançar para o agendamento após a confirmação do pagamento integral.

---

## RN-019 — Política de pagamento com sinal

Na política de pagamento com sinal, o fluxo deverá seguir:

**Aprovação → Entrada → Agendamento → Serviço → Pagamento do restante**

O serviço poderá ser agendado após a confirmação do pagamento da entrada definida pela empresa.

O valor restante deverá permanecer registrado como pendente até sua quitação.

---

## RN-020 — Política de pagamento após o serviço

Na política de pagamento após o serviço, o fluxo deverá seguir:

**Aprovação → Agendamento → Serviço → Pagamento**

O serviço poderá ser agendado após a aprovação do orçamento.

O pagamento será realizado após a execução do serviço.

---

## RN-021 — Política definida pela empresa

Cada empresa deverá possuir uma política de pagamento configurada para seus serviços.

---

## RN-022 — Alteração da política de pagamento

A alteração da política de pagamento da empresa não deverá modificar automaticamente as condições de orçamentos já enviados ou aprovados.

---

## RN-023 — Pagamento integral

Quando a política exigir pagamento integral antecipado, o orçamento somente poderá avançar para o agendamento após confirmação do valor total.

---

## RN-024 — Pagamento de entrada

Quando a política utilizar sinal, o sistema deverá registrar:

- valor total;
- valor da entrada;
- valor restante;
- situação de cada pagamento.

---

## RN-025 — Pagamento pendente

Um pagamento pendente deverá permanecer identificado até que seja confirmado, cancelado ou tratado conforme as regras financeiras da plataforma.

---

## RN-026 — Confirmação de pagamento

O pagamento somente deverá ser considerado confirmado após o sistema receber uma confirmação válida do meio de pagamento utilizado.

---

# 3.8 Agendamento

## RN-027 — Agendamento após aprovação

Um serviço somente poderá ser agendado após o orçamento ser aprovado.

---

## RN-028 — Restrição conforme política de pagamento

Quando a política de pagamento exigir pagamento antecipado ou entrada, o agendamento somente poderá ocorrer após a confirmação do pagamento mínimo exigido.

---

## RN-029 — Dados do agendamento

O agendamento deverá possuir, no mínimo:

- cliente;
- serviço;
- data;
- horário;
- empresa responsável;
- status do agendamento.

---

## RN-030 — Conflito de horário

O sistema deverá impedir ou alertar sobre conflitos de horário quando houver incompatibilidade entre agendamentos de um mesmo responsável ou recurso.

---

## RN-031 — Alteração do agendamento

A empresa poderá alterar um agendamento de acordo com as permissões disponíveis.

A alteração deverá preservar o histórico necessário para rastreabilidade.

---

## RN-032 — Cancelamento do agendamento

Um agendamento poderá ser cancelado de acordo com as condições estabelecidas pela empresa e pelo estado atual do serviço.

---

# 3.9 Ordem de Serviço

## RN-033 — Criação da ordem de serviço

Uma ordem de serviço deverá ser criada a partir de um serviço aprovado e agendado.

---

## RN-034 — Associação da ordem de serviço

A ordem de serviço deverá estar relacionada a:

- empresa;
- cliente;
- orçamento;
- serviço;
- agendamento;
- responsável pela execução.

---

## RN-035 — Status da ordem de serviço

A ordem de serviço deverá possuir um status para representar sua situação.

Os principais status poderão incluir:

- Aberta;
- Agendada;
- Em execução;
- Pausada;
- Concluída;
- Cancelada.

---

## RN-036 — Execução do serviço

A ordem de serviço deverá permitir registrar informações relacionadas à execução do serviço.

---

## RN-037 — Conclusão do serviço

Uma ordem de serviço somente poderá ser marcada como concluída após o registro das informações necessárias para sua finalização.

---

## RN-038 — Histórico da ordem de serviço

As alterações relevantes da ordem de serviço deverão ser registradas para permitir rastreabilidade.

---

# 3.10 Relação entre Orçamento, Pagamento, Agendamento e Serviço

## RN-039 — Sequência do processo

O sistema deverá respeitar a sequência lógica do ciclo do serviço:

**Cliente → Orçamento → Aprovação → Pagamento conforme política → Agendamento → Ordem de Serviço → Execução → Conclusão**

---

## RN-040 — Impedimento de execução

A execução do serviço deverá respeitar as condições definidas pela política de pagamento da empresa.

---

## RN-041 — Serviço não aprovado

Um serviço cujo orçamento tenha sido recusado, cancelado ou expirado não poderá ser executado através do fluxo normal da plataforma.

---

## RN-042 — Serviço cancelado

Um serviço cancelado não deverá permanecer disponível para execução como se estivesse ativo.

---

# 3.11 Status e Transições

## RN-043 — Transição de status

As mudanças de status deverão respeitar as regras definidas para cada entidade.

O sistema não deverá permitir transições incompatíveis com o estado atual do registro.

---

## RN-044 — Histórico de status

As alterações importantes de status deverão poder ser rastreadas para permitir identificar a evolução do processo.

---

# 3.12 Valores e Pagamentos

## RN-045 — Valor total do orçamento

O valor total do orçamento deverá ser calculado a partir dos itens e demais valores aplicáveis.

---

## RN-046 — Consistência dos valores

Os valores registrados no orçamento e nos pagamentos deverão permanecer consistentes.

---

## RN-047 — Valor restante

Quando houver pagamento parcial, o sistema deverá calcular ou registrar o valor restante necessário para quitação do orçamento.

---

# 3.13 Cancelamentos

## RN-048 — Cancelamento de orçamento

Um orçamento poderá ser cancelado conforme suas condições atuais e as permissões do usuário.

---

## RN-049 — Cancelamento de serviço

Um serviço poderá ser cancelado de acordo com as regras e condições definidas pela empresa.

---

## RN-050 — Histórico de cancelamento

Cancelamentos relevantes deverão manter informações suficientes para identificar quando e por quem foram realizados.

---

# 3.14 Rastreabilidade

## RN-051 — Identificação das ações

Operações relevantes deverão permitir identificar o usuário ou processo responsável pela ação.

---

## RN-052 — Histórico

O sistema deverá manter histórico suficiente para acompanhar a evolução de:

- orçamento;
- aprovação;
- pagamento;
- agendamento;
- ordem de serviço;
- conclusão.

---

# 3.15 Princípios Gerais do Fluxo

## RN-053 — Aprovação não significa pagamento

A aprovação do orçamento deverá ser tratada separadamente da confirmação do pagamento.

---

## RN-054 — Pagamento não significa conclusão

A confirmação do pagamento não deverá marcar automaticamente o serviço como concluído.

A conclusão dependerá da execução do serviço e do encerramento da ordem de serviço.

---

## RN-055 — Agendamento não significa execução

Um serviço agendado ainda não deverá ser considerado executado.

---

## RN-056 — Ordem de serviço representa execução

A ordem de serviço deverá representar o processo operacional de execução do serviço.

---

## RN-057 — Conclusão do ciclo

O ciclo completo deverá permitir identificar claramente quando um serviço:

- foi solicitado;
- recebeu orçamento;
- foi aprovado;
- teve pagamento realizado ou ficou pendente conforme a política;
- foi agendado;
- foi executado;
- foi concluído.

---

# 3.16 Resumo das principais regras

As principais regras de negócio do Autonomo Services podem ser representadas pelo seguinte fluxo:

```text
Cliente
   ↓
Orçamento
   ↓
Aprovação
   ↓
Política de pagamento
   │
   ├── 100% antecipado
   │       ↓
   │    Pagamento
   │       ↓
   │    Agendamento
   │
   ├── Sinal
   │       ↓
   │    Entrada
   │       ↓
   │    Agendamento
   │       ↓
   │    Serviço
   │       ↓
   │    Restante
   │
   └── Após serviço
           ↓
       Agendamento
           ↓
        Serviço
           ↓
       Pagamento

          ↓
    Ordem de Serviço
          ↓
       Execução
          ↓
       Conclusão
