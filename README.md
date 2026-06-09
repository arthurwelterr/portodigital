# 🚀 Residência Porto Digital | Squad 24

Sistema web inteligente de geração automática de criativos para redes sociais, utilizando **Google Gemini AI + Python + Playwright**, capaz de transformar um tema em um post visual pronto (1080x1080).

---

## 📋 Sobre o Projeto

Este projeto foi desenvolvido no programa de residência tecnológica do **Porto Digital**.

A aplicação funciona como um **gerador automático de criativos para redes sociais**, onde o usuário informa um tema e o sistema gera automaticamente um post completo, incluindo:

* Ideias e keywords com IA (Google Gemini)
* Prompt de imagem
* Copy para redes sociais
* Geração de imagem via serviço externo
* Renderização de um post final em HTML (1080x1080)
* Exportação da imagem final em PNG

---

## 🧠 Fluxo da Aplicação

1. O usuário envia um tema via API (`/gerar`).
2. O Backend processa o tema com o **Google Gemini**.
3. A IA retorna: Keywords, Prompt de imagem, Texto do post e Descrição.
4. O sistema gera uma imagem via URL externa.
5. O **Playwright** renderiza um HTML (`template.html`).
6. O sistema exporta um PNG final pronto para uso.

---

## 📁 Estrutura do Repositório

```text
backend/
├── app.py              # API Flask principal
├── main.py             # Lógica de IA e geração de criativos
└── template.html       # Template HTML usado no render do post

frontend/
├── index.html          # Interface do usuário
└── template.html       # Template visual do post (usado pelo backend)

database/
└── projeto.sql         # Estrutura do banco de dados (se aplicável)

docs/
└── documentação técnica e protótipos

```

---

## 🛠️ Tecnologias Utilizadas

### Backend & IA

* Python 3.10+
* Flask & Flask-CORS
* Google Gemini API (`google-genai`)

### Automação & Renderização

* Playwright (Chromium)
* HTML5 / CSS3 + Base64 image embedding
* Renderização de imagem via screenshot automatizado

### Frontend

* HTML5 / CSS3 / JavaScript (Vanilla)

---

## ⚙️ Como Executar o Projeto

### 1. Pré-requisitos

* Python 3.10 ou superior
* Gerenciador de pacotes `pip`
* Chromium (instalado via Playwright)

### 2. Clonar o repositório

```bash
git clone [https://github.com/arthurwelterr/portodigital.git](https://github.com/arthurwelterr/portodigital.git)
cd portodigital

```

### 3. Instalar as dependências

```bash
pip install flask flask-cors google-genai playwright
python -m playwright install chromium

```

### 4. Configurar a variável de ambiente (API Key)

Substitua `"SUA_CHAVE_AQUI"` pela sua chave real da API do Gemini.

#### No Linux / Git Bash:

```bash
export GEMINI_API_KEY="SUA_CHAVE_AQUI"

```

#### No Windows (PowerShell):

```powershell
$env:GEMINI_API_KEY="SUA_CHAVE_AQUI"

```

#### No Windows (Prompt de Comando - CMD):

```cmd
set GEMINI_API_KEY=SUA_CHAVE_AQUI

```

### 5. Executar o backend

```bash
cd backend
python app.py

```

A API estará disponível em: `http://127.0.0.1:5000`

---

## 📡 Rotas da API

### 🔹 Gerar Criativo

* **Endpoint:** `/gerar`
* **Método:** `POST`
* **Headers:** `Content-Type: application/json`

#### Corpo da requisição (JSON):

```json
{
  "tema": "marketing digital com IA",
  "brand": "Minha Marca"
}

```

#### Resposta:

* Retorna o arquivo de imagem no formato **PNG** gerado automaticamente, pronto para download ou visualização direta.
