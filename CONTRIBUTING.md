# Como Contribuir

Ficamos muito felizes por você se interessar em contribuir com [Nome do Projeto]! Toda contribuição é bem-vinda.

Ao participar deste projeto, você concorda em seguir nosso [Código de Conduta](CODE_OF_CONDUCT.md).

## Como Posso Ajudar?

### Reportando Bugs

- **Verifique se o bug já não foi reportado:** Pesquise nas [Issues](link-para-issues) do projeto.
- **Se não foi:** Abra uma nova issue usando o template de "Bug Report".
- **Descreva em detalhes:**
  - Passos exatos para reproduzir o bug.
  - O que você esperava que acontecesse.
  - O que de fato aconteceu (inclua logs de erro e screenshots, se possível).
  - A versão do projeto que você está usando.

### Sugerindo Melhorias

- Abra uma nova issue usando o template de "Feature Request".
- Descreva o problema que sua sugestão resolve e por que ela seria útil.

### Contribuindo com Código

Este é o fluxo de trabalho básico para enviar uma contribuição:

1.  **Faça um Fork** deste repositório.
2.  **Configure o ambiente:**
    ```bash
    # Ex: Clone seu fork
    git clone [https://github.com/SEU-USUARIO/NOME-DO-PROJETO.git](https://github.com/SEU-USUARIO/NOME-DO-PROJETO.git)
    cd NOME-DO-PROJETO
    # Ex: Instale as dependências (ajuste para seu projeto)
    mvn install
    ```
3.  **Crie uma Branch:**
    ```bash
    # Use um nome descritivo (ex: fix/bug-123 ou feature/nova-funcionalidade)
    git checkout -b feature/minha-contribuicao
    ```
4.  **Codifique e Teste:**
    - Faça suas alterações no código.
    - **Adicione testes!** Sua contribuição precisa ser testada.
    - Rode a suíte de testes localmente para garantir que nada quebrou:
      ```bash
      # Ex: (ajuste para seu projeto)
      mvn test
      ```
5.  **Faça o Commit:**
    - Use mensagens de commit claras e descritivas (sugerimos [Conventional Commits](https://www.conventionalcommits.org/)).
    ```bash
    git add .
    git commit -m "feat: Adiciona funcionalidade X que faz Y"
    ```
6.  **Envie para o seu Fork (Push):**
    ```bash
    git push origin feature/minha-contribuicao
    ```
7.  **Abra um Pull Request (PR):**
    - Vá até o repositório original no GitHub e abra um Pull Request.
    - Preencha o template do PR, linkando a issue que sua contribuição resolve (ex: "Closes #123").
    - Aguarde a revisão. Responderemos o mais breve possível!

Obrigado pela sua contribuição!
