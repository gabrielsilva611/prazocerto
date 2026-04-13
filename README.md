# PRAZOCERTO
    DESCRIÇÃO
  O PrazoCerto é um sistema web desenvolvido para auxiliar pequenos comerciantes e trabalhadores autônomos na gestão de vendas a prazo e no acompanhamento de recebimentos.
  A aplicação centraliza o controle de clientes, transações e vencimentos, substituindo métodos informais como anotações em papel, planilhas improvisadas e registros em aplicativos de mensagens.

A solução tem como finalidade estruturar e automatizar processos operacionais que normalmente são realizados de forma manual, reduzindo erros, melhorando a organização e aumentando a eficiência no controle das cobranças.

    Objetivo

O projeto tem como objetivo mitigar a desorganização e a perda de receita enfrentadas por microempreendedores que realizam vendas a prazo sem ferramentas adequadas de controle.

Busca-se fornecer uma ferramenta digital acessível e eficiente, permitindo que o próprio usuário gerencie seus clientes, acompanhe suas cobranças e organize seus recebimentos de forma autônoma, sem depender de métodos informais.

      Proposta

A solução, enquadrada na linha de Web Apps, será composta por três componentes principais:

    Aplicação Web (Frontend)

Interface responsiva acessível via navegador, responsável por permitir ao usuário:

cadastrar e gerenciar clientes;

registrar vendas a prazo;

acompanhar cobranças pendentes;

visualizar vencimentos;

consultar histórico de transações por cliente;

acessar dashboards com indicadores operacionais.

    API de Gestão (Backend)

Servidor responsável pelo processamento das regras de negócio, incluindo:

gerenciamento de clientes e transações;

controle do status de pagamentos;

persistência de dados;

validação de informações;

garantia de segurança e integridade dos dados.

    Orquestrador de Cobrança

Módulo responsável por apoiar o processo de comunicação com o cliente, incluindo:

geração de mensagens estruturadas de lembrete;

integração com WhatsApp para envio de cobranças;

padronização da comunicação de cobrança, reduzindo esforço manual.

    Status do Projeto

Projeto em fase inicial de definição e planejamento documental (NP1), seguindo as diretrizes da disciplina PAC Extensionista VII e aplicando práticas de Engenharia de Software voltadas à construção de soluções com impacto real na comunidade.

    Documentação

A documentação do projeto será organizada no repositório principal, contendo:

RFC.md: documento completo com a definição do problema, objetivos, escopo, arquitetura e requisitos do sistema;

diagramas de arquitetura baseados no modelo C4;

instruções de instalação e deploy;

definição de requisitos funcionais e não funcionais.

    Engenharia e Qualidade

Para atender aos requisitos obrigatórios do portfólio, o projeto adotará as seguintes práticas:

    Testes (TDD)
cobertura mínima de 75% no backend;

cobertura mínima de 25% no frontend;

foco em testes unitários das regras de negócio.

    Integração e Entrega Contínua (CI/CD)

pipeline automatizado utilizando GitHub Actions;

execução automática de testes a cada commit;

validação contínua da qualidade do código antes do deploy.

    Arquitetura

arquitetura baseada no modelo cliente-servidor;

organização em camadas (controller, service, repository);

modularização do código com separação de responsabilidades;

documentação por meio de diagramas no modelo C4.

    Qualidade de Código

utilização de ferramentas de análise estática como SonarCloud;

padronização de código conforme boas práticas;

monitoramento de métricas de qualidade.

    Monitoramento e Observabilidade
    
utilização de ferramentas de monitoramento de aplicação;

registro de logs para rastreamento de eventos;

acompanhamento da disponibilidade e desempenho do sistema.
