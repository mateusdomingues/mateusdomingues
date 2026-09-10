# PetOS

> Aplicação web em desenvolvimento para gestão de operações relacionadas a serviços para pets. O código-fonte permanece privado.

## Contexto

Negócios do segmento pet podem precisar controlar unidades, profissionais, serviços, animais, agenda e transporte no mesmo ambiente. O PetOS explora essa operação em uma aplicação organizada por perfis e módulos.

## Minha participação

Trabalhei na estrutura da aplicação, autenticação, organização multitenant, dashboards, agendamento público, gestão de pets e integração com Firebase.

## Funcionalidades implementadas

- Autenticação e rotas protegidas
- Separação de dados por empresa
- Dashboard administrativo e área do cliente
- Cadastro e histórico de pets
- Agenda e agendamento público
- Gestão de profissionais e serviços
- Planejamento e acompanhamento de rotas
- Visão específica para motoristas
- Atualizações em tempo real com Firestore
- Manifest e service worker para experiência PWA

## Tecnologias

Next.js, React, TypeScript, Firebase Authentication, Firestore, Tailwind CSS e Vercel.

## Arquitetura em alto nível

A interface utiliza contextos separados para autenticação e empresa ativa. As rotas protegidas verificam usuário e organização antes de liberar os módulos. Serviços de acesso a dados concentram operações de agenda, profissionais, serviços e rotas.

## Desafios trabalhados

- Diferentes experiências para administrador, cliente e motorista
- Isolamento de dados por empresa
- Sincronização em tempo real
- Organização de rotas e agendamentos
- Adaptação de uma aplicação React para Next.js

## Situação

Projeto em desenvolvimento. Os módulos financeiro e de estoque ainda aparecem como etapas futuras e não são apresentados como funcionalidades concluídas.

[Ver demonstração](https://pet-os-five.vercel.app)
