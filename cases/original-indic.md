# Original Indic

> Case técnico de um SaaS de gestão e agendamentos. O código-fonte permanece privado por conter regras de negócio e integrações de produção.

## Contexto

Pequenos negócios que trabalham com atendimento marcado costumam controlar agenda, clientes, profissionais e pagamentos em ferramentas separadas. O Original Indic foi desenvolvido para reunir essa operação em um único sistema e oferecer um fluxo simples de reserva para o cliente final.

## Minha participação

Sou responsável pela concepção do produto, definição dos fluxos, desenvolvimento da interface, modelagem das regras de negócio, integração com serviços externos, evolução do banco de dados e publicação da aplicação.

## Principais funcionalidades

- Cadastro e gestão de clientes, profissionais e serviços
- Configuração de disponibilidade, duração e intervalos
- Regras para evitar conflitos entre horários
- Agenda operacional e painel administrativo
- Perfis de acesso e permissões de equipe
- Agendamentos recorrentes
- Área do cliente
- Gestão de planos e assinaturas
- Cobrança por Pix e integração com webhook do Mercado Pago
- Geocodificação e cálculo de informações de deslocamento
- Notificações push
- Geração de recibos
- Experiência instalável como PWA
- Landing page, sitemap e recursos de SEO

## Tecnologias

React, TypeScript, Vite, Node.js, Express, Supabase, PostgreSQL, Firebase, APIs REST e Vercel.

## Arquitetura em alto nível

A aplicação separa a experiência pública de agendamento, o painel autenticado e rotas administrativas. O frontend consome uma camada de serviços organizada por domínio, enquanto operações que exigem credenciais ou validações sensíveis são processadas no servidor. Dados de diferentes empresas são isolados por contexto de organização.

Nenhuma credencial, regra sensível de pagamento ou configuração interna é apresentada neste case.

## Decisões técnicas

- Centralização das chamadas externas em módulos de API
- Separação de contextos de autenticação, organização, plano e permissões
- Validação de disponibilidade antes da confirmação do horário
- Uso de webhooks para processar atualizações assíncronas de pagamentos
- Rotas distintas para site institucional, agendamento e painel
- Evolução do banco por migrações versionadas

## Desafios trabalhados

Os principais desafios foram conciliar duração de serviços com disponibilidade real, impedir reservas conflitantes, atender diferentes perfis de usuário e integrar pagamentos e notificações sem expor credenciais no navegador.

## Situação

Projeto privado em evolução e conectado a um ambiente de produção. Uma demonstração pode ser apresentada durante processos seletivos sem exposição do código-fonte.
