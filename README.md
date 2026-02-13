# React + TypeScript + Vite
# ✅ Todo List App

Aplicação de lista de tarefas construída com **React + TypeScript + Vite** e estilizada com **Tailwind CSS v4**.

## 📸 Visão geral

Este projeto permite:

- Adicionar novas tarefas.
- Marcar tarefas como concluídas.
- Filtrar tarefas por status (**All**, **Active**, **Completed**).
- Limpar tarefas concluídas com um clique.
- Alternar entre tema **dark** e **light**.

As tarefas iniciais são carregadas de forma assíncrona (simulando uma chamada de API).

## 🧱 Tecnologias
- React 19
- TypeScript
- Vite
- Tailwind CSS 4

## 🚀 Como executar o projeto

- Node.js 18+ (recomendado)
- npm
### Instalação
```bash
npm install
```
### Ambiente de desenvolvimento
```bash
npm run dev
```

A aplicação ficará disponível em `http://localhost:5173`.

### Build de produção
```bash
npm run build
```
### Preview da build
```bash
npm run preview
```
### Lint
```bash
npm run lint

## 📁 Estrutura principal

```text
src/
  components/
    TodoContainer/
    TodoForm/
    TodoHeader/
    TodoList/
  contexts/
    ThemeContext.ts
    ThemeProvider.tsx
    theme.ts
  hooks/
    useTodo.ts
  styles/
    globals.css
  App.tsx
  main.tsx
```

## 🧠 Regras de negócio implementadas

- O hook `useTodo` centraliza o estado da lista, filtro e ações.
- Ao adicionar uma tarefa, o filtro volta para `all`.
- O botão de conclusão alterna o estado da tarefa (`completed`).
- `Clear Completed` remove somente tarefas já concluídas.

## 🎨 Temas

A troca de tema é feita via `ThemeContext` + `ThemeProvider`, e os estilos variam com base no tema atual.

## 📝 Licença

Este projeto está sem licença definida no momento.