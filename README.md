<h1 align="center"> OpsTask Manager 🚀 </h1>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Plataforma-Bubble.io-blue?style=for-the-badge&logo=bubble"/>
  <img src="https://img.shields.io/badge/Categoria-No--Code-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Instituição-UniFECAF-purple?style=for-the-badge"/>
</p>

> **Portal de gerenciamento de tarefas e comunicação interna projetado para otimizar o fluxo de equipes de Operações e TI.**

## 📖 Sobre o Projeto

O **OpsTask Manager** foi desenvolvido como Produto Mínimo Viável (MVP) para a disciplina de *Fundamentos de No-Code e Low-Code* da faculdade de Inteligência Artificial e Automação Digital. 
    
O objetivo central é resolver a descentralização de informações no dia a dia de times operacionais. Ao invés de demandas perdidas em e-mails e chats paralelos, a aplicação oferece um painel Kanban centralizado, garantindo rastreabilidade, controle de SLA e um histórico de comunicação atrelado a cada ticket de forma auditável.

## ✨ Funcionalidades Principais

- 🔐 **Autenticação e Perfis:** Sistema de login seguro e gerenciamento de conta (Nome, E-mail e Avatar).
- 📊 **Dashboard Kanban:** Painel interativo com status em tempo real (`Pendentes`, `Em Andamento`, `Concluídas`).
- 🎯 **Visão Individual:** Aba "Minhas Demandas" para foco exclusivo nos tickets atribuídos ao usuário logado.
- 💬 **Comunicação Integrada:** Sistema de comentários relacionais dentro de cada tarefa para registro de resolução da equipe.
- 🔍 **Busca e Filtros:** Pesquisa rápida de tickets para agilizar a operação.
- 📱 **Design Responsivo:** Interface adaptada para uso fluido em diferentes tamanhos de tela.

## 🛠️ Tecnologias Utilizadas

- **[Bubble.io](https://bubble.io/):** Plataforma *Full-stack No-Code* responsável pela interface (Front-end), lógica de negócios (Workflows) e hospedagem.
- **Bubble Built-in Database:** Banco de dados relacional nativo estruturando as entidades `UserProfile`, `Task` e `Comment`.

## 🚀 Como Acessar e Testar

1. **Acesse a aplicação:** [Clique aqui para abrir o OpsTask Manager](https://marcosdrjunior.bubbleapps.io/version-test/?debug_mode=true)
2. **Cadastro/Login:** Crie uma conta rapidamente ou utilize credenciais de teste.
3. **Exploração:**
   - No painel principal (Board), clique em **+ Nova Tarefa** para registrar uma demanda, definindo título, descrição, prioridade e prazo.
   - Mova os cards entre as colunas para testar a atualização de status em tempo real.
   - Clique em um card existente e adicione um comentário para visualizar a comunicação atrelada à tarefa.
   - Navegue até a aba **Perfil** para personalizar sua visualização no sistema.

## 🗄️ Arquitetura de Dados (Resumo)

O banco de dados relacional foi modelado para garantir a integridade da operação:
- `UserProfile`: Armazena dados do colaborador e sua função.
- `Task`: Entidade central com campos de status, prioridade e relacionamento com o `UserProfile` (Responsável).
- `Comment`: Entidade de comunicação com relacionamento obrigatório apontando para a tarefa de origem (`Task_Parent`), isolando o contexto do chat.

---
<p align="center">
  Desenvolvido por Marcos para validação prática de fundamentos No-Code.
</p>
