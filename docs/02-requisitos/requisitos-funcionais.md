\# 2. Requisitos Funcionais



\## 2.1 Objetivo



Este documento especifica os requisitos funcionais do Autonomo Services.



Os requisitos funcionais descrevem as funcionalidades que o sistema deverá disponibilizar aos seus usuários.



Os requisitos serão organizados de acordo com os módulos definidos para o MVP.



\### Módulos



1\. Empresa e Usuários

2\. Clientes

3\. Orçamentos

4\. Cliente e Aprovação

5\. Pagamentos

6\. Agenda

7\. Ordem de Serviço

8\. Dashboard



\---



\# Módulo 1 — Empresa e Usuários



\## RF-001 — Cadastrar empresa



\*\*Descrição:\*\*  

O sistema deve permitir que um usuário cadastre uma empresa na plataforma.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário deve estar acessando a plataforma e ainda não possuir uma empresa cadastrada para aquela conta.



\*\*Dados mínimos:\*\*



\- Nome da empresa;

\- Nome do responsável;

\- E-mail;

\- Telefone;

\- CPF ou CNPJ;

\- Endereço.



\*\*Fluxo principal:\*\*



1\. O usuário acessa a opção de cadastro;

2\. O sistema apresenta o formulário de cadastro;

3\. O usuário informa os dados solicitados;

4\. O usuário confirma o cadastro;

5\. O sistema valida os dados;

6\. O sistema registra a empresa;

7\. O sistema associa o usuário à empresa;

8\. O sistema apresenta uma confirmação de cadastro.



\*\*Resultado esperado:\*\*  

A empresa é cadastrada com sucesso e fica disponível para utilização na plataforma.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-002 — Realizar cadastro de usuário



\*\*Descrição:\*\*  

O sistema deve permitir que um usuário crie uma conta para acessar a plataforma.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário ainda não deve possuir uma conta cadastrada com o e-mail informado.



\*\*Dados mínimos:\*\*



\- Nome;

\- E-mail;

\- Senha.



\*\*Fluxo principal:\*\*



1\. O usuário acessa a tela de cadastro;

2\. O sistema apresenta o formulário;

3\. O usuário informa seus dados;

4\. O usuário confirma o cadastro;

5\. O sistema valida os dados;

6\. O sistema verifica se o e-mail já está cadastrado;

7\. O sistema cria a conta;

8\. O sistema informa que o cadastro foi realizado.



\*\*Resultado esperado:\*\*  

A conta do usuário é criada com sucesso.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-003 — Realizar login



\*\*Descrição:\*\*  

O sistema deve permitir que o usuário autenticado acesse sua conta através de e-mail e senha.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário deve possuir uma conta cadastrada.



\*\*Fluxo principal:\*\*



1\. O usuário acessa a tela de login;

2\. O sistema solicita e-mail e senha;

3\. O usuário informa suas credenciais;

4\. O sistema valida as credenciais;

5\. O sistema autentica o usuário;

6\. O sistema direciona o usuário para a área principal da plataforma.



\*\*Fluxo alternativo:\*\*



Caso as credenciais sejam inválidas:



1\. O sistema rejeita a autenticação;

2\. O sistema informa que o e-mail ou senha são inválidos;

3\. O usuário pode tentar novamente.



\*\*Resultado esperado:\*\*  

O usuário acessa somente os recursos permitidos para sua conta.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-004 — Encerrar sessão



\*\*Descrição:\*\*  

O sistema deve permitir que o usuário encerre sua sessão.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário deve estar autenticado.



\*\*Fluxo principal:\*\*



1\. O usuário seleciona a opção de sair;

2\. O sistema encerra a sessão;

3\. O sistema direciona o usuário para a tela de login.



\*\*Resultado esperado:\*\*  

A sessão do usuário é encerrada com segurança.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-005 — Recuperar senha



\*\*Descrição:\*\*  

O sistema deve permitir que o usuário solicite a recuperação de sua senha.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário deve possuir uma conta cadastrada.



