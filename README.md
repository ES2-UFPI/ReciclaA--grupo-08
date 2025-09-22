# ReciclaAI

### Integrantes
- Bernardo Ferreira de Mourão Ribeiro
- Maria do Rosario de Fatima Martins Ferreira 
- Geyldson Lucas Mendes de Sousa 

## Visão geral

O ReciclaAi é um aplicativo voltado para incentivar e facilitar a reciclagem, conectando produtores, coletores e cooperativas.
O sistema permite acompanhar estatísticas, compartilhar relatórios, receber lembretes, organizar coletas e gamificar o processo de reciclagem, tornando-o mais acessível e motivador.

## Arquitetura (MVC)

O projeto segue a arquitetura Model–View–Controller (MVC):

- Model (M): responsável pela lógica de dados, representando as entidades do sistema (usuários, resíduos, relatórios, coletas etc.).

- View (V): responsável pela interface com o usuário, exibindo as informações e recebendo entradas.

- Controller (C): responsável por orquestrar a comunicação entre Model e View, aplicando regras de negócio.


Essa separação permite manter o código organizado, facilitar testes, e dar flexibilidade para futuras expansões.

## Integração das Ferramentas

O sistema é dividido em camadas, cada uma com sua responsabilidade:

#### Camada de Apresentação (View)

Implementada no front-end.
Responsável por exibir as telas, gráficos, relatórios e formulários.
Comunica-se com a camada de controle por meio de requisições à API. 

#### Camada de Controle (Controller)

Implementada no back-end.
Processa as requisições vindas do front-end.
Aplica regras de negócio, validações e orquestra o fluxo de dados.


#### Camada de Dados (Model)

Representa as entidades principais (usuário, resíduos, coleta, relatório, etc.).
Garante persistência dos dados.
Comunica-se com a camada de controle por meio de consultas e atualizações.


Esse desenho garante que mudanças em uma camada não impactem diretamente as demais, facilitando manutenção e escalabilidade.
