# 🤖 DIO Agent

> Seu mentor de Inteligência Artificial para aprender mais e melhor na [DIO](https://dio.me), agora também especializado em cibersegurança.

O **DIO Agent** é um agente de IA que acompanha você na sua jornada de estudos. Ele conhece as experiências da DIO (Bootcamps, Formações, Cursos, Desafios e muito mais) e ajuda você a estudar com mais clareza, destravar desafios e entender qualquer conceito.

Além disso, conta com uma especialização em **cibersegurança**, voltada ao aprendizado de segurança da informação, análise de vulnerabilidades, avaliação de riscos e boas práticas de proteção de aplicações e sistemas.

E você não precisa instalar nada complicado. Em **3 passos simples**, seu mentor de IA estará pronto para usar.

---

## ✨ Antes de começar: dois conceitos rápidos

Para usar o DIO Agent, basta entender duas palavras. As duas estão no [Glossário completo](docs/glossary.md), mas aqui vai a versão rápida:

- 🧠 **Agente de IA:** um chatbot comum responde perguntas, como um buscador mais esperto. Um *agente* de IA vai além: ele lê, planeja e executa passos para te ajudar a alcançar um objetivo. É a diferença entre alguém que te explica o caminho e alguém que caminha junto com você. O DIO Agent é um agente desse tipo: um tutor particular que acompanha a sua evolução.

- 🖥️ **Harness:** é o programa onde a conversa com o agente acontece. Vale a comparação: o agente é o professor, e o harness é a sala de aula. O mesmo professor pode dar aula em salas diferentes. Por isso o DIO Agent funciona em qualquer harness: você escolhe a "sala" no Passo 1, e seu mentor continua o mesmo.

Pronto. Com isso já dá para começar.

---

## 🎯 O que o DIO Agent faz por você

| Você precisa de... | O DIO Agent... |
|--------------------|----------------|
| Saber por onde começar | Monta um plano de estudos no seu ritmo |
| Destravar um desafio | Te guia até a solução, sem entregar a resposta pronta |
| Entender um conceito | Explica de forma simples, com analogias e exemplos |
| Aprender cibersegurança | Ensina fundamentos de segurança da informação |
| Analisar vulnerabilidades | Ajuda a identificar, compreender, avaliar e priorizar vulnerabilidades |
| Melhorar a segurança de aplicações | Recomenda medidas de prevenção, mitigação e correção |

Ele conhece os formatos da DIO: Bootcamps, Formações, Acelerações, Cursos, English4Tech, Desafios de Código, Desafios de Projeto, Desafios Criativos, Lives e Mentorias. Assim, as recomendações sempre apontam para algo que você já tem na plataforma.

---

## 🔐 Especialização em Cibersegurança

O DIO Agent também atua como **mentor de cibersegurança**, auxiliando estudantes a compreender conceitos de segurança da informação e desenvolver conhecimentos práticos sobre proteção de sistemas e aplicações.

### 📚 Base de conhecimento

A especialização conta com uma base de conhecimento dedicada aos seguintes assuntos:

- Tríade CIA: confidencialidade, integridade e disponibilidade.
- Ameaças, vulnerabilidades e riscos.
- Avaliação de impacto, probabilidade e severidade.
- Boas práticas de segurança da informação.
- Prevenção e correção de vulnerabilidades.
- Desenvolvimento e manutenção de aplicações mais seguras.

Arquivo: `agent/knowledge/security-basics.md`

### 🛡️ Skill: Vulnerability Analysis

A skill `vulnerability-analysis` orienta o agente na análise de vulnerabilidades em aplicações, sistemas e infraestruturas.

Com essa especialização, o DIO Agent pode:

- Identificar e compreender possíveis vulnerabilidades.
- Analisar evidências e avaliar riscos.
- Considerar impacto, probabilidade e severidade.
- Priorizar problemas de segurança.
- Recomendar medidas de correção e mitigação.
- Orientar verificações após a implementação das correções.
- Documentar resultados de análises de segurança.

Arquivo: `skills/vulnerability-analysis/SKILL.md`

### ⚖️ Segurança e uso responsável

Todas as orientações de cibersegurança seguem princípios de uso ético e responsável:

- Verificar autorização e escopo antes de orientar testes.
- Trabalhar somente em ambientes próprios, laboratórios ou sistemas autorizados.
- Priorizar análises defensivas e medidas de proteção.
- Evitar ações destrutivas ou que possam causar indisponibilidade.
- Proteger senhas, tokens, chaves privadas e outras informações sensíveis.
- Não orientar invasões, roubo de credenciais ou exploração de sistemas sem autorização.

O objetivo é ensinar cibersegurança de forma prática, ética e responsável.

---

## 🚀 Comece em 3 passos

### 1️⃣ Instale um Harness

O harness é o programa que dá vida ao agente. Recomendamos o **Google Antigravity**, que tem limites de uso mais generosos para quem está começando. Mas qualquer harness moderno funciona.

| Harness | Documentação oficial |
|---------|----------------------|
| Google Antigravity (recomendado) | https://antigravity.google/docs |
| Claude Code | https://docs.claude.com/en/docs/claude-code |
| Codex | https://developers.openai.com/codex |
| OpenCode | https://opencode.ai/docs |
| Hermes | https://hermes-agent.nousresearch.com/docs |

Escolha um e siga o passo a passo da documentação oficial dele.

### 2️⃣ Configure o DIO Agent

Agora você vai baixar este repositório para o seu computador. Escolha a forma mais simples para você:

**Opção A: com Git**

```bash
git clone https://github.com/digitalinnovationone/dio-agent.git
```

**Opção B: baixando o .zip**

Na página do repositório no GitHub, clique no botão verde **Code** e depois em **Download ZIP**. Em seguida, extraia a pasta em um lugar fácil de encontrar.

Com o repositório baixado, abra a pasta `dio-agent` no harness que você instalou.

O harness lê automaticamente o arquivo `AGENTS.md` e o agente já sabe quem é, como deve se comportar e quais especializações pode utilizar.

> 🔄 **Fique de olho nas atualizações.** O projeto evolui com o tempo. De tempos em tempos, vale voltar ao repositório e pegar a versão mais recente.

### 3️⃣ Hands On!

Agora é só conversar. Você pode falar naturalmente, com suas próprias palavras. Mas, principalmente nas primeiras vezes, vale usar um modelo de prompt pronto.

**🗺️ Plano de estudos**

```text
Quero montar um plano de estudos (se possível, com materiais complementares).
- Meu objetivo: [ex: aprender mais sobre IA, ser dev back-end]
- Experiência ou carreira da DIO: [URL ou nome do bootcamp/formação]
- Meu nível hoje: [iniciante, intermediário, avançado]
- Tempo disponível: [ex: 1 hora por dia]
```

**🔓 Destravar desafio**

```text
Estou travado em um Desafio de Código, Projeto ou Criativo da DIO.
- O que o desafio pede: [descreva o enunciado]
- Onde eu travei: [explique a dificuldade]
- Meu código atual: [cole aqui, se for Desafio de Código]

Me ajuda a destravar sem dar a resposta pronta.
```

**💡 Explicar conceito**

```text
Me explica o conceito de [ex: API, laço de repetição, herança].
- Meu nível: [nunca vi, já ouvi falar, quero aprofundar]
- Onde apareceu: [ex: no curso X de um bootcamp]
```

**🔐 Analisar vulnerabilidade**

```text
Quero aprender a analisar uma possível vulnerabilidade de segurança.

- Sistema ou aplicação: [descreva o ambiente]
- Ambiente: [laboratório próprio, aplicação local ou ambiente autorizado]
- Objetivo: [entender, avaliar ou corrigir a vulnerabilidade]
- Evidências disponíveis: [descreva o comportamento observado]

Antes de orientar qualquer teste, verifique o contexto,
a autorização e o escopo.

Explique os riscos e recomende medidas de correção
de maneira didática e responsável.
```

Não precisa de comando especial nem de formato perfeito: o agente identifica a necessidade e utiliza a skill adequada.

---

## 🧩 As skills do agente

Uma **skill** é uma habilidade do agente, descrita em um guia passo a passo. O DIO Agent possui as seguintes especializações:

| Skill | Para que serve |
|-------|----------------|
| [Plano de estudos](skills/study-plan/SKILL.md) | Organiza o que estudar, em que ordem e em quanto tempo |
| [Destravar desafio](skills/unblock-challenge/SKILL.md) | Conduz você até a solução de um desafio, sem dar a resposta pronta |
| [Explicar conceito](skills/explain-concept/SKILL.md) | Explica conceitos de forma didática, com analogias e exemplos |
| [Pesquisa na web](skills/web-search/SKILL.md) | Busca informações atuais e verificáveis |
| [Análise de vulnerabilidades](skills/vulnerability-analysis/SKILL.md) | Identifica, compreende, avalia, prioriza e orienta a correção de vulnerabilidades |

Você não precisa chamar uma skill manualmente. O agente identifica o que você precisa e utiliza a especialização correspondente.

---

## 🗂️ Estrutura do repositório

```text
dio-agent/
├── README.md
├── AGENTS.md
├── CLAUDE.md
│
├── agent/
│   ├── persona.md
│   └── knowledge/
│       ├── dio-platform.md
│       ├── learning-experiences.md
│       └── security-basics.md
│
├── skills/
│   ├── README.md
│   ├── study-plan/
│   │   └── SKILL.md
│   ├── unblock-challenge/
│   │   └── SKILL.md
│   ├── explain-concept/
│   │   └── SKILL.md
│   ├── web-search/
│   │   └── SKILL.md
│   └── vulnerability-analysis/
│       ├── README.md
│       └── SKILL.md
│
└── docs/
    └── glossary.md
```

> 🔍 **Por que funciona em qualquer harness?** O coração do projeto é o arquivo `AGENTS.md`, um padrão aberto que harnesses modernos sabem ler. O `CLAUDE.md` apenas aponta para ele, permitindo que você use o harness que preferir.

---

## 📖 Glossário rápido

Termos como *agente*, *harness*, *skill* e *prompt* estão explicados com analogias simples no [Glossário completo](docs/glossary.md).

---

## 💬 Sobre este projeto

O DIO Agent foi criado para acompanhar estudantes desde o início dos Bootcamps e Formações da DIO.

Com a especialização em cibersegurança, o projeto amplia sua proposta educacional, oferecendo orientação sobre segurança da informação, análise de vulnerabilidades e desenvolvimento seguro.

A ideia é simples: aprender na era da IA fica mais fácil quando você tem um mentor disponível a qualquer hora.

Bons estudos, e vem com a gente. 🚀