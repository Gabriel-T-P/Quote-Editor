# Projeto Turbo Rails — Editor de Cotações

Este projeto é uma aplicação Ruby on Rails 7 que implementa um **editor de cotações (quote editor)** com funcionalidades reativas utilizando **Turbo Rails**, conforme apresentado no tutorial gratuito do Hotrails.

## Sobre o Tutorial

O tutorial **Turbo Rails** ensina como usar o `turbo-rails` (biblioteca incluída por padrão no Rails 7) para criar aplicações de página única (SPA-like), com pouca ou nenhuma necessidade de JavaScript personalizado.

O que é implementado:

- Um controlador CRUD simples para o modelo `Quote`
- Organização de CSS com metodologia BEM
- **Turbo Drive** — acelera navegação interceptando cliques e submissões de formulários e transformando-os em requisições AJAX
- **Turbo Frames** e **Turbo Streams** — para fragmentar páginas em componentes independentes e fornecer atualizações em tempo real com Action Cable
- Flash messages animadas com Stimulus
- Tratamento de estados vazios e mensagens de interface com Turbo
- Funcionalidade de cálculo dinâmico do total da cotação quando itens são adicionados, atualizados ou removidos

## Objetivo do Projeto

Este projeto replica o tutorial **Turbo Rails** do Hotrails, implementando um editor de cotações totalmente funcional:

- Permite criar, editar e remover **quotes**, **datas** e **itens**.
- Ao interagir com a aplicação (por exemplo, adicionar um item ou editar uma data), a interface se atualiza sem recarregar a página, graças ao uso de Turbo.
- O total da cotação é atualizado dinamicamente conforme os itens são manipulados.

## Como Começar

1. Clone este repositório.
2. No Gemfile, certifique-se de usar a versão compatível do `turbo-rails`:
    ```ruby
    gem "turbo-rails", "~> 1.0"
    ```
3. Execute:
    ```bash
    bundle install
    bin/setup
    bin/dev
    ```
   Isso vai instalar dependências, criar o banco de dados, executar migrações e iniciar o servidor com compilação automática de assets.
4. Acesse `http://localhost:3000` e explore o editor de cotações.

---

## Referência

Baseado no **Turbo Rails Tutorial** disponível em [Hotrails.dev](https://www.hotrails.dev/turbo-rails).

---
