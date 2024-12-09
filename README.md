
<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="40px" src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png"></a>
    <span>Previsão com Pontos de Extremidade no Azure ML</span>
</h1>

## Sobre o Projeto
Página desenvolvida para fins didáticos para o curso *Microsoft - AZURE AI-900** da [Digital Innovation One](https://www.dio.me/). O projeto é um estudo sobre a criação de AI na plataforma Azure Microsoft. Adicionei legendas em uma imagem de hambúrguer que foi trago os seguintes resultados:



## Passo a Passo

### 1. Configuração do Ambiente
- **Conta Azure**: Certifique-se de ter uma conta Azure ativa.
- **Azure ML Studio**: Acesse o [Azure ML Studio](https://ml.azure.com/).
- **Workspace**: Crie ou selecione um workspace existente.

### 2. Criar um Dataset
- **Acesse Datasets**: No menu lateral, clique em "Datasets".
- **Criar Dataset**: Clique em "Create Dataset" e escolha "From local files".
- **Upload de Arquivo**: Faça o upload do seu arquivo de dados (por exemplo, CSV).
- **Configuração**: Dê um nome ao dataset e configure as colunas.

### 3. Criar um Pipeline de Treinamento
- **Acesse Pipelines**: No menu lateral, clique em "Pipelines".
- **Criar Pipeline**: Clique em "Create Pipeline".
- **Adicionar Módulos**:
  - Arraste e solte os módulos necessários.
  - Conecte o dataset ao módulo "Split Data".
  - Adicione o módulo "Train Model" e configure-o.
  - Adicione o módulo "Score Model" e "Evaluate Model".
- **Executar Pipeline**: Clique em "Submit" e aguarde a conclusão.

### 4. Registrar o Modelo
- **Acesse Models**: No menu lateral, clique em "Models".
- **Registrar Modelo**: Clique em "Register Model".
- **Selecionar Modelo**: Escolha o modelo treinado.
- **Configuração**: Dê um nome ao modelo e clique em "Register".

### 5. Criar um Ponto de Extremidade
- **Acesse Endpoints**: No menu lateral, clique em "Endpoints".
- **Criar Endpoint**: Clique em "Create Endpoint".
- **Configuração**: Escolha "Real-time endpoint", dê um nome e selecione o modelo.
- **Criar**: Clique em "Create".
- **Testar**: Após a criação, use a opção "Test" para verificar a previsão.

## Saídas JSON

### Exemplo de Saída do Ponto de Extremidade

```json
{
  "input": {
    "data": [
      {
        "feature1": 1.23,
        "feature2": 4.56,
        "feature3": 7.89
      }
    ]
  },
  "output": {
    "prediction": 0.987
  }
}

## Tecnologias
![HTML](https://img.shields.io/badge/HTML-000?style=for-the-badge&logo=html5&logoColor=30A3DC)
