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

````markdown
## Rodando Testes

É **obrigatório** que todos os testes passem antes de um Pull Request ser aberto.

```bash
# Exemplo para Java/Maven:
mvn test
````

**Qualquer nova funcionalidade ou correção de bug DEVE incluir novos testes** que cubram a mudança.

-----

## Nosso Fluxo de Trabalho (Gitflow)

### 1\. Sincronize sua `main`

Sempre comece da branch `main` (ou `develop`, se usarem) atualizada.

```bash
git checkout main
git pull origin main
```

### 2\. Crie sua Branch

Nunca trabalhe diretamente na `main`. Crie uma nova branch seguindo nosso padrão de nomenclatura:

  * **Features (Novas Funcionalidades):** `feature/[ID-TAREFA]-descricao-curta`
  * **Fixes (Correção de Bugs):** `fix/[ID-TAREFA]-descricao-curta`
  * **Chores (Tarefas técnicas):** `chore/[ID-TAREFA]-refatoracao-build`

**Exemplo:**

```bash
git checkout -b feature/TASK-101-login-com-google
```

### 3\. Codifique, Teste, Faça o Commit

Faça seu trabalho. Faça commits pequenos e atômicos. Use o padrão [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) para as mensagens:

  * `feat:` (nova funcionalidade)
  * `fix:` (correção de bug)
  * `docs:` (mudanças na documentação)
  * `style:` (formatação, ponto-e-vírgula, etc.)
  * `refactor:` (refatoração de código que não altera funcionalidade)
  * `test:` (adição ou correção de testes)
  * `chore:` (atualização de build, dependências, etc.)

**Exemplo de commit:**

```bash
git commit -m "feat: Adiciona endpoint de autenticação OAuth2"
```

### 4\. Abra um Pull Request (PR)

Envie sua branch para o repositório e abra um Pull Request.

```bash
git push origin feature/TASK-101-login-com-google
```

Preencha o template do Pull Request que aparecerá automaticamente. Um PR só será "mergeado" após a aprovação de pelo menos um outro membro da equipe e com a CI (GitHub Actions) passando.

```
```
