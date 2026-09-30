# DisplayCSV

Aplicação web desenvolvida em **Python com Flask** para upload e visualização de arquivos CSV diretamente pelo navegador.

O projeto foi desenvolvido como prática de **desenvolvimento web com Python, manipulação de dados e deploy de uma aplicação em nuvem utilizando o Microsoft Azure**.

---

## 🚀 Tecnologias

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Azure](https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

- **Python** — Linguagem de programação utilizada no desenvolvimento
- **Flask** — Micro-framework web para criação da aplicação
- **Pandas** — Leitura, manipulação e processamento dos arquivos CSV
- **HTML/CSS** — Estrutura e estilização das páginas web
- **Microsoft Azure** — Hospedagem e deploy da aplicação em nuvem

---

## 📌 Sobre o projeto

O **DisplayCSV** permite que o usuário envie um arquivo `.csv` através de uma interface web e visualize seu conteúdo de forma clara e estruturada diretamente no navegador.

Após o upload, a aplicação utiliza o **Pandas** para ler o arquivo e transformar os dados em uma tabela HTML interativa para exibição.

Além disso, a aplicação conta com tratamento automático para diferentes codificações de caracteres (`UTF-8`, `latin1`, `ISO-8859-1`), garantindo que arquivos com acentuação e caracteres especiais sejam lidos corretamente.

---

## ✨ Funcionalidades

- 📂 **Upload de arquivos CSV**: Envio simples através de formulário web.
- 📊 **Visualização em Tabela**: Exibição limpa dos dados diretamente na página.
- 🔤 **Tratamento de Encoding**: Suporte automático a múltiplos padrões de codificação de texto.
- ☁️ **Deploy em Nuvem**: Aplicação publicada no ambiente do Microsoft Azure.

---

## ⚙️ Como funciona

O fluxo de processamento da aplicação segue as seguintes etapas:

```text
Usuário
   │
   ▼
Seleciona um arquivo CSV
   │
   ▼
Upload para a aplicação Flask
   │
   ▼
Pandas realiza a leitura
   │
   ▼
Dados são convertidos para HTML
   │
   ▼
Tabela exibida no navegador
```

---

## 📁 Estrutura do projeto

```text
displaycsv/
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── templates/
    ├── index.html
    └── display.html
```

### Principais arquivos

| Arquivo | Descrição |
|---|---|
| `app.py` | Código principal da aplicação Flask e lógica de leitura dos arquivos CSV |
| `requirements.txt` | Lista de dependências e bibliotecas Python necessárias |
| `templates/index.html` | Página inicial contendo o formulário de upload de arquivo |
| `templates/display.html` | Página responsável por renderizar a tabela com os dados |
| `.gitignore` | Arquivo que especifica quais arquivos/diretórios o Git deve ignorar |

---

## 💻 Como executar localmente

### 1. Clone o repositório
```bash
git clone https://github.com/Tkailaine/displaycsv.git
cd displaycsv
```

### 2. Crie um ambiente virtual
```bash
python -m venv venv
```

### 3. Ative o ambiente virtual

- **Windows:**
  ```powershell
  venv\Scripts\activate
  ```

- **Linux / macOS:**
  ```bash
  source venv/bin/activate
  ```

### 4. Instale as dependências
```bash
pip install -r requirements.txt
```

### 5. Execute a aplicação
```bash
python app.py
```

A aplicação estará disponível no seu navegador em:
👉 **[http://127.0.0.1:5000](http://127.0.0.1:5000)**

---

## 📄 Formato do arquivo

A aplicação está configurada para processar arquivos CSV separados por ponto e vírgula (`;`).

**Exemplo de arquivo `dados.csv`:**
```csv
Nome;Idade;Cidade
Maria;25;São Paulo
João;31;Campinas
Ana;28;Santos
```

Após realizar o upload, os dados são processados e apresentados formatados em uma tabela no navegador.

---

## ☁️ Deploy no Microsoft Azure

A aplicação foi publicada utilizando o **Microsoft Azure App Service (Web App)**.

### Fluxo de Deploy:

```text
GitHub
   │
   ▼
Código da aplicação
   │
   ▼
Azure App Service
   │
   ▼
Aplicação Flask publicada
```

Durante a configuração do recurso no Azure:
- Foi criado e utilizado um **Resource Group** dedicado para a organização dos recursos da aplicação.
- A integração contínua permite atualizar a aplicação online a partir das alterações enviadas ao repositório.

🔗 **Aplicação online:** [DisplayCSV no Azure](https://displaycsvapplication-gfc2hxhme0apavds.brazilsouth-01.azurewebsites.net/)

---

## 🎯 Objetivo do projeto

O projeto foi desenvolvido com foco prático para consolidar conhecimentos em:

- Desenvolvimento web com **Python** e micro-framework **Flask**
- Manipulação e tratamento de dados com **Pandas**
- Manipulação de uploads de arquivos e encoding de caracteres
- Versionamento de código com **Git e GitHub**
- Conceitos de computação em nuvem e publicação utilizando **Microsoft Azure**

---

## 👩‍💻 Autora

**Thaissa Kailaine**

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Tkailaine)

*Projeto desenvolvido para fins de estudo e prática em desenvolvimento de software e computação em nuvem.*
