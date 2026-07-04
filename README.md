# BamParser

Ferramenta de análise forense para Windows que lê o **BAM/DAM** (Background/Desktop Activity Moderator) do registro, mostrando quais executáveis rodaram, quando e por qual usuário.



## O que ele faz

- Lê o BAM/DAM **ao vivo** do sistema atual, ou de um **hive SYSTEM offline** (extraído de outra máquina/imagem forense)
- Resolve o caminho do executável (letra de unidade) quando possível
- Resolve o SID para nome de usuário
- Exporta os resultados em **CSV** e **JSON**



## Requisitos

- Windows 10 1709+ ou Windows 11
- Executar como **Administrador**




