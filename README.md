# 🐛 API de Gerenciamento de Reclamações de Bugs

API RESTful desenvolvida em Node.js com Express para registrar, consultar, atualizar e deletar relatos de bugs em jogos. O projeto utiliza armazenamento de dados em memória e a biblioteca nativa `crypto` para a geração automática de identificadores únicos (UUID v4).

---

## 📋 Atributos da Reclamação

Cada registro salvo na aplicação possui a seguinte estrutura:

* **`id`**: String (UUID v4 gerado automaticamente).
* **`titulo`**: Resumo da ocorrência.
* **`descricao`**: Detalhamento do problema.
* **`categoria`**: Classificação (ex: *Bug Visual*, *Física/Veículos*, *IA de NPCs*).
* **`autor`**: Nome do usuário que reportou.
* **`prioridade`**: Urgência (*Baixa*, *Média*, *Alta*, *Crítica*).
* **`status`**: Situação do chamado (*Aberta*, *Em Análise*, *Resolvida*).
* **`dataCriacao`**: Data de abertura gerada automaticamente no formato `DD/MM/AAAA`.

---

## 💻 Tecnologias Utilizadas

* **Node.js**: Ambiente de execução JavaScript.
* **Express**: Framework para gerenciamento de rotas e requisições HTTP.
* **Crypto**: Módulo nativo do Node.js para geração de UUIDs seguros.

---

## 🛠️ Como Executar o Projeto

1. **Clonar/Preparar a pasta do projeto**:
   ```bash
   mkdir api-reclamacoes
   cd api-reclamacoes


