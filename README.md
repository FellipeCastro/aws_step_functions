# AWS Step Functions
AWS Step Functions é uma ferramenta de orquestração de aplicações distribuidas (microserviços) de maneira visal (clica e arrasta)

## Contexto
Imagine um aplicativo de delivery que conta com vários microserviços, ou seja, vários passos:
- Um serviço cuida da verificação dos pedidos em estoque
- Um serviço notifica o usuário sobre o status do seu pedido
- Um serviço notifica o restaurante sobre novos pedidos
- Assim por diante...

Para que todos esses microserviços se comuniquem, é necessário um *Serviço de mensageria*, ou seja, um serviço que comunique uma aplicação sobre a outra. Por exempo, é necessário que o serviço do restaurante seja comunicado quando houver um novo pedido, assim como o serviço do usuário precisa ser comunicado quando o pedido sair para entrega, e assim por diante. 

Para essa facilitar comunicação, surge o AWS Step Functions. Ou seja, se você tem varias aplicações rodando na AWS, você pode utilizar esse serviço para orquestra-las de maneira visual, sem código - para que todos esses serviços se comuniquem entre si.

Essa orquestração segue padroes de *Saga Patter*, podendo ser:
- Tarefas sequènciais
- Repetição de tarefas com falhas
- Tarefas paralelas
- Tarefas baseadas em saídas
- Tratativas de erros

Tudo isso contribui para uma orquestração fácil, segura e escalável dos serviços criados, além da automação de processos.