\*\*Fluxo principal:\*\*



1\. O usuário acessa a opção "Esqueci minha senha";

2\. O sistema solicita o e-mail cadastrado;

3\. O usuário informa o e-mail;

4\. O sistema verifica a existência da conta;

5\. O sistema envia as instruções de recuperação;

6\. O usuário acessa o mecanismo de recuperação;

7\. O usuário define uma nova senha;

8\. O sistema atualiza a senha.



\*\*Resultado esperado:\*\*  

O usuário consegue recuperar o acesso à sua conta.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-006 — Visualizar perfil



\*\*Descrição:\*\*  

O sistema deve permitir que o usuário visualize seus dados cadastrais.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário deve estar autenticado.



\*\*Fluxo principal:\*\*



1\. O usuário acessa seu perfil;

2\. O sistema consulta seus dados;

3\. O sistema apresenta as informações cadastradas.



\*\*Resultado esperado:\*\*  

Os dados do perfil são apresentados ao usuário.



\*\*Prioridade:\*\*  

Média



\---



\## RF-007 — Editar perfil



\*\*Descrição:\*\*  

O sistema deve permitir que o usuário altere seus dados cadastrais.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário deve estar autenticado.



\*\*Fluxo principal:\*\*



1\. O usuário acessa seu perfil;

2\. O sistema apresenta os dados atuais;

3\. O usuário altera as informações desejadas;

4\. O usuário confirma as alterações;

5\. O sistema valida os dados;

6\. O sistema salva as alterações;

7\. O sistema apresenta uma confirmação.



\*\*Resultado esperado:\*\*  

Os dados do perfil são atualizados.



\*\*Prioridade:\*\*  

Média



\---



\## RF-008 — Visualizar dados da empresa



\*\*Descrição:\*\*  

O sistema deve permitir que o usuário visualize os dados da empresa vinculada à sua conta.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O usuário deve estar autenticado e possuir uma empresa vinculada.



\*\*Fluxo principal:\*\*



1\. O usuário acessa as configurações da empresa;

2\. O sistema consulta os dados da empresa;

3\. O sistema apresenta as informações.



\*\*Resultado esperado:\*\*  

Os dados da empresa são apresentados ao usuário.



\*\*Prioridade:\*\*  

Média



\---



\## RF-009 — Editar dados da empresa



\*\*Descrição:\*\*  

O sistema deve permitir que o usuário autorizado altere os dados da empresa.



\*\*Ator:\*\*  

Administrador da empresa



\*\*Pré-condições:\*\*  

O usuário deve estar autenticado e possuir permissão administrativa.



\*\*Fluxo principal:\*\*



1\. O administrador acessa as configurações da empresa;

2\. O sistema apresenta os dados atuais;

3\. O administrador altera as informações;

4\. O administrador confirma as alterações;

5\. O sistema valida os dados;

6\. O sistema salva as alterações;

7\. O sistema apresenta uma confirmação.



\*\*Resultado esperado:\*\*  

Os dados da empresa são atualizados.



\*\*Prioridade:\*\*  

Média



\---



\## RF-010 — Associar usuário à empresa



\*\*Descrição:\*\*  

O sistema deve permitir que um usuário esteja vinculado a uma empresa.



\*\*Ator:\*\*  

Sistema



\*\*Pré-condições:\*\*  

O usuário e a empresa devem existir.



\*\*Fluxo principal:\*\*



1\. O sistema identifica o usuário;

2\. O sistema identifica a empresa;

3\. O sistema registra o vínculo;

4\. O usuário passa a acessar os dados permitidos da empresa.



\*\*Resultado esperado:\*\*  

O usuário possui um vínculo válido com a empresa.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-011 — Controlar acesso aos dados da empresa



\*\*Descrição:\*\*  

O sistema deve garantir que o usuário tenha acesso somente aos dados das empresas às quais possui vínculo e permissão.



\*\*Ator:\*\*  

