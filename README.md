# fullstack-iot-monitoring
Full Stack Programming Challenge: IoT Device Monitoring

Desafio de Programação Full Stack: Monitoramento de Dispositivos IoT
Introdução
Sua tarefa é desenvolver uma aplicação web que monitora dispositivos IoT conectados à internet. A aplicação deverá permitir que os usuários visualizem o estado dos dispositivos, recebam alertas em caso de falhas, e gerenciem as configurações de monitoramento. Esta aplicação será usada por operadores que precisam manter o controle sobre o funcionamento de dispositivos críticos em tempo real.
Objetivo
Desenvolver uma aplicação web Full Stack que permita:
•	Visualizar o status dos dispositivos IoT: Mostrar uma lista de dispositivos e seu status atual.
•	Gerenciar dispositivos: Adicionar, editar e remover dispositivos monitorados.
•	Configurar alertas: Configurar alertas que serão disparados quando um dispositivo não responder ou apresentar falhas.
•	Visualizar logs: Permitir a visualização dos logs de atividade de cada dispositivo.
•	Autenticação de usuário: Implementar um sistema básico de autenticação para proteger a aplicação.
Requisitos Técnicos
Backend:
•	Desenvolver uma API RESTful usando Java 8+ (preferencialmente com Spring Boot).
•	Utilizar um banco de dados relacional (ex: PostgreSQL, MySQL).
•	Os dispositivos devem ser representados por uma entidade contendo as seguintes informações:
o	id: UUID do dispositivo.
o	name: Nome do dispositivo.
o	status: Status atual do dispositivo (ativo, inativo, em falha).
o	lastPing: Data e hora do último ping recebido.
o	location: Localização do dispositivo (opcional).
o	logs: Registros de atividades relacionadas ao dispositivo.
•	Endpoints mínimos:
o	GET /devices: Retorna a lista de dispositivos.
o	GET /devices/{id}: Retorna os detalhes de um dispositivo específico.
o	POST /devices: Adiciona um novo dispositivo.
o	PUT /devices/{id}: Atualiza os dados de um dispositivo.
o	DELETE /devices/{id}: Remove um dispositivo.
o	GET /devices/{id}/logs: Retorna os logs de um dispositivo específico.
o	POST /alerts: Configura alertas para os dispositivos.
Frontend:
•	Desenvolver a interface do usuário usando Vue 3.
•	Implementar uma dashboard que exiba a lista de dispositivos e permita a interação (CRUD) com os mesmos.
•	Mostrar os detalhes de um dispositivo em uma página separada.
•	Permitir que os operadores visualizem logs e configurem alertas diretamente pela interface.
•	Implementar autenticação básica (login/logout) para acessar a aplicação.
Entregáveis
•	Código fonte: Inclua todo o código fonte da aplicação (frontend e backend) em um repositório Git pessoal. O repositório deve ser público para que possamos avaliar o código durante a entrevista.
•	Instruções de setup: Forneça um arquivo README.md com instruções claras de como configurar e rodar a aplicação localmente.
•	Documentação: Incluir uma breve documentação explicando as decisões de arquitetura, estrutura do código, e qualquer funcionalidade extra que foi implementada.
Requisitos Extras (Opcional)
•	Monitoramento em tempo real: Implemente a capacidade de visualizar em tempo real o status dos dispositivos utilizando WebSockets.
•	Relatórios: Gere relatórios sobre o status dos dispositivos, por exemplo, quantas vezes um dispositivo entrou em falha em um determinado período.
•	Testes unitários e de integração: Adicione testes para garantir a qualidade do código e da aplicação.
Avaliação
A avaliação do desafio será baseada nos seguintes critérios:
•	Funcionalidade: A aplicação atende aos requisitos especificados?
•	Qualidade do Código: O código está limpo, bem documentado e segue boas práticas de desenvolvimento?
•	Interface de Usuário: A interface é intuitiva e bem projetada?
•	Eficiência: A aplicação é eficiente em termos de desempenho?
•	Extras: Implementou funcionalidades extras ou melhorias?
