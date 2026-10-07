# Arquitetura

## Visão geral

O Engineering Toolkit separa a interoperabilidade em camadas para reduzir o acoplamento entre o formato de origem e a API do ambiente de destino.

### Contratos

Define os modelos utilizados na representação intermediária dos dados de tubulação.

### Core

Responsável por interpretação, normalização, topologia, validações geométricas, resolução de catálogo e preparação do plano de execução.

### UI

Fornece os fluxos de seleção de arquivos, pré-validação, acompanhamento e geração de relatórios.

### E3D

Isola as operações dependentes das APIs AVEVA e aplica a política de criação controlada, leitura de retorno e reversão.

### Harness

Executa testes e regressões fora da interface principal, permitindo validar regras sem depender de interação manual.

## Princípio de segurança

A arquitetura evita considerar "objeto desenhado" como sinônimo de "objeto tecnicamente compatível". A criação depende da combinação entre topologia, geometria, catálogo e validação posterior.
