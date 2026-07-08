# Forensics

Ferramenta de análise forense para Windows que lê o **BAM/DAM** (Background/Desktop Activity Moderator) do registro, mostrando quais executáveis rodaram, quando e por qual usuário.



## O que ele faz

- Lê o BAM/DAM **ao vivo** do sistema atual, ou de um **hive SYSTEM offline** (extraído de outra máquina/imagem forense)
- Resolve o caminho do executável (letra de unidade) quando possível
- Resolve o SID para nome de usuário
- Exporta os resultados em **CSV** e **JSON**
- Mostra arquivos deletados
- consulta o Sysmon (EventID 10) por acessos a um processo alvo ( HD.Player.exe)
- Detect de manual-mapped/injetado acessando o processo alvo
- Event 1102 (Security) / 104 (System) — log de eventos limpo manualmente
- Event 4616 (Security) — mudança manual do relógio do sistema
- Sysmon Event 8 — criação de thread remota em processo alvo (indício de injeção de código)
- Sysmon Event 7 — DLLs suspeitas carregadas no processo alvo



## Requisitos

- Windows 10 1709+ ou Windows 11
- Executar como **Administrador**
- A build mínima é a 16299 (Windows 10 versão 1709)




