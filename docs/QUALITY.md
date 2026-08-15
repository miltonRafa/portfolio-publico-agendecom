# Qualidade e validações

## Validação de dados

A aplicação utiliza esquemas de validação no backend para limitar formatos, tamanhos e valores recebidos. Formulários também apresentam validações e mensagens de erro antes ou durante o envio.

Entre os dados validados estão perfil profissional, disponibilidade, serviços, solicitações de agendamento, lista de espera e ações realizadas pelo cliente.

## Regras de negócio

O projeto possui verificações aplicadas a áreas como:

- expediente, intervalos e dias sem atendimento;
- bloqueios de dia inteiro ou de períodos específicos;
- duração do serviço e conflito com outros atendimentos;
- limite de agendamentos simultâneos;
- antecedência e janela futura de disponibilidade;
- prazo permitido para cancelamento pelo cliente;
- visibilidade e ativação de serviços;
- cálculo de sinal fixo ou percentual;
- transições de estado do atendimento e do sinal;
- isolamento dos dados de cada conta profissional.

## Testes automatizados

O projeto utiliza Vitest e Supertest em testes de regras e componentes de domínio. A suíte contempla políticas de agenda, períodos de relatório, persistência de clientes, seleção de contatos, sessões autenticadas, área do cliente e limites de segurança da API.

As regras de acesso do Cloud Firestore possuem testes preparados para execução com o Firebase Emulator Suite.

## Responsividade

A interface possui navegação e componentes adaptados para desktop e celular. O fluxo público de agendamento e a agenda profissional foram verificados nos dois formatos.

## Tratamento de erros

A interface apresenta estados de carregamento, mensagens de validação e retornos de falha para operações relevantes. A API centraliza respostas de erro e evita retornar detalhes internos desnecessários ao cliente.

## Segurança

O projeto adota, em alto nível:

- autenticação com Firebase Authentication;
- confirmação de e-mail para áreas protegidas;
- controle de acesso por identidade e situação da assinatura;
- Firebase App Check nas operações configuradas;
- validação de entrada no backend;
- limitação de requisições e cabeçalhos de segurança;
- validação das comunicações de assinatura com o Stripe;
- regras de acesso ao banco verificadas em ambiente emulado.

Detalhes operacionais, credenciais, regras completas e configurações internas não fazem parte desta documentação pública.
