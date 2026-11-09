# Fundamentos de Segurança da Informação

Este documento reúne conceitos fundamentais de cibersegurança para apoiar o DIO Agent em análises de vulnerabilidades, avaliação de riscos e recomendações de segurança.

O agente deve utilizar esta base de conhecimento para explicar problemas técnicos de maneira didática, fundamentar suas análises e orientar boas práticas defensivas.

## 1. Segurança da Informação

Segurança da informação é o conjunto de práticas, políticas e tecnologias utilizadas para proteger informações e sistemas contra acessos não autorizados, alterações indevidas, perdas e interrupções.

Seus principais objetivos são preservar a confidencialidade, a integridade e a disponibilidade das informações.

## 2. Tríade CIA

A tríade CIA representa três pilares fundamentais da segurança da informação.

### 2.1 Confidencialidade (Confidentiality)

Garante que informações sejam acessadas somente por pessoas, sistemas ou processos autorizados.

Exemplos de ameaças:

- Vazamento de senhas.
- Exposição de dados pessoais.
- Acesso indevido a arquivos.
- Falhas de controle de acesso.

Boas práticas:

- Utilizar autenticação multifator (MFA).
- Aplicar o princípio do menor privilégio.
- Criptografar informações sensíveis.
- Proteger credenciais e tokens.

### 2.2 Integridade (Integrity)

Garante que informações permaneçam corretas, completas e protegidas contra modificações não autorizadas.

Exemplos de ameaças:

- Alteração indevida de registros.
- Manipulação de transações.
- Modificação de arquivos.
- Injeção de comandos em aplicações.

Boas práticas:

- Implementar controles de autorização.
- Utilizar mecanismos de validação de dados.
- Registrar alterações importantes em logs.
- Utilizar hashes para verificar integridade quando apropriado.

### 2.3 Disponibilidade (Availability)

Garante que sistemas, serviços e informações estejam disponíveis quando necessários.

Exemplos de ameaças:

- Ataques de negação de serviço (DoS).
- Falhas de hardware.
- Interrupções de rede.
- Erros de configuração.
- Ransomware.

Boas práticas:

- Realizar backups periódicos.
- Implementar redundância.
- Monitorar serviços e infraestrutura.
- Manter planos de recuperação de desastres.
- Atualizar sistemas e componentes.

## 3. Conceitos fundamentais

### 3.1 Ativo

É qualquer recurso que tenha valor para uma organização ou usuário.

Exemplos:

- Servidores.
- Aplicações.
- Bancos de dados.
- Informações pessoais.
- Equipamentos de rede.
- Credenciais de acesso.

### 3.2 Ameaça

É uma circunstância, evento ou agente com potencial para causar danos a um ativo.

Exemplos:

- Malware.
- Engenharia social.
- Ataques de força bruta.
- Erros humanos.
- Desastres físicos.

### 3.3 Vulnerabilidade

É uma fraqueza em um sistema, aplicação, processo ou configuração que pode ser explorada por uma ameaça.

Exemplos:

- SQL Injection.
- Cross-Site Scripting (XSS).
- Senhas fracas.
- Software desatualizado.
- Permissões excessivas.
- Configurações inseguras.

### 3.4 Exploração

É o aproveitamento de uma vulnerabilidade para provocar um comportamento não autorizado ou indesejado em um sistema.

Uma vulnerabilidade pode existir sem ter sido explorada.

### 3.5 Risco

É a possibilidade de uma ameaça explorar uma vulnerabilidade e causar impacto negativo sobre um ativo.

A avaliação de risco deve considerar:

- Valor e importância do ativo.
- Existência de vulnerabilidades.
- Probabilidade de exploração.
- Impacto potencial.
- Controles de segurança existentes.

### 3.6 Impacto

Representa as consequências que um incidente de segurança pode provocar.

Pode envolver:

- Perda ou exposição de informações.
- Alteração indevida de dados.
- Interrupção de serviços.
- Prejuízo financeiro.
- Danos à reputação.
- Consequências legais e regulatórias.

### 3.7 Probabilidade

Representa a possibilidade de uma ameaça explorar determinada vulnerabilidade.

Considere fatores como exposição, facilidade de exploração, complexidade técnica, autenticação exigida e controles existentes.

## 4. Severidade das vulnerabilidades

A severidade representa o nível de gravidade técnica de uma vulnerabilidade.

Classificações utilizadas:

| Nível | Descrição |
|---|---|
| Crítica | Possibilidade de comprometimento muito grave. |
| Alta | Pode provocar danos significativos. |
| Média | Pode causar impacto moderado. |
| Baixa | Impacto limitado ou exploração mais restrita. |
| Informativa | Informação relevante sem falha confirmada. |

A classificação deve ser justificada com base em evidências.

Quando aplicável, utilizar o CVSS (Common Vulnerability Scoring System) como referência complementar.

Não confundir severidade técnica com risco de negócio: o contexto do ativo também influencia a prioridade de correção.

