## REQUISITOS FUNCIONAIS

- [x] O Sistema deve permitir o cadastro de usuários com nome, e-mail e senha.
- [x] O Sistema deve validar se o e-mail é único.
- [] O Sistema deve permitir que o usuário faça login com e-mail e senha.
- [] O sistema deve permitir que o usuário crie tarefas com título, descrição e prazo de entrega.
- [] O Sistema deve permitir que o usuário edite tarefas criadas por ele.
- [] O sistema deve permitir que o usuário exclua tarefas criadas por ele.
- [] O sistema deve listar as tarefas do usuário, podendo ser filtradas por status (pendente, em progresso, concluída).
- [] O sistema deve permitir que o usuário altere o status de uma tarefa (pendente → em progresso → concluída).
- [] O sistema deve registrar a data e hora de criação e atualização das tarefas.

## REQUISITOS NÃO FUNCIONAIS

- [x] Usar Node.js, Typescript e fastify para desenvolvimento
- [x] PostgreSQL como banco de dados
- [x] Senha do usuário devem ser armazenadas de forma segura usando hash
- [] As rotas protegidas (como gerencimando de tarefas) devem usar autenticação baseada em JWT
- [] O sistema deve ter uma documentação (README ou SWAGGER)
- [] O sistema deve ser capaz de lidar até com 100 requisições simultâneas sem degradar a performance
- [x] Seguir boas praticas de organização
- [x] Escrever testes unitários

## REGRAS DE NEGÓCIO

- [] Apenas o criador da tarefa pode editá-la ou excluí-la
- [x] Tarefas criadas sempre iniciam com o status "pendente"
- [] O prazo de entrega não pode ser uma data anterior à data atual
- [] Usuários não podem criar tarefas sem estar logados
- [] Usuários só podem visualizar e gerenciar suas próprias tarefas
- [] Um e-mail só pode ser associado a um único usuário
- [] Tarefas concluídas não podem voltar para o status "em progresso" ou "pendente"
