# Synthetic Personas 🧪

**Teste ideias antes de testar pessoas.**

Um protocolo aberto para testes de usabilidade sintéticos assistidos por IA, compatível com diferentes LLMs e ambientes de agentes.

**Criado e mantido pela OutBoxLab.**

> Beta público: `v0.1.0-beta` · Licença MIT

🇧🇷 **Português** · [🇺🇸 English](README.en.md)

### Comece em poucos minutos

**[Instalar](#comece-aqui) · [Executar o primeiro teste](#seu-primeiro-teste) · [Ver exemplo](examples/first-test.md) · [Dar feedback](https://github.com/outboxlab/synthetic-personas/issues)**

> ⭐ Se o Synthetic Personas for útil para você, marque o repositório com uma Star para acompanhar a evolução do protocolo.

Synthetic Personas guia agentes de IA na execução de testes estruturados de usabilidade sintética para conceitos, jornadas, wireframes e protótipos, mantendo o comportamento simulado claramente separado de evidências obtidas com usuários reais.

## Por que Synthetic Personas?

Times de produto frequentemente precisam explorar uma ideia antes de uma pesquisa formal estar disponível ou antes de um protótipo estar maduro o suficiente para um estudo completo.

Synthetic Personas oferece uma forma estruturada de usar IA nessa exploração sem tratar simulações como se fossem usuários reais.

Ele foi criado como um protocolo aberto, e não como um prompt preso a um modelo específico. Assim, a metodologia pode viajar entre ChatGPT, Claude, Hermes e outros ambientes de agentes.

## O que ele faz

Um wizard conversacional ajuda você a:

- definir o objetivo da pesquisa;
- entender a fidelidade do material;
- analisar os materiais disponíveis;
- selecionar, importar ou criar personas;
- formular missões neutras;
- executar as simulações;
- consolidar descobertas, hipóteses e recomendações.

Você não precisa saber estruturar um teste de usabilidade antes de começar.

## Comece aqui

### ChatGPT

Disponibilize este repositório ou seus arquivos em um ambiente do ChatGPT que consiga lê-los. Comece por `SKILL.md` e diga:

**`Instalar Personas`**

### Claude

Disponibilize os arquivos do repositório no projeto/ambiente Claude. Carregue `SKILL.md` e `adapters/claude/SKILL.md` e diga:

**`Instalar Personas`**

### Hermes

Disponibilize o repositório no workspace do Hermes. Carregue `SKILL.md` e `adapters/hermes/SKILL.md` e diga:

**`Instalar Personas`**

### Outros agentes

Carregue `SKILL.md` e `adapters/generic/SYSTEM_PROMPT.md`. O protocolo se adapta às capacidades realmente disponíveis no ambiente.

> A mecânica exata de instalação varia conforme o host. Synthetic Personas não exige um fornecedor, servidor MCP ou integração de design específicos.

## Seu primeiro teste

Depois da configuração, diga:

**`Novo teste`**

O wizard conduz o processo:

`Projeto → Fidelidade → Materiais → Personas → Objetivos de aprendizado → Missões → Plano de teste → Execução → Síntese → Relatório`

Informações que você já forneceu são aproveitadas. O wizard não transforma a configuração em uma maratona de perguntas.

## Materiais de entrada

Use o que seu ambiente suportar:

- fontes de design conectadas, como Figma;
- screenshots ou imagens;
- PDFs;
- links de protótipos acessíveis;
- jornadas descritas pelo usuário.

**Figma é opcional.**

## Método

A sequência padrão do teste é:

1. exploração livre, sem missão e sem direcionamento;
2. investigação do modelo mental;
3. missões neutras específicas por persona;
4. consolidação entre personas;
5. descobertas, incertezas, hipóteses e recomendações.

A avaliação muda de acordo com a fidelidade. **Um wireframe é avaliado como wireframe, não como interface visual finalizada.**

## Integridade da pesquisa

Participantes sintéticos são **simulações, não usuários reais**.

Eles podem ajudar a explorar hipóteses, identificar possíveis fricções, ensaiar jornadas e preparar pesquisas reais, mas não substituem evidências empíricas obtidas com pessoas.

O protocolo mantém separados:

**evidência fornecida → comportamento sintético → interpretação → hipótese → recomendação → limitações/desconhecidos**

Essa separação é uma parte central do método.

## Arquitetura

- `core/` → protocolo, wizard, metodologia, capacidades e modelo de evidência
- `workflows/` → instalação, novo teste, execução, auditoria e atualização
- `adapters/` → adaptações específicas por ambiente
- `integrations/` → integrações opcionais com fontes de design
- `personas/` → schema e exemplos de personas
- `templates/` → briefing, plano de teste e relatório
- `examples/` → exemplos completos

## Exemplo

Veja `examples/first-test.md` para um exemplo compacto de ponta a ponta.

## Idioma

A experiência do wizard é multilíngue e deve utilizar automaticamente o idioma do usuário, salvo quando solicitado de outra forma.

A documentação técnica interna permanece majoritariamente em inglês para facilitar portabilidade entre modelos, agentes e colaboração open source.

## Criado pela OutBoxLab

Synthetic Personas nasceu como uma metodologia aplicada de UX Research e evoluiu para um protocolo aberto para explorar conceitos, jornadas, wireframes e protótipos com participantes sintéticos assistidos por IA.

A **OutBoxLab** criou e mantém o protocolo e recebe experimentos da comunidade, críticas metodológicas, novos adapters e contribuições.

🌐 [outboxlab.com.br](https://outboxlab.com.br)

## Feedback

Este beta é intencionalmente público.

Experimente o protocolo em diferentes modelos, compartilhe casos de uso, questione a metodologia, reporte problemas ou proponha melhorias por meio das Issues e Pull Requests do GitHub.

## Licença

Synthetic Personas é distribuído sob a **Licença MIT**. Consulte `LICENSE`.

Copyright © 2026 OutBoxLab.

## Versão

`0.1.0-beta`
