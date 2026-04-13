# RFC-001 — PrazoCerto

| Campo        | Valor                                      |
|--------------|---------------------------------------------|
| RFC          | RFC-001                                     |
| Status       | Rascunho                                    |
| Versão       | 0.1.0                                       |
| Data         | Abril / 2026                                |
| Autor        | Seu Nome                                    |
| Curso        | Engenharia de Software                      |
| Disciplina   | PAC VII                                     |
| Categoria    | Web App / Sistema de Gestão Comercial       |
| Repositório  | https://github.com/seu-usuario/prazocerto   |

Sumário
Problema Identificado
Oportunidade
Proposta de Solução
Justificativa
Alternativas Consideradas
Resultados Esperados
Questões em Aberto
1. Problema Identificado

No contexto de pequenos comerciantes e trabalhadores autônomos que realizam vendas a prazo, o controle das transações e dos recebimentos é frequentemente realizado de forma manual, utilizando cadernos físicos, anotações informais ou registros dispersos em aplicativos de mensagens.

Esse modelo de controle apresenta limitações críticas, tais como:

dificuldade no acompanhamento de clientes inadimplentes;
ausência de organização estruturada das informações;
risco de esquecimento de cobranças;
falta de histórico consolidado de transações;
perda de receita devido à desorganização operacional.

A inexistência de uma ferramenta digital simples e acessível que centralize essas informações torna o processo de gestão reativo, ineficiente e suscetível a falhas humanas.

2. Oportunidade

Existe a oportunidade de desenvolver uma plataforma digital voltada à gestão de vendas a prazo, com foco na simplicidade e na eficiência operacional, permitindo:

Organização: centralização de clientes e transações em um único sistema;
Controle: acompanhamento estruturado de vencimentos e pagamentos;
Agilidade: redução do tempo gasto em consultas e registros manuais;
Automação: apoio ao processo de cobrança com geração de lembretes;
Visibilidade: acesso a indicadores operacionais por meio de dashboards.

Essa solução contribui diretamente para a profissionalização da gestão de pequenos negócios informais.

3. Proposta de Solução

Desenvolver o PrazoCerto, um sistema web de gestão de vendas a prazo composto por três componentes principais:

[ Interface Web ] ──API──► [ Servidor de Gestão ] ──Integração──► [ Comunicação com Cliente ]
3.1 Interface Web (Frontend)

Módulo responsável pela interação com o usuário. Responsável por:

permitir o cadastro e gestão de clientes;
registrar vendas a prazo com valor e vencimento;
exibir lista de cobranças pendentes;
apresentar histórico de transações por cliente;
disponibilizar dashboards com indicadores de desempenho.
3.2 Servidor de Gestão (Backend)

Serviço central responsável pelas regras de negócio. Responsável por:

processar e validar transações;
gerenciar clientes e registros financeiros;
controlar o status de pagamentos;
armazenar dados em banco persistente;
disponibilizar uma API REST segura para o frontend.
3.3 Orquestrador de Comunicação

Módulo responsável por apoiar o processo de cobrança. Responsável por:

gerar mensagens estruturadas de lembrete;
permitir integração com WhatsApp para contato com clientes;
padronizar a comunicação de cobrança.
4. Justificativa

A proposta justifica-se pela necessidade de digitalizar e estruturar o processo de controle de vendas a prazo em pequenos negócios.

As soluções disponíveis no mercado apresentam limitações relevantes:

sistemas financeiros completos são complexos para o público-alvo;
ferramentas genéricas não atendem o contexto informal de vendas;
métodos manuais são suscetíveis a erros e perda de informações.

O projeto permite a aplicação prática de conceitos essenciais de Engenharia de Software, incluindo:

modelagem de dados relacionais (clientes e transações);
desenvolvimento de APIs RESTful com foco em segurança e escalabilidade;
aplicação de testes automatizados (TDD);
implementação de pipelines de integração contínua (CI/CD);
construção de interfaces centradas na experiência do usuário.
5. Alternativas Consideradas
Alternativa	Motivo do descarte
Caderno físico	Alta suscetibilidade a erros e perda de dados
Planilhas (Excel)	Baixa usabilidade em dispositivos móveis e pouca automação
Aplicativos financeiros genéricos	Complexidade excessiva para o público-alvo
Aplicações de notas	Falta de estrutura e controle de dados

Escolha adotada: desenvolvimento de uma aplicação web dedicada, com foco na simplicidade, autonomia do usuário e adequação ao contexto de pequenos comerciantes.

6. Resultados Esperados

Ao final do projeto, espera-se entregar:

um sistema web funcional para gestão de vendas a prazo;
centralização das informações de clientes e transações;
redução significativa de erros operacionais;
melhoria no controle de cobranças e vencimentos;
dashboards com indicadores básicos de desempenho;
documentação técnica estruturada e alinhada às boas práticas.
7. Questões em Aberto
Qual será a melhor estratégia de autenticação (JWT, sessão, OAuth)?
A integração com WhatsApp será realizada via link direto ou API oficial?
O sistema deverá suportar múltiplos usuários ou apenas uso individual?
Haverá necessidade de exportação de dados (PDF/CSV)?
O sistema deverá funcionar offline ou apenas online?
