# fornecedores-api

Vamos desenvolver uma api de fornecedores RESTUL utilizando fastapi + mongo, utilizando vscode.

Esse desenvolvimento será realizado por etapas.

1 - Etapa
    Nosso problema se delimita, a api irá gerenciar os fornecedores.
    Onde o fornecedor pode ser uma pessoa fisica ou juridica, o cadastro deve ser unico.
    Nessa etapa o fornecedor deve possuir nome (até 150 caracteres) e cpf ou cnpj.

    1.1 Estrutura da api:
        /
        /.vscode
        /app
        /requirements.txt

        Utilizar python3.8 o arquivo requirements.txt deve conter os requisitos para api executar.
    
    1.2 linter
        Adicionar a pasta \.vscode o arquivo settings.json

        {
          "python.linting.flake8Enabled": true,
          "python.linting.pydocstyleEnabled": false,
          "python.linting.enabled": true,
        }

    1.3 virtualenv
        Criar o virtualenv na raiz do projeto
        /venv
    
    1.4 rotas
        Vamos definir a primeira rota, a de criação do fornecedor.
         - Caminho path para rota
         - Payload de input
         - Payload de output
         - status codes
        
        Importante a forma (modelo de dados) que o fornecedor será salvo no database pode ou será
        diferente da representação (modelo / schema) utilizado na api.
        Como estamos utilizando fastapi os modelos/schemas vão utilizar pydantic.
