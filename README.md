# 🚀 Residência Porto Digital | Squad 24

Interface Web inteligente integrada à API do Google Gemini para processamento de requisições e automação de tarefas.

---

## 📋 Sobre o Projeto

Este projeto foi desenvolvido como parte do programa de residência tecnológica do **Porto Digital**. A aplicação consiste em um sistema web completo que utiliza inteligência artificial para otimizar fluxos de trabalho. 

A estrutura do projeto unifica um backend em Python com um frontend dinâmico e um banco de dados estruturado.

---

## 📁 Estrutura do Repositório

O repositório foi organizado separando os escopos do projeto para facilitar a manutenção e escalabilidade:

* **`backend/`**: Contém a lógica de servidor da aplicação em Python (arquivos `main.py` e `app.py`).
* **`frontend/`**: Interface do usuário desenvolvida com arquivos HTML (`index.html` e `template.html`).
* **`database/`**: Scripts de modelagem e criação do banco de dados (arquivo `projeto.sql`).
* **`docs/`**: Documentação técnica, protótipos de tela e diagramas do projeto.

---

## 🛠️ Tecnologias Utilizadas

A stack principal do projeto foi escolhida para garantir performance e facilidade de integração:

* **Backend:** Python 3
* **IA:** Google Gemini API (Biblioteca `google-generativeai`)
* **Frontend:** HTML5, CSS3 e JavaScript (ES6)
* **Banco de Dados:** SQL (Modelagem inclusa)

---

## ⚙️ Como Executar o Projeto

Siga o passo a passo abaixo para rodar a aplicação localmente na sua máquina:

### 1. Pré-requisitos
Certifique-se de ter o **Python 3** instalado no seu sistema.

### 2. Clonar o Repositório
```bash
Abra o terminal e execute o comando:
git clone [https://github.com/arthurwelterr/portodigital.git](https://github.com/arthurwelterr/portodigital.git)
cd portodigital
```

### 3. Clonar o Repositório
Instale a biblioteca oficial da API do Gemini e outras dependências necessárias:
```bash
pip install google-generativeai
```

### 4. Configurar a Chave da API (Segurança)
Crie um arquivo chamado .env na raiz do seu projeto (ele já está protegido no .gitignore para não vazar no GitHub) e adicione a sua chave do Gemini:
```bash
GEMINI_API_KEY=sua_chave_secreta_aqui
```

### 5. Executar a Aplicação
Navegue até a pasta do backend e rode o arquivo principal para subir o servidor:
```bash
cd backend
python app.py
```
Abra o seu navegador e acesse o endereço local indicado no terminal (ex: http://localhost:5000 ou similar).

---

### 🔄 Como enviar a atualização:

Abra o arquivo `README.md` no seu computador, cole esse texto novo, salve e digite os comandos no terminal:

```bash
git add README.md
git commit -m "Docs: atualiza estrutura de pastas no README"
git push origin main
```
