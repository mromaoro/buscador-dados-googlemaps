# Buscador de Dados da Chapada dos Veadeiros

Um script em Python que utiliza a **API do Google Maps** para extrair informações de pontos de interesse (como restaurantes, pousadas e comércios) nas cidades de **Alto Paraíso de Goiás, Cavalcante e Vila São Jorge**. O resultado é consolidado em um arquivo `.csv` para análise posterior.

---

## 🚀 Funcionalidades

* **Coleta Abrangente**: Realiza múltiplas buscas por diferentes termos (`pousadas`, `restaurantes`, `agências de turismo`, etc.) para coletar uma variedade de dados.
* **Consolidação de Dados**: Combina os resultados de todas as buscas, removendo duplicatas para garantir um conjunto de dados limpo e único.
* **Geolocalização**: Categoriza cada ponto de interesse em uma das regiões predefinidas (Vila São Jorge, Alto Paraíso de Goiás, Cavalcante).
* **Geração de CSV**: Salva todos os dados coletados em um arquivo CSV (`comércios_alto_paraíso.csv`), facilitando a importação para planilhas ou outras ferramentas de análise.

---

## 🛠️ Tecnologias e Dependências

* **Python 3.x**
* **Google Maps API**: A principal fonte de dados para o projeto.
* **`googlemaps`**: Biblioteca Python para interagir com a API do Google Maps.
* **`pandas`**: Utilizada para manipular e organizar os dados em um `DataFrame` e exportá-los para CSV.

---

## ⚙️ Como Usar

### Pré-requisitos

Para rodar este script, você precisa de:

* Uma **chave de API do Google Maps** com as permissões **Places API** ativadas.
* Um ambiente de notebook como **Google Colab** para executar o código.

### Configuração

1.  **Obtenha sua Chave de API**: Se ainda não tiver uma, crie um projeto no **Google Cloud Console** e gere uma chave de API, ativando a **Places API**.
2.  **Configure o Google Colab**:
    * No Google Colab, vá em **Segredos** (o ícone de chave no menu lateral).
    * Clique em **Adicionar segredo** e crie uma nova variável com o nome `Maps_API_KEY`.
    * Cole sua chave de API no campo de valor.

### Executando o Script

1.  Abra o script em um ambiente como o Google Colab.
2.  Execute todas as células na ordem.
3.  O script irá instalar as bibliotecas necessárias, carregar sua chave de API e iniciar a coleta de dados.
4.  Ao final da execução, um arquivo chamado `comércios_alto_paraíso.csv` será gerado. Você pode baixá-lo diretamente do menu de arquivos do Colab.