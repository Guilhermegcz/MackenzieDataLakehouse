# Projeto MBA Engenharia de dados
## Construção de um Data Lakehouse Transacional




## 📂 Estrutura do Projeto

```
/
├── data/
│   └── logistica_raw.csv       # Dataset bruto para ser utilizado no exercicio.
├── notebooks/
│   ├── geradorDataset.ipynb    # Notebook Jupter com o codigo para Gerar o arquivo CSV para o Exercicio.
│   ├── script.ipynb            # Notebook Jupyter com todo o código PySpark.
│   └── vendas_brutas.csv       # Dataset bruto utilizado no exemplo.
├── docker-compose.yml          # Arquivo para orquestrar o ambiente Docker.
├── Dockerfile                  # Arquivo de configuração para a imagem Docker.
├── exercicio.md                # Arquivo com o Desafio para ser feito em aula
└── readme.md                   # Este arquivo.
```

## 🛠️ Setup e Execução do Ambiente

Para executar o projeto, utilizamos um ambiente Docker que já contém o Jupyter e o PySpark configurados.

### Pré-requisitos
*   [Docker](httpss://docs.docker.com/get-docker/)
*   [Docker Compose](httpss://docs.docker.com/compose/install/)

### Passos para Execução

1.  **Clone o Repositório**:
    ```bash
    git clone 
    cd dataqualitySpark
    ```

2.  **Inicie o Ambiente Docker**:
    No terminal, a partir da raiz do projeto, execute o comando abaixo. Ele irá construir a imagem Docker (se ainda não existir) e iniciar o container do JupyterLab em background.
    ```bash
    docker compose up --build -d
    ```

3.  **Acesse o Jupyter**:
    Abra seu navegador e acesse o seguinte endereço:
    ```
    http://localhost:8888/
    ```
    *   O token de acesso já está configurado no `docker-compose.yml` para simplificar.
