# AntifraudeDocs Challenge

Este projeto é uma aplicação web desenvolvida com Streamlit que permite o upload de documentos (imagens e PDFs) para o Azure Blob Storage e realiza a análise de cartões de crédito utilizando a API de Document Intelligence da Azure.

## Funcionalidades

- Upload de arquivos (PNG, JPG, JPEG, PDF).
- Armazenamento dos arquivos enviados no Azure Blob Storage.
- Análise de informações de cartões de crédito, incluindo:
  - Nome do titular do cartão
  - Número do cartão
  - Data de validade
  - Banco emissor

## Tecnologias Utilizadas

- [Streamlit](https://streamlit.io/)
- [Azure Storage Blob](https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blobs-overview)
- [Azure Document Intelligence](https://learn.microsoft.com/en-us/azure/cognitive-services/document-intelligence/)
- [Python](https://www.python.org/)

## Pré-requisitos

Antes de executar o projeto, você precisa ter o Python instalado em sua máquina. Além disso, você deve ter uma conta no Azure e configurar os seguintes serviços:

1. Azure Blob Storage
2. Azure Document Intelligence

## Configuração do Ambiente

1. Clone este repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd antifraudedocs_challenge

2. Crie um ambiente virtual e ative-o:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Para Linux/Mac
    venv\Scripts\activate  # Para Windows

3. Instale as dependências:\
    ```bash
    pip install -r requirements.txt

4. Crie um arquivo .env na raiz do projeto e adicione suas credenciais do Azure:
    ```bash
    ENDPOINT=<SEU_ENDPOINT>
    SUBSCRIPTION_KEY=<SUA_CHAVE_DE_ASSINATURA>
    AZURE_STORAGE_CONNECTION_STRING=<SUA_CONNECTION_STRING>
    CONTAINER_NAME=<NOME_DO_SEU_CONTAINER>

## Execução do Projeto
 
Para iniciar a aplicação, execute o seguinte comando:
    ```bash
    streamlit run app.py

A aplicação estará disponível em http://localhost:8501.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## Licença
Este projeto está licenciado sob a MIT License. Veja o arquivo LICENSE para mais detalhes.