Sistema



\*\*Pré-condições:\*\*  

O usuário deve estar autenticado.



\*\*Fluxo principal:\*\*



1\. O usuário solicita um recurso;

2\. O sistema identifica o usuário autenticado;

3\. O sistema identifica a empresa relacionada à solicitação;

4\. O sistema verifica as permissões;

5\. O sistema permite ou bloqueia o acesso conforme as regras definidas.



\*\*Resultado esperado:\*\*  

O usuário não consegue acessar dados de empresas às quais não possui autorização.



\*\*Prioridade:\*\*  

Crítica



\---



\# Resumo do Módulo 1



| Código | Requisito | Prioridade |

|---|---|---|

| RF-001 | Cadastrar empresa | Alta |

| RF-002 | Cadastrar usuário | Alta |

| RF-003 | Realizar login | Alta |

| RF-004 | Encerrar sessão | Alta |

| RF-005 | Recuperar senha | Alta |

| RF-006 | Visualizar perfil | Média |

| RF-007 | Editar perfil | Média |

| RF-008 | Visualizar dados da empresa | Média |

| RF-009 | Editar dados da empresa | Média |

| RF-010 | Associar usuário à empresa | Alta |

| RF-011 | Controlar acesso aos dados da empresa | Crítica |



\---



\# Módulo 2 — Clientes



\## RF-012 — Cadastrar cliente



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador cadastre um cliente.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O prestador deve estar autenticado e possuir uma empresa vinculada.



\*\*Dados mínimos:\*\*



\- Nome;

\- Telefone;

\- E-mail;

\- CPF ou CNPJ;

\- Endereço;

\- Observações.



\*\*Fluxo principal:\*\*



1\. O prestador acessa o módulo de clientes;

2\. Seleciona a opção de cadastrar cliente;

3\. O sistema apresenta o formulário;

4\. O prestador informa os dados;

5\. O prestador confirma o cadastro;

6\. O sistema valida os dados;

7\. O sistema registra o cliente;

8\. O sistema apresenta uma confirmação.



\*\*Resultado esperado:\*\*  

O cliente é cadastrado e fica disponível para utilização nos demais módulos.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-013 — Consultar clientes



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador consulte os clientes cadastrados.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O prestador deve estar autenticado.



\*\*Fluxo principal:\*\*



1\. O prestador acessa o módulo de clientes;

2\. O sistema consulta os clientes vinculados à empresa;

3\. O sistema apresenta a lista de clientes;

4\. O prestador pode pesquisar ou filtrar os registros.



\*\*Resultado esperado:\*\*  

Os clientes da empresa são apresentados ao prestador.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-014 — Visualizar cliente



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador visualize os dados de um cliente específico.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O cliente deve estar cadastrado e vinculado à empresa.



\*\*Fluxo principal:\*\*



1\. O prestador seleciona um cliente;

2\. O sistema consulta os dados;

3\. O sistema apresenta as informações cadastrais;

4\. O sistema apresenta o histórico relacionado ao cliente.



\*\*Resultado esperado:\*\*  

O prestador consegue visualizar as informações e o histórico do cliente.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-015 — Editar cliente



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador altere os dados cadastrais de um cliente.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O cliente deve existir e estar vinculado à empresa.



\*\*Fluxo principal:\*\*



1\. O prestador acessa o cliente;

2\. Seleciona a opção de edição;

3\. O sistema apresenta os dados atuais;

4\. O prestador altera as informações;

5\. O prestador confirma;

6\. O sistema valida os dados;

7\. O sistema salva as alterações.



\*\*Resultado esperado:\*\*  

Os dados do cliente são atualizados.



\*\*Prioridade:\*\*  

Média



\---



\## RF-016 — Consultar histórico do cliente



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador consulte o histórico de serviços relacionados a um cliente.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O cliente deve possuir registros relacionados à empresa.



\*\*Fluxo principal:\*\*



1\. O prestador acessa o cliente;

