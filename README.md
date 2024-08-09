# Fullstack Monitoring

## Desafio de Programação Full Stack: Monitoramento de Dispositivos

### Introdução
Sua tarefa é desenvolver uma aplicação web que monitora dispositivos conectados à internet. A aplicação deverá permitir que os usuários visualizem o estado dos dispositivos, recebam alertas em caso de falhas, e gerenciem as configurações de monitoramento. Esta aplicação será usada por operadores que precisam manter o controle sobre o funcionamento de dispositivos críticos em tempo real.

### Objetivo
Desenvolver uma aplicação web Full Stack que permita:

- **Visualizar o status dos dispositivos:** Mostrar uma lista de dispositivos e seu status atual.
- **Gerenciar dispositivos:** Adicionar, editar e remover dispositivos monitorados.
- **Configurar alertas:** Configurar alertas que serão disparados quando um dispositivo não responder ou apresentar falhas.
- **Visualizar logs:** Permitir a visualização dos logs de atividade de cada dispositivo.
- **Autenticação de usuário:** Implementar um sistema básico de autenticação para proteger a aplicação.

### Requisitos Técnicos

#### Backend:
- Desenvolver uma API RESTful usando **Java 8+** (preferencialmente com Spring Boot).
- Utilizar um banco de dados relacional (ex: PostgreSQL, MySQL).
- Os dispositivos devem ser representados por uma entidade contendo as seguintes informações:
  - **id:** UUID do dispositivo.
  - **name:** Nome do dispositivo.
  - **status:** Status atual do dispositivo (ativo, inativo, em falha).
  - **lastPing:** Data e hora do último ping recebido.
  - **location:** Localização do dispositivo (opcional).
  - **logs:** Registros de atividades relacionadas ao dispositivo.
  
- Endpoints mínimos:
  - `GET /devices`: Retorna a lista de dispositivos.
  - `GET /devices/{id}`: Retorna os detalhes de um dispositivo específico.
  - `POST /devices`: Adiciona um novo dispositivo.
  - `PUT /devices/{id}`: Atualiza os dados de um dispositivo.
  - `DELETE /devices/{id}`: Remove um dispositivo.
  - `GET /devices/{id}/logs`: Retorna os logs de um dispositivo específico.
  - `POST /alerts`: Configura alertas para os dispositivos.

#### Frontend:
- Desenvolver a interface do usuário usando qualquer framework de **sua preferência**.
- Implementar uma dashboard que exiba a lista de dispositivos e permita a interação (CRUD) com os mesmos.
- Mostrar os detalhes de um dispositivo em uma página separada.
- Permitir que os operadores visualizem logs e configurem alertas diretamente pela interface.
- Implementar autenticação básica (login/logout) para acessar a aplicação.

### Entregáveis
- **Código fonte:** Inclua todo o código fonte da aplicação (frontend e backend) em um repositório Git pessoal. O repositório deve ser público para que possamos avaliar o código durante a entrevista.
- **Instruções de setup:** Forneça um arquivo `README.md` com instruções claras de como configurar e rodar a aplicação localmente.
- **Documentação:** Incluir uma breve documentação explicando as decisões de arquitetura, estrutura do código, e qualquer funcionalidade extra que foi implementada.

### Requisitos Extras (Opcional)
- **Monitoramento em tempo real:** Implemente a capacidade de visualizar em tempo real o status dos dispositivos utilizando WebSockets.
- **Relatórios:** Gere relatórios sobre o status dos dispositivos, por exemplo, quantas vezes um dispositivo entrou em falha em um determinado período.
- **Testes unitários e de integração:** Adicione testes para garantir a qualidade do código e da aplicação.

### Avaliação
A avaliação do desafio será baseada nos seguintes critérios:

- **Funcionalidade:** A aplicação atende aos requisitos especificados?
- **Qualidade do Código:** O código está limpo, bem documentado e segue boas práticas de desenvolvimento?
- **Interface de Usuário:** A interface é intuitiva e bem projetada?
- **Eficiência:** A aplicação é eficiente em termos de desempenho?
- **Extras:** Implementou funcionalidades extras ou melhorias?

## Expectativas por Nível

### **Júnior**
Esperamos que os candidatos de nível Júnior demonstrem um entendimento básico dos conceitos de desenvolvimento web Full Stack. O foco principal deve ser na implementação das funcionalidades essenciais, seguindo as melhores práticas básicas de codificação. O candidato deve:

- Implementar o CRUD para dispositivos IoT de forma funcional e eficiente.
- Demonstrar compreensão dos fundamentos de autenticação e controle de acesso.
- Fornecer código que seja legível, com comentários claros onde necessário.
- Documentar quaisquer desafios encontrados e como foram resolvidos.
- A entrega deve atender a todos os requisitos funcionais, com atenção especial para a correta implementação dos endpoints e da interface do usuário.

### **Pleno**
Candidatos de nível Pleno devem mostrar uma compreensão mais aprofundada do desenvolvimento Full Stack, incluindo a estruturação da aplicação para manutenção e escalabilidade futura. O candidato deve:

- Projetar uma arquitetura que suporte a escalabilidade e a manutenibilidade da aplicação.
- Implementar um sistema de logs eficiente e detalhado, com capacidade de auditoria.
- Garantir que o código seja modular, reutilizável e devidamente testado (testes unitários e de integração são esperados).
- Demonstrar uma abordagem proativa no tratamento de erros e na gestão de exceções.
- Incluir explicações sobre as decisões arquiteturais tomadas e suas vantagens.
- Fornecer documentação que cubra tanto o setup quanto a manutenção da aplicação.

### **Sênior**
Candidatos de nível Sênior devem demonstrar liderança técnica e a capacidade de pensar em uma aplicação robusta, segura e altamente escalável. O candidato deve:

- Propor e implementar uma arquitetura avançada que suporte grandes volumes de dispositivos IoT e multi-tenancy, se aplicável.
- Garantir a segurança em todos os aspectos da aplicação, desde a autenticação até a proteção contra vulnerabilidades comuns.
- Otimizar o desempenho da aplicação, tanto no backend quanto no frontend, utilizando técnicas avançadas.
- Implementar práticas de monitoramento e manutenção que garantam a estabilidade e a disponibilidade da aplicação em ambiente de produção.
- Demonstrar uma compreensão sólida de como a aplicação pode ser escalada e mantida no longo prazo, incluindo práticas para monitoramento em tempo real e relatórios.
- Produzir uma documentação detalhada, incluindo justificativas para escolhas técnicas, práticas de segurança e estratégias de monitoramento e otimização.
