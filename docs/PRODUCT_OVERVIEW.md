# Visão geral do produto

## Visão geral

O AgendeCom é uma aplicação web responsiva para a gestão de atendimentos com hora marcada. O produto conecta a rotina interna do profissional a uma página pública pela qual o cliente pode solicitar um horário.

## Público

O sistema foi desenvolvido para profissionais autônomos e pequenos prestadores de serviço que organizam a rotina por agenda, como atividades de beleza, bem-estar, aulas, treinamento e fotografia.

O cliente final também utiliza o produto para escolher horários e, opcionalmente, acompanhar seus compromissos em uma área privada.

## Problema

Serviços, clientes, horários, confirmações e cancelamentos frequentemente ficam espalhados entre conversas e anotações. Essa fragmentação dificulta visualizar a operação e reaproveitar uma vaga que ficou disponível.

## Solução

O AgendeCom centraliza essas informações e oferece um link público conectado à disponibilidade configurada pelo profissional. O sistema também apoia o acompanhamento de sinais, faltas, cancelamentos e oportunidades da lista de espera.

## Funcionalidades

- agenda diária, histórico, atendimentos manuais e bloqueios;
- disponibilidade semanal, intervalos, antecedência e regras de cancelamento;
- serviços com preço, duração, instruções, visibilidade e sinal opcional;
- página pública para escolha de serviço, data e horário;
- cadastro, busca, observações e histórico relacionado aos clientes;
- lista de espera com preferências e convite assistido por WhatsApp;
- acompanhamento de presença, faltas, cancelamentos e sinais;
- relatórios de faturamento previsto, comparecimento, faltas, horários recuperados e serviços mais agendados;
- área opcional do cliente para compromissos vinculados;
- assinatura da plataforma integrada ao Stripe;
- interface adaptada para desktop e celular.

## Principais fluxos

### Configuração profissional

O profissional cria a conta, conclui o perfil, cadastra serviços e define expediente, intervalos e demais regras de disponibilidade.

### Agendamento público

O profissional compartilha seu link. O cliente seleciona um serviço, escolhe data e horário disponíveis, informa seus dados e registra a solicitação sem cadastro obrigatório.

### Sinal via Pix

Quando configurado, o cliente recebe a opção de sinal via Pix. O valor é pago diretamente ao profissional, que acompanha e confere a informação no sistema.

### Lista de espera

O cliente ou o profissional registra o interesse e as preferências. Ao surgir uma vaga, o sistema prepara um convite e abre o WhatsApp; o usuário revisa e confirma o envio.

### Área do cliente

O cliente pode criar uma conta, vincular compromissos recebidos por link, consultar próximos horários e histórico, confirmar presença e cancelar quando a regra configurada permitir.

## Tecnologias

- **Front-end:** React, TypeScript, Vite e Tailwind CSS;
- **Backend:** Node.js, Express e Zod;
- **Dados e autenticação:** Firebase Authentication e Cloud Firestore;
- **Proteção da aplicação:** Firebase App Check;
- **Infraestrutura:** Firebase Hosting e Google Cloud Run;
- **Assinaturas:** Stripe;
- **Qualidade:** Vitest, Supertest, Firebase Emulator Suite, TypeScript e lint automatizado;
- **Aplicação web:** manifesto PWA e service worker.

## Integrações públicas relevantes

- Stripe para assinatura da plataforma;
- WhatsApp por links preparados pelo sistema e acionados pelo usuário;
- geração local de QR Code e código Pix para sinal pago diretamente ao profissional;
- seletor de contatos do dispositivo quando disponível e autorizado pelo usuário.

## Responsividade

A navegação profissional e o agendamento público possuem composições adaptadas para desktop e celular. A versão móvel mantém acesso às ações essenciais da agenda e ao fluxo público de escolha de serviço.

## Status

O AgendeCom está disponível em produção e continua em evolução.

Endereço confirmado: [https://agenda-b4b7c.web.app](https://agenda-b4b7c.web.app).