2\. O sistema consulta os registros relacionados;

3\. O sistema apresenta o histórico;

4\. O prestador pode consultar os serviços, orçamentos e pagamentos relacionados.



\*\*Resultado esperado:\*\*  

O prestador consegue consultar o histórico do relacionamento com o cliente.



\*\*Prioridade:\*\*  

Alta



\---



\# Módulo 3 — Orçamentos



\## RF-017 — Criar orçamento



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador crie um orçamento para um cliente.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O cliente deve estar cadastrado.



\*\*Fluxo principal:\*\*



1\. O prestador seleciona um cliente;

2\. O prestador cria um novo orçamento;

3\. O sistema permite adicionar os itens do serviço;

4\. O prestador informa quantidades e valores;

5\. O sistema calcula o valor total;

6\. O prestador informa a validade do orçamento;

7\. O prestador salva o orçamento;

8\. O sistema registra o orçamento.



\*\*Resultado esperado:\*\*  

Um orçamento é criado e associado ao cliente.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-018 — Adicionar itens ao orçamento



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador adicione serviços, materiais ou outros itens ao orçamento.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O orçamento deve estar em estado editável.



\*\*Fluxo principal:\*\*



1\. O prestador seleciona a opção de adicionar item;

2\. Informa a descrição;

3\. Informa quantidade;

4\. Informa valor unitário;

5\. O sistema calcula o valor do item;

6\. O sistema atualiza o valor total do orçamento.



\*\*Resultado esperado:\*\*  

O item é adicionado ao orçamento e o total é atualizado.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-019 — Gerar link público do orçamento



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador gere um link público para que o cliente possa visualizar o orçamento.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O orçamento deve estar criado.



\*\*Fluxo principal:\*\*



1\. O prestador seleciona o orçamento;

2\. Solicita o link público;

3\. O sistema gera ou recupera um identificador público;

4\. O sistema apresenta o link;

5\. O prestador pode copiar o link para enviá-lo ao cliente.



\*\*Resultado esperado:\*\*  

Um link público válido é disponibilizado para o orçamento.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-020 — Enviar orçamento ao cliente



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador utilize o link público do orçamento para encaminhá-lo ao cliente.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O orçamento deve possuir um link público.



\*\*Fluxo principal:\*\*



1\. O prestador acessa o orçamento;

2\. O sistema apresenta o link;

3\. O prestador copia o link;

4\. O prestador envia o link ao cliente através do canal de comunicação escolhido.



\*\*Resultado esperado:\*\*  

O cliente recebe o acesso ao orçamento.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-021 — Consultar orçamentos



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador consulte os orçamentos cadastrados.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O prestador deve estar autenticado.



\*\*Fluxo principal:\*\*



1\. O prestador acessa o módulo de orçamentos;

2\. O sistema apresenta os orçamentos da empresa;

3\. O prestador pode pesquisar e filtrar os registros;

4\. O sistema apresenta os resultados.



\*\*Resultado esperado:\*\*  

O prestador consegue acompanhar os orçamentos da empresa.



\*\*Prioridade:\*\*  

Alta



\---



\# Módulo 4 — Cliente e Aprovação



\## RF-022 — Visualizar orçamento através de link público



\*\*Descrição:\*\*  

O sistema deve permitir que o cliente visualize um orçamento através do link público recebido do prestador.



\*\*Ator:\*\*  

Cliente



\*\*Pré-condições:\*\*  

O link deve ser válido e o orçamento deve estar disponível para visualização.



\*\*Fluxo principal:\*\*



1\. O cliente acessa o link;

2\. O sistema valida o identificador público;

3\. O sistema apresenta os dados do orçamento;

4\. O cliente visualiza os serviços, valores, condições e validade.



\*\*Resultado esperado:\*\*  

O cliente consegue visualizar o orçamento sem precisar criar uma conta.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-023 — Aprovar orçamento



\*\*Descrição:\*\*  

O sistema deve permitir que o cliente aprove um orçamento.



