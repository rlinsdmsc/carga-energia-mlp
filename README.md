# 📊 Previsão de Carga Energética Mensal com Redes Neurais (MLP)

Este projeto tem como objetivo prever a **carga mensal de energia elétrica (MW médios)** do Sistema Interligado Nacional (SIN) brasileiro utilizando uma **rede neural artificial (MLP)** simples implementada com Keras.

## ⚙️ Tecnologias Utilizadas
- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib

## 🗂️ Estrutura do Projeto

carga-energia-mlp/
├── data/
│ └── CARGA_MENSAL.csv # Base de dados do ONS
├── notebooks/
│ └── previsao_carga.ipynb # Código em Jupyter Notebook
├── README.md
├── requirements.txt
└── .gitignore

## 📁 Fonte dos Dados

Dados públicos obtidos do Operador Nacional do Sistema Elétrico (ONS):  
🔗 https://www.ons.org.br/paginas/energia-agora/dados-gerais

Formato:
- `id_subsistema`: N, NE, S, SE
- `nom_subsistema`: NORTE, NORDESTE, SUL, SUDESTE/CENTRO-OESTE
- `din_instante`: data da medição (DD/MM/AAAA)
- `val_cargaenergiamwmed`: valor médio mensal da carga (MW médios)

## 📈 Objetivo

Prever o valor da carga energética mensal futura com base no **ano e mês**, utilizando um modelo de Rede Neural Multilayer Perceptron (MLP). A previsão pode ser feita para qualquer subsistema (ex: SE - Sudeste/Centro-Oeste).

## ▶️ Como Executar

1. Clone o repositório:

   git clone https://github.com/seu-usuario/carga-energia-mlp.git
   cd carga-energia-mlp

2. Crie e ative um ambiente virtual:

    Editar
    python -m venv venv
    .\venv\Scripts\activate   # Para Windows

3. Instale as dependências:

    pip install -r requirements.txt

4. Execute o notebook previsao_carga.ipynb na pasta /notebooks.

📊 Resultado Esperado

    Gráfico comparativo entre a carga real e a previsão feita pela rede neural, além da previsão de carga para o próximo mês, com base no histórico de dados.

    Exemplo de saída: Previsão de carga para agosto/2025: 70245.32 MW médios

🧠 Melhorias Futuras

    Incluir variáveis climáticas externas (ex: temperatura, pluviometria)

    Incluir crescimento populacional

    Usar LSTM para prever sequências

    Treinar modelos por região e comparar desempenho

Desenvolvido por
Ruan Damasceno
Eng. Eletricista