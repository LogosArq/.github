# Diretrizes de Contribuição

Bem-vindo(a) à equipe! Este documento estabelece as diretrizes para contribuir com este projeto. Segui-las garante a qualidade do código e a eficiência da equipe.

Ao contribuir, você concorda em seguir nosso [Código de Conduta](CODE_OF_CONDUCT.md) (que define a cultura da nossa equipe).

## Configuração do Ambiente

1.  **Clone o Repositório:**
    Como este é um projeto privado, você não precisa fazer "Fork". Clone o repositório diretamente (assumindo que você tenha permissão).
    ```bash
    git clone [URL-DO-REPOSITORIO-AQUI]
    cd [NOME-DO-PROJETO]
    ```

2.  **Instale as Dependências:**
    *(Esta seção deve ser adaptada para cada serviço. Ex: Java/Maven, Node/NPM, etc.)*
    ```bash
    # Exemplo para Java/Maven:
    mvn clean install
    ```

3.  **Variáveis de Ambiente:**
    Copie o arquivo de exemplo `.env.example` para um novo arquivo `.env` e preencha as variáveis locais necessárias (ex: senhas de banco de dados, URLs de outros serviços).
    ```bash
    cp .env.example .env
    ```

4.  **Serviços Dependentes:**
    Este projeto pode depender de outros serviços (ex: um banco de dados, outra API). Use o Docker Compose para subir a infraestrutura local.
    ```bash
    # Exemplo: (pode estar na raiz do projeto ou no repo 'infra')
    docker-compose up -d
    ```

5.  **Rode o Projeto:**
    ```bash
    # Exemplo para Quarkus:
    mvn quarkus:dev
    ```

## Rodando Testes

É **obrigatório** que todos os testes passem antes de um Pull Request ser aberto.

```bash
# Exemplo para Java/Maven:
mvn test