\*\*Ator:\*\*  

Cliente



\*\*Pré-condições:\*\*  

O orçamento deve estar válido e disponível para aprovação.



\*\*Fluxo principal:\*\*



1\. O cliente acessa o orçamento;

2\. O cliente seleciona a opção de aprovação;

3\. O sistema solicita confirmação;

4\. O cliente confirma a aprovação;

5\. O sistema registra a aprovação;

6\. O sistema altera o status do orçamento;

7\. O sistema direciona o fluxo conforme a política de pagamento definida.



\*\*Resultado esperado:\*\*  

O orçamento é registrado como aprovado.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-024 — Recusar orçamento



\*\*Descrição:\*\*  

O sistema deve permitir que o cliente recuse um orçamento.



\*\*Ator:\*\*  

Cliente



\*\*Pré-condições:\*\*  

O orçamento deve estar disponível para resposta.



\*\*Fluxo principal:\*\*



1\. O cliente acessa o orçamento;

2\. Seleciona a opção de recusar;

3\. O sistema solicita confirmação;

4\. O cliente confirma;

5\. O sistema registra a recusa;

6\. O sistema altera o status do orçamento.



\*\*Resultado esperado:\*\*  

O orçamento é registrado como recusado.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-025 — Registrar resposta do cliente



\*\*Descrição:\*\*  

O sistema deve registrar a ação realizada pelo cliente sobre o orçamento.



\*\*Ator:\*\*  

Sistema



\*\*Pré-condições:\*\*  

O cliente deve realizar uma ação válida sobre o orçamento.



\*\*Fluxo principal:\*\*



1\. O sistema identifica o orçamento;

2\. Identifica a ação realizada;

3\. Registra data e horário;

4\. Atualiza o status do orçamento;

5\. Mantém o registro para consulta futura.



\*\*Resultado esperado:\*\*  

A resposta do cliente fica registrada no histórico do orçamento.



\*\*Prioridade:\*\*  

Alta



\---



\# Módulo 5 — Pagamentos



\## RF-026 — Definir política de pagamento



\*\*Descrição:\*\*  

O sistema deve permitir que a empresa defina a política de pagamento aplicável aos seus serviços.



\*\*Ator:\*\*  

Prestador



\*\*Políticas disponíveis no MVP:\*\*



1\. Pagamento 100% antecipado;

2\. Pagamento com sinal;

3\. Pagamento após o serviço.



\*\*Fluxo principal:\*\*



1\. O prestador acessa as configurações de pagamento;

2\. Seleciona uma política;

3\. O sistema registra a configuração;

4\. A política passa a ser utilizada nos novos orçamentos.



\*\*Resultado esperado:\*\*  

A política de pagamento da empresa é definida.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-027 — Registrar pagamento



\*\*Descrição:\*\*  

O sistema deve registrar o pagamento realizado pelo cliente.



\*\*Ator:\*\*  

Sistema



\*\*Pré-condições:\*\*  

Deve existir um orçamento ou serviço com pagamento previsto.



\*\*Fluxo principal:\*\*



1\. O pagamento é processado pelo meio de pagamento utilizado;

2\. O sistema recebe a confirmação do pagamento;

3\. O sistema identifica o orçamento ou serviço relacionado;

4\. O sistema registra o pagamento;

5\. O sistema atualiza o status financeiro.



\*\*Resultado esperado:\*\*  

O pagamento é registrado corretamente.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-028 — Controlar pagamento de entrada



\*\*Descrição:\*\*  

O sistema deve permitir o controle do pagamento de uma entrada quando a empresa utilizar a política de sinal.



\*\*Ator:\*\*  

Sistema



\*\*Pré-condições:\*\*  

O orçamento deve utilizar a política de pagamento com sinal.



\*\*Fluxo principal:\*\*



1\. O sistema identifica o valor da entrada;

2\. O cliente realiza o pagamento;

3\. O sistema recebe a confirmação;

