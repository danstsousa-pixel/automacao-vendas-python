# Automação de Indicadores de Vendas com Python

## Sobre o Projeto
Este projeto foi desenvolvido para resolver um problema real de negócios: o tempo gasto com a compilação manual de dados e envio de relatórios rotineiros. 

O script automatiza o processo de ponta a ponta: ele processa uma base de dados de vendas, calcula os principais indicadores (Faturamento Total e Quantidade de Produtos Vendidos) e dispara um e-mail com o resumo gerencial de forma 100% autônoma, utilizando a biblioteca nativa `smtplib` do Python.

## Principais Funcionalidades

* **Processamento de Dados:** Leitura e cálculo de indicadores utilizando pandas.
* **Automação de E-mail:** Integração com o servidor SMTP do Gmail para envio automatizado.
* **Segurança de Credenciais:** Implementação da biblioteca `python-dotenv` para proteger informações sensíveis (e-mails e senhas de app) através de variáveis de ambiente, seguindo as melhores práticas de desenvolvimento.

## Tecnologias Utilizadas

* **Python 3**
* **Jupyter Notebook** (Ambiente de desenvolvimento iterativo)
* **Pandas** (Análise e manipulação de dados)
* **Smtplib & Email.message** (Protocolos de envio de e-mail)
* **Python-dotenv** (Gestão de variáveis de ambiente)

## Como Executar o Projeto
1. Clone o repositório:
   
```
git clone https://github.com/danstsousa-pixel/automacao-vendas-python.git
cd automacao-vendas-python
```

2. Instale as dependências:

```
pip install pandas python-dotenv jupyter
```

3. Configure as Variáveis de Ambiente:
   
Para rodar este projeto na sua máquina, você precisará configurar as suas próprias credenciais de e-mail.
Crie um arquivo chamado .env na raiz do projeto e adicione as seguintes variáveis:

```
EMAIL=seu_email@gmail.com
SENHA_APP=sua_senha_de_app_do_google
EMAIL_DESTINO=email_do_destinatario@gmail.com
```
(Nota: O arquivo .env está adicionado ao .gitignore neste repositório para garantir a segurança das credenciais).

4. Execute o projeto:
   
Como o código foi desenvolvido em blocos interativos, inicie o ambiente do Jupyter pelo terminal:

```
jupyter notebook projeto1.ipynb
```
(Ou abra o arquivo projeto1.ipynb diretamente na sua IDE de preferência, como o VS Code).

## Autor
Daniel Aleixo
Profissional focado em soluções através da tecnologia e Ciência da Informação.
[LinkedIn](https://www.linkedin.com/in/daniel-souza-8075371bb/)
