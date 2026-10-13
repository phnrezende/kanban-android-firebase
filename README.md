# Kanban Android com Firebase

Aplicativo Android de quadro kanban para organizar tarefas em três colunas: **A fazer**, **Fazendo** e **Feito**. Cada usuário tem sua própria conta e suas tarefas ficam sincronizadas na nuvem.

## Funcionalidades

- Cadastro, login e recuperação de senha com **Firebase Authentication**
- Criação, edição e exclusão de tarefas
- Mudança de status entre as colunas
- Tarefas salvas por usuário no **Firebase Realtime Database**, atualizadas em tempo real

## Tecnologias

- Kotlin e XML
- Firebase Authentication e Realtime Database
- Navigation Component com Safe Args
- ViewModel, ViewBinding e ViewPager2
- Material Design (BottomSheet, Toolbar)

## Estrutura dos dados

```
task/
  {uid do usuário}/
    {id da tarefa}: { id, description, status }
```

## Como rodar

1. Clone o repositório e abra no Android Studio.
2. Crie um projeto no [Firebase](https://console.firebase.google.com/), ative **Authentication (e-mail e senha)** e o **Realtime Database**.
3. Baixe o `google-services.json` do seu projeto e coloque em `app/`.
4. Rode no emulador ou em um aparelho com Android 7.0 (API 24) ou superior.

## Autor

Pedro Henrique Rezende · [LinkedIn](https://www.linkedin.com/in/pedro-henrique-rezende-543588373/)