4\. O sistema registra a entrada;

5\. O sistema calcula o saldo restante;

6\. O sistema atualiza o status do pagamento.



\*\*Resultado esperado:\*\*  

A entrada e o saldo restante ficam registrados.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-029 — Controlar saldo restante



\*\*Descrição:\*\*  

O sistema deve permitir o controle do valor restante após o pagamento parcial.



\*\*Ator:\*\*  

Sistema



\*\*Pré-condições:\*\*  

Deve existir um pagamento parcial registrado.



\*\*Fluxo principal:\*\*



1\. O sistema identifica o valor total;

2\. Identifica os pagamentos realizados;

3\. Calcula o saldo restante;

4\. Apresenta o saldo ao prestador.



\*\*Resultado esperado:\*\*  

O saldo restante é calculado e apresentado corretamente.



\*\*Prioridade:\*\*  

Alta



\---



\# Módulo 6 — Agenda



\## RF-030 — Criar agendamento



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador agende a execução de um serviço.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O orçamento deve estar aprovado e as condições necessárias da política de pagamento devem ter sido atendidas.



\*\*Fluxo principal:\*\*



1\. O prestador seleciona o serviço;

2\. Seleciona a data;

3\. Seleciona o horário;

4\. Confirma o endereço;

5\. Confirma o agendamento;

6\. O sistema registra o agendamento.



\*\*Resultado esperado:\*\*  

O serviço fica agendado.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-031 — Consultar agenda



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador consulte seus serviços agendados.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O prestador deve estar autenticado.



\*\*Fluxo principal:\*\*



1\. O prestador acessa a agenda;

2\. O sistema consulta os agendamentos;

3\. O sistema apresenta os serviços;

4\. O prestador pode visualizar os compromissos por período.



\*\*Resultado esperado:\*\*  

O prestador consegue visualizar sua agenda.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-032 — Alterar agendamento



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador altere um agendamento existente.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O agendamento deve existir e estar em estado que permita alteração.



\*\*Fluxo principal:\*\*



1\. O prestador seleciona o agendamento;

2\. Solicita alteração;

3\. Altera data, horário ou informações permitidas;

4\. Confirma a alteração;

5\. O sistema atualiza o agendamento.



\*\*Resultado esperado:\*\*  

O agendamento é atualizado.



\*\*Prioridade:\*\*  

Média



\---



\## RF-033 — Cancelar agendamento



\*\*Descrição:\*\*  

O sistema deve permitir que um agendamento seja cancelado conforme as regras de negócio.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O agendamento deve existir.



\*\*Fluxo principal:\*\*



1\. O prestador seleciona o agendamento;

2\. Solicita cancelamento;

3\. O sistema solicita confirmação;

4\. O prestador confirma;

5\. O sistema registra o cancelamento;

6\. O sistema atualiza o status.



\*\*Resultado esperado:\*\*  

O agendamento é marcado como cancelado.



\*\*Prioridade:\*\*  

Alta



\---



\# Módulo 7 — Ordem de Serviço



\## RF-034 — Criar ordem de serviço



\*\*Descrição:\*\*  

O sistema deve permitir a criação de uma ordem de serviço a partir de um serviço aprovado e agendado.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

O orçamento deve estar aprovado e o serviço deve estar agendado.



\*\*Fluxo principal:\*\*



1\. O prestador acessa o serviço;

2\. Solicita a criação da ordem de serviço;

3\. O sistema recupera as informações do orçamento;

4\. O sistema cria a ordem de serviço;

5\. O sistema associa a ordem ao cliente e ao serviço.



\*\*Resultado esperado:\*\*  

Uma ordem de serviço é criada.



\*\*Prioridade:\*\*  

Crítica



\---



\## RF-035 — Registrar execução do serviço



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador registre informações relacionadas à execução do serviço.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

A ordem de serviço deve existir.



\*\*Fluxo principal:\*\*



1\. O prestador acessa a ordem de serviço;

2\. Registra informações da execução;

