# 🚀 **Guia Rápido de Execução – Bolso Aberto**

> **Projeto Acadêmico**
> Documento elaborado para orientar a instalação, execução e validação do aplicativo *Bolso Aberto*.



## ⚡ **Configuração em 3 Etapas**

### 1️⃣ **Preparar o Ambiente**
Verifique se o **Node.js (versão 18 ou superior)** está instalado:
node --version

Caso não esteja instalado, baixe em:
[https://nodejs.org/](https://nodejs.org/)

### 2️⃣ **Instalar Dependências**
No terminal, acesse a pasta do projeto:
cd controle-financeiro

Instale as dependências necessárias:
npm install

### 3️⃣ **Executar a Aplicação**
Inicie o servidor de desenvolvimento:
npm run dev

Acesse no navegador:
**[http://localhost:8080](http://localhost:8080)**



## 🎯 **Primeiro Uso – O que verificar**
### 📝 **Checklist Inicial**
* [ ] Projeto abrindo em **[http://localhost:8080](http://localhost:8080)**
* [ ] Interface carregando sem erros
* [ ] Alternância de tema (claro/escuro) funcionando
* [ ] Botão flutuante “+” visível



## 📊 **Testando Funcionalidades Principais**
### 1. **Adicionar uma transação**
* Clique no **botão “+”** (canto inferior direito)
* Escolha **Receita**
* Exemplo: *Salário* → R$ 3.000
* O saldo deve atualizar automaticamente

### 2. **Criar uma meta financeira**
* Acesse **Metas Financeiras**
* Clique em **Nova Meta**
* Exemplo:
  * Nome: *Viagem*
  * Valor: **R$ 2.000**
* A barra de progresso deve ser exibida

### 3. **Verificar elementos de gamificação**
* Observe o card **Nível do Usuário**
* Ao completar metas, o usuário ganha **XP**
* Conquistas também podem ser desbloqueadas



🛠️ **Solução de Problemas Comuns**
### ❌ **“npm não encontrado”**
Instale o Node.js:
[https://nodejs.org/](https://nodejs.org/)
Reinicie o terminal.

### ❌ **Erro: “Porta 8080 em uso”**
Execute em outra porta:
npm run dev -- --port 3000

### ❌ **Aplicação não inicia**
Reinstale dependências:
rm -rf node_modules
npm install
npm run dev

### ❌ **Tela branca no navegador**
* Abra o console (F12) e verifique erros
* Observe também o terminal onde o servidor está rodando



## 📋 **Comandos Úteis**
**Desenvolvimento**
npm run dev

**Build de Produção**
npm run build
npm run preview

**Manutenção / Qualidade**
npm run lint



## 🗂️ **Estrutura Rápida do Projeto**
📁 src/
  ├── 📁 components/   → Componentes de interface
  ├── 📁 hooks/         → Lógica e estados reutilizáveis
  ├── 📁 pages/         → Páginas principais (Index.tsx, etc.)
  ├── 📁 types/         → Definições TypeScript
  └── 📄 index.css      → Estilos globais



## 💡 **Boas Práticas**
* Utilize **npm run dev** durante o desenvolvimento
* Evite editar arquivos dentro de **node_modules/**
* Modificações salvam e recarregam automaticamente
* Use o console (F12) para depuração
* Pressione **Ctrl + C** no terminal para encerrar o servidor

🎉 **Pronto! O aplicativo está preparado.