# App FluxoLivre

Aplicativo em Flutter para gerenciamento de fluxo, desenvolvido como parte de um projeto de aprendizado.

## Visão Geral

O App FluxoLivre visa fornecer uma plataforma para usuários interagirem com um sistema de fluxo (detalhes específicos do fluxo a serem definidos/implementados). Atualmente, o aplicativo conta com funcionalidades de autenticação, cadastro de novos usuários e um painel administrativo.

## Funcionalidades Implementadas

*   **Autenticação:**
    *   Tela de Login (`/`)
    *   Serviço de autenticação (`AuthApiService`) para conectar com a API.
    *   Gerenciamento de estado do token com `AuthProvider`.
*   **Cadastro de Usuário:**
    *   Tela de Cadastro (`/novousuario`)
    *   Serviço para registro de novos usuários (`UserApiService`).
*   **Painel Administrativo (`/admin`):**
    *   Navegação para diferentes seções administrativas.
    *   **Gerenciamento de Usuários (`/users`):**
        *   Tela para listar usuários (atualmente com dados simulados).
        *   Layout estilizado com imagem de fundo e `Card`s para cada usuário.
        *   Botões de placeholder para editar e excluir usuários.
        *   Preparado para integração com API para busca de usuários.
    *   Seções para Relatórios e Configurações (ainda não implementadas).
*   **Navegação:**
    *   Rotas definidas em `app_fluxolivre.dart`.
*   **Conexão com API:**
    *   URL base da API configurada em `lib/src/utils/constants.dart` (`http://18.215.175.96:4040`).
    *   Serviços implementados para login e cadastro de usuários.

## Estrutura do Projeto

O projeto segue uma estrutura comum para aplicativos Flutter, organizada da seguinte forma:

*   `lib/src/pages/`: Contém as telas (widgets de rota) da aplicação.
*   `lib/src/widgets/`: Contém widgets reutilizáveis.
*   `lib/src/services/`: Contém a lógica de comunicação com a API.
*   `lib/src/providers/`: Contém os gerenciadores de estado (usando Provider).
*   `lib/src/models/`: Contém os modelos de dados.
*   `lib/src/utils/`: Contém utilitários, como constantes.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
