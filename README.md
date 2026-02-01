# 🚀 Projeto Integrado: Python + HTML/Tailwind

Este documento é o guia oficial para todos os membros da equipe. Aqui você aprenderá como configurar seu ambiente e como usar o Git para que possamos trabalhar juntos sem apagar o código uns dos outros.

---

## 📁 1. Organização do Projeto (Onde colocar seus arquivos)

Para o projeto funcionar, precisamos respeitar estas pastas:

* 📂 **app/templates/**: AQUI entra o seu trabalho de **Frontend**. Coloque seus arquivos `.html` aqui.
* 📂 **app/static/**: Coloque aqui seus ativos que não mudam (Imagens na pasta `/img`, JavaScript na pasta `/js`).
* 📂 **app/routes/**: AQUI entra o trabalho de **Backend**. Cada módulo de Python deve ficar aqui (ex: `pagamentos.py`).
* 📄 **run.py**: O arquivo que "liga" o site.
* 📄 **.env**: Arquivo secreto para as senhas do Supabase e Mercado Pago. **NUNCA** suba este arquivo para o GitHub.

---

## 🛠️ 2. Configuração Inicial (Primeira vez)

Cada membro deve fazer isso **apenas uma vez**:

1.  **Instalar o Git**: [Clique aqui para baixar](https://git-scm.com/).
2.  **Configurar seu nome e e-mail** (Abra o terminal e digite):
    ```bash
    git config --global user.name "Seu Nome"
    git config --global user.email "seu-email@exemplo.com"
    ```
3.  **Clonar o repositório**:
    ```bash
    git clone https://github.com/alecarvalho950/WolfScale.git
    ```
4.  **Criar o Ambiente Python**:
    ```bash
    python -m venv venv
    # Ativar (Windows): venv\Scripts\activate
    # Ativar (Mac/Linux): source venv/bin/activate
    pip install -r requirements.txt
    ```

---

## 🌿 3. O Fluxo Diário (Como trabalhar sem erros)

**REGRA DE OURO:** A branch `main` é o nosso produto final. Ninguém mexe nela diretamente. Trabalhamos em "galhos" (branches).

### Passo 1: Começando uma tarefa
Antes de escrever qualquer código, garanta que você tem o código mais recente e crie sua branch:
```bash
git checkout main          # Vai para a branch principal
git pull origin main       # Baixa as novidades que seus colegas fizeram
git checkout -b minha-tarefa  # Cria sua própria área de trabalho