## 5. Vulnerabilidades comuns em aplicações

### 5.1 SQL Injection (SQLi)

Ocorre quando dados fornecidos pelo usuário são incorporados indevidamente a comandos SQL.

Possíveis consequências:

- Acesso não autorizado a registros.
- Exposição de informações.
- Alteração ou exclusão de dados.

Prevenção:

- Utilizar consultas parametrizadas.
- Evitar concatenar entradas diretamente em comandos SQL.
- Aplicar privilégios mínimos ao usuário do banco.
- Validar entradas de acordo com o contexto.

### 5.2 Cross-Site Scripting (XSS)

Ocorre quando uma aplicação permite a execução de scripts maliciosos no navegador de outros usuários.

Possíveis consequências:

- Roubo de sessão.
- Manipulação da interface.
- Ações indevidas em nome do usuário.

Prevenção:

- Aplicar codificação de saída contextual.
- Validar e tratar entradas.
- Utilizar Content Security Policy (CSP) como camada adicional.
- Configurar cookies com atributos de segurança.

### 5.3 Quebra de controle de acesso

Ocorre quando usuários conseguem acessar recursos ou executar operações além das permissões concedidas.

Prevenção:

- Implementar autorização no servidor.
- Aplicar o princípio do menor privilégio.
- Verificar permissões em cada operação sensível.
- Não confiar exclusivamente em controles visuais no navegador.

### 5.4 Autenticação insegura

Ocorre quando mecanismos de identificação e autenticação apresentam falhas.

Exemplos:

- Senhas fracas.
- Ausência de proteção contra tentativas automatizadas.
- Recuperação de senha insegura.
- Sessões mal configuradas.

Prevenção:

- Implementar MFA quando possível.
- Armazenar senhas com algoritmos apropriados de hash, como Argon2id.
- Aplicar limitação de tentativas.
- Proteger sessões e cookies.

### 5.5 Configuração insegura

Ocorre quando sistemas, aplicações ou serviços utilizam configurações inadequadas.

Exemplos:

- Credenciais padrão.
- Serviços desnecessariamente expostos.
- Diretórios com permissões excessivas.
- Mensagens de erro que revelam informações internas.

Prevenção:

- Desabilitar serviços desnecessários.
- Revisar permissões.
- Remover configurações padrão.
- Aplicar atualizações de segurança.
- Utilizar configurações seguras desde a instalação.

## 6. Boas práticas de segurança

### Gestão de atualizações

Manter sistemas operacionais, bibliotecas, frameworks e aplicações atualizados para reduzir a exposição a vulnerabilidades conhecidas.

### Controle de acesso

Aplicar o princípio do menor privilégio: cada usuário ou processo deve possuir apenas as permissões necessárias.

### Senhas e autenticação

- Utilizar senhas fortes e exclusivas.
- Preferir gerenciadores de senhas.
- Habilitar autenticação multifator.
- Nunca armazenar senhas em texto puro.

### Proteção de dados

- Criptografar informações sensíveis.
- Proteger dados durante transmissão e armazenamento.
- Evitar registrar segredos em logs.
- Restringir o acesso a informações confidenciais.

### Monitoramento

- Registrar eventos relevantes.
- Monitorar atividades suspeitas.
- Acompanhar tentativas de autenticação.
- Investigar comportamentos anormais.

### Backup e recuperação

- Realizar backups periódicos.
- Manter cópias protegidas contra alterações indevidas.
- Testar regularmente a restauração.
- Documentar procedimentos de recuperação.

## 7. Referências de segurança

O agente pode utilizar as seguintes referências para aprofundar suas análises:

- OWASP Top 10: categorias importantes de riscos de segurança em aplicações web.
- OWASP Web Security Testing Guide: orientação para testes de segurança em aplicações.
- CWE: catálogo de tipos de fraquezas em software e hardware.
- CVE: identificadores públicos de vulnerabilidades conhecidas.
- CVSS: sistema de pontuação de severidade de vulnerabilidades.
- MITRE ATT&CK: base de conhecimento de táticas e técnicas utilizadas em ataques cibernéticos.
- NIST Cybersecurity Framework: estrutura de referência para gestão de riscos de cibersegurança.

## 8. Diretrizes para o DIO Agent

Ao utilizar esta base de conhecimento, o agente deve:

1. Diferenciar ameaça, vulnerabilidade, exploração e risco.
2. Relacionar os problemas identificados aos pilares da tríade CIA.
3. Avaliar impacto e probabilidade antes de classificar a severidade.
4. Fundamentar suas conclusões em evidências.
5. Recomendar medidas preventivas e corretivas.
6. Priorizar a proteção de ambientes e dados.
7. Explicar conceitos técnicos de maneira acessível.
8. Reconhecer quando não existem informações suficientes para uma conclusão.

A segurança deve ser tratada como um processo contínuo de identificação, prevenção, correção e melhoria.