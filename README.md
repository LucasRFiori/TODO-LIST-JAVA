
# TODO APPLICATION

É uma api rest que tem como objetivo gerenciar tarefas a serem realizadas durante o dia.


Desenvolvido durante o curso de java da Rocketseat.




## Dependências

Siga as instruções desse notion:

https://efficient-sloth-d85.notion.site/Curso-de-Java-2408d11bfc3447e980fe9460b6293976

## Rodando o projeto
```bash
  # Na raiz do projeto rode:
  mvn spring-boot:run
```
    

## Documentação da API

⚠️ **Todas as rotas - /tasks/ necessitam da autenticação por Basic Auth**. ⚠️

#### Criando um usuário

```http
  POST /user/
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `name` | `string` | Nome do usuário. |
| `username` | `string` | Username do usuário. |
| `password` | `string` | Senha do usuário. |

#### Retornando tarefas de um usuário.

```http
  GET /tasks/
```

#### Retorna um item

```http
  POST /tasks/
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `title`      | `string` | Título da tarefa. |
| `description` | `string` | Descrição da tarefa. |
| `priority` | `string` | Prioridade da tarefa. |
| `startAt` | `DateTime` | Início da tarefa. |
| `endAt` | `DateTime` | Término da tarefa. |


#### Atualizar dados da tarefa.
```http
  PUT /tasks/{taskId}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `title`      | `string` | Título da tarefa. |
| `description` | `string` | Descrição da tarefa. |
| `priority` | `string` | Prioridade da tarefa. |
| `startAt` | `DateTime` | Início da tarefa. |
| `endAt` | `DateTime` | Término da tarefa. |



##### - Lucas Rodrigues Fiori 2023

