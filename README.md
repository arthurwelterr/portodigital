\# 🚀 Residência Porto Digital | Squad 24



Interface Web inteligente integrada à API do Google Gemini para processamento de requisições e automação de tarefas.



\---



\## 📋 Sobre o Projeto



Este projeto foi desenvolvido como parte do programa de residência tecnológica do \*\*Porto Digital\*\*. A aplicação consiste em um sistema web completo que utiliza inteligência artificial para otimizar fluxos de trabalho. 



A versão atual unifica o backend estruturado em Python com um frontend responsivo e dinâmico.



\---



\## 📁 Estrutura do Repositório



O repositório foi organizado seguindo as melhores práticas de mercado, separando o código-fonte executável dos arquivos de design e modelagem:



\*   \*\*`src/`\*\*: Contém o código-fonte ativo da aplicação (arquivos `app.py`, `main.py`, as páginas HTML e templates).

\*   \*\*`docs/`\*\*: Documentação técnica do projeto, contendo os protótipos de tela, diagramas do Draw.io e o script de modelagem do banco de dados (`projeto.sql`).



\---



\## 🛠️ Tecnologias Utilizadas



A stack principal do projeto foi escolhida para garantir performance e facilidade de integração:



\*   \*\*Backend:\*\* Python 3

\*   \*\*IA:\*\* Google Gemini API (Biblioteca `google-generativeai`)

\*   \*\*Frontend:\*\* HTML5, CSS3 e JavaScript (ES6)

\*   \*\*Banco de Dados:\*\* SQL (Modelagem lógica e física inclusa)



\---



\## ⚙️ Como Executar o Projeto



Siga o passo a passo abaixo para rodar a aplicação localmente na sua máquina:



\### 1. Pré-requisitos

Certifique-se de ter o \*\*Python 3\*\* instalado no seu sistema.



\### 2. Clonar o Repositório

Abra o terminal e execute o comando:

```bash

git clone \[https://github.com/arthurwelterr/portodigital.git](https://github.com/arthurwelterr/portodigital.git)

cd portodigital



\### 3. Instale as dependências

Instale a biblioteca oficial da API do Gemini e outras dependências que seu script necessite:

pip install google-generativeai



\### 4. Configurar a Chave da API (Segurança)

Crie um arquivo chamado .env na raiz do seu projeto (ele já está protegido no .gitignore para não vazar no GitHub) e adicione a sua chave do Gemini:

GEMINI\_API\_KEY=sua\_chave\_secreta\_aqui



\### 5. Configurar a Chave da API (Segurança)

Rode o arquivo principal do backend para subir o servidor:

python src/app.py

Abra o seu navegador e acesse o endereço local indicado no terminal (ex: http://localhost:5000 ou similar).

