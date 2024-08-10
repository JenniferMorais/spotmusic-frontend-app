# SpotMusic Frontend App

Este repositório contém o código fonte do aplicativo móvel da SpotMusic, desenvolvido em Flutter.

## Tecnologias Utilizadas

- **Flutter**: Framework para desenvolvimento de aplicativos móveis multiplataforma.
- **Dart**: Linguagem de programação usada pelo Flutter.
- **Provider**: Gerenciamento de estado.
- **HTTP**: Para comunicação com o backend via RESTful APIs.

## Como Executar

1. **Instalar as Dependências:**
   ```bash
   flutter pub get

# Estrutura de Branches para SpotMusic

Esta é a estratégia de branching que seguimos no desenvolvimento do SpotMusic.

## Branches Principais

- **main:** Este é o branch principal e sempre contém o código mais estável. As novas funcionalidades e correções de bugs devem ser integradas ao `main` através de pull requests.
- **stage:** Branch de homologação, onde novas funcionalidades são integradas e testadas antes de serem lançadas. As novas funcionalidades e correções de bugs devem ser integradas ao `stage` através de pull requests
- **develop:** Este branch é usado para o desenvolvimento contínuo e contém o código que está sendo testado e revisado antes de ser integrado a `stage`.

## Branches de Funcionalidade (Feature Branches)

- **Nomeação:** `feature/nome-da-funcionalidade`
- **Uso:** Criados a partir do branch `develop` para o desenvolvimento de novas funcionalidades. Após a conclusão, o branch deve ser mergeado de volta em `develop` e então deletado.

## Branches de Correção de Bug (Bugfix Branches)

- **Nomeação:** `bugfix/nome-da-correção`
- **Uso:** Criados a partir do branch `develop` (ou `main` se o bug for crítico). Após a correção, o branch deve ser mergeado de volta em `develop` ou `main` e então deletado.

## Branches de Hotfix (Hotfix Branches)

- **Nomeação:** `hotfix/nome-da-correção`
- **Uso:** Criados a partir de `main` para correções rápidas em produção. Após a correção, o branch deve ser mergeado de volta em `main` e `develop`.

## Como Criar um Branch

1. **Feature Branch:**
   ```bash
   git checkout -b feature/minha-funcionalidade