3\. Adiciona observações;

4\. Registra materiais utilizados quando aplicável;

5\. Adiciona fotos quando aplicável;

6\. Salva as informações.



\*\*Resultado esperado:\*\*  

As informações da execução ficam registradas na ordem de serviço.



\*\*Prioridade:\*\*  

Alta



\---



\## RF-036 — Finalizar ordem de serviço



\*\*Descrição:\*\*  

O sistema deve permitir que o prestador finalize uma ordem de serviço.



\*\*Ator:\*\*  

Prestador



\*\*Pré-condições:\*\*  

A ordem de serviço deve estar em execução ou em estado que permita finalização.



\*\*Fluxo principal:\*\*



1\. O prestador acessa a ordem de serviço;

2\. Confirma a conclusão;

3\. O sistema valida as condições necessárias;

4\. O sistema altera o status para concluído;

5\. O sistema registra data e horário da conclusão.



\*\*Resultado esperado:\*\*  

A ordem de serviço é finalizada e permanece disponível no histórico.



\*\*Prioridade:\*\*  

Crítica



\---



\# Módulo 8 — Dashboard



\## RF-037 — Visualizar resumo dos orçamentos



\*\*Descrição:\*\*  

O sistema deve apresentar ao prestador um resumo dos orçamentos da empresa.



\*\*Ator:\*\*  

Prestador



\*\*Informações mínimas:\*\*



\- Orçamentos pendentes;

\- Orçamentos aprovados;

\- Orçamentos recusados;

\- Orçamentos expirados.



\*\*Resultado esperado:\*\*  

O prestador consegue visualizar rapidamente a situação dos seus orçamentos.



\*\*Prioridade:\*\*  

Média



\---



\## RF-038 — Visualizar resumo dos pagamentos



\*\*Descrição:\*\*  

O sistema deve apresentar um resumo dos pagamentos relacionados aos serviços.



\*\*Ator:\*\*  

Prestador



\*\*Informações mínimas:\*\*



\- Pagamentos recebidos;

\- Pagamentos pendentes;

\- Entradas recebidas;

\- Saldos restantes.



\*\*Resultado esperado:\*\*  

O prestador consegue visualizar a situação dos pagamentos.



\*\*Prioridade:\*\*  

Média



\---



\## RF-039 — Visualizar próximos agendamentos



\*\*Descrição:\*\*  

O sistema deve apresentar os próximos serviços agendados.



\*\*Ator:\*\*  

Prestador



\*\*Resultado esperado:\*\*  

O prestador consegue visualizar rapidamente seus próximos compromissos.



\*\*Prioridade:\*\*  

Média



\---



\## RF-040 — Visualizar serviços em andamento



\*\*Descrição:\*\*  

O sistema deve apresentar os serviços que estão atualmente em execução.



\*\*Ator:\*\*  

Prestador



\*\*Resultado esperado:\*\*  

O prestador consegue acompanhar os serviços em andamento.



\*\*Prioridade:\*\*  

Média



\---



\## RF-041 — Visualizar serviços concluídos



\*\*Descrição:\*\*  

O sistema deve apresentar os serviços concluídos pela empresa.



\*\*Ator:\*\*  

Prestador



\*\*Resultado esperado:\*\*  

O prestador consegue consultar os serviços finalizados.



\*\*Prioridade:\*\*  

Média



\---



\# Resumo geral dos requisitos funcionais



| Módulo | Requisitos |

|---|---|

| Empresa e Usuários | RF-001 a RF-011 |

| Clientes | RF-012 a RF-016 |

| Orçamentos | RF-017 a RF-021 |

| Cliente e Aprovação | RF-022 a RF-025 |

| Pagamentos | RF-026 a RF-029 |

| Agenda | RF-030 a RF-033 |

| Ordem de Serviço | RF-034 a RF-036 |

| Dashboard | RF-037 a RF-041 |



\*\*Total inicial:\*\* 41 requisitos funcionais.

