# NexTask

Gerenciador de projetos pessoal que roda direto no browser. Sem instalação, sem conta, sem servidor — um único arquivo `.html`.

![Dashboard do NexTask](prints/dashboard.jpg)

Construído para resolver um problema específico: manter contexto de projetos entre conversas com IAs. O fluxo é preencher uma planilha Excel, importar no app, acompanhar o andamento e exportar um resumo em texto para jogar no início de cada sessão com a IA. O contexto fica preservado de uma sessão pra outra, além de ter um acompanhamento de cada etapa do projeto para documentar ao final.

O projeto começou como um artefato dentro do Claude. Quando as limitações apareceram — sem persistência entre sessões, sem exportação de arquivos — a solução foi migrar para HTML standalone. Isso resolveu tudo e ainda tornou a ferramenta fácil de compartilhar: basta abrir o arquivo no browser.

---

## Screenshots

![Lista de tarefas](prints/tarefas.jpg)

![Matriz de riscos](prints/riscos.jpg)

---

## Como usar

1. Baixe o arquivo `nexTask.html`
2. Abra no browser
3. Preencha os dados do projeto ou importe um `.xlsx` com o template
4. Acompanhe tarefas, subtarefas, riscos e anexos
5. Exporte o resumo em `.md` e use como contexto em conversas com IA

---

## Funcionalidades

- Fases de projeto: Iniciação → Planejamento → Execução → Encerramento
- Tarefas com subtarefas, responsável, data prevista e status
- Arrastar e soltar para reordenar e mover tarefas entre fases
- Busca e filtro por status (clique nos cards do dashboard)
- Matriz 3×3 de riscos por probabilidade × impacto
- Desfazer com Ctrl+Z em ações destrutivas
- Próxima ação em destaque com botão de iniciar
- Export para `.xlsx`, `.csv` e `.md`
- Import de planilha `.xlsx` com validação por aba
- Salvamento automático no browser

---

## Stack

HTML5 · CSS3 · Vanilla JS · SheetJS

Nenhuma dependência de runtime. Zero build step. Arquivo único.

---

## Template Excel

O repositório inclui `NexTask_Template.xlsx` com as abas:

`Projeto` · `Tarefas` · `Subtarefas` · `Riscos` · `Anexos`

Preencha e importe direto no app.

---

## Contexto

Desenvolvido durante transição de carreira de Supply Chain para Dados. Colaboração com Claude (Anthropic) e DeepSeek ao longo do processo para revisão de interface, experiência de uso e código.
