# 🛒 Scraping de Dados — Preços de Tênis na Amazon

## 📝 Descrição do Projeto
Este projeto consiste em um coletor automatizado de dados que extrai informações de preços de tênis diretamente das páginas da Amazon. O objetivo principal é monitorar variações de preço em tempo real, identificando o **valor mais caro**, o **valor mais barato** e os produtos em **promoção**.

Desenvolvido como projeto pessoal/profissional, o sistema realiza o scraping das listagens da Amazon, processa os dados coletados e os armazena em arquivos `.csv` para análise posterior, exibindo os resultados por meio de dashboards visuais gerados com Matplotlib.

![Dashboard principal](IMAGEM_1_AQUI)
*Figura 1: Dashboard principal exibindo a variação de preços dos tênis coletados.*

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Bibliotecas:** Pandas, Matplotlib, Requests, BeautifulSoup
* **Armazenamento:** CSV
* **Fonte de dados:** Amazon Brasil

## 📊 Resultados e Aprendizados
O projeto entrega uma visão clara e automatizada do mercado de tênis na Amazon, facilitando a tomada de decisão de compra.
* **Monitoramento de preços:** O sistema identifica automaticamente o produto mais barato, o mais caro e os itens em promoção a cada execução.
* **Tratamento de dados:** Aprendi a limpar e normalizar dados extraídos da web (remoção de caracteres especiais, conversão de moeda, tratamento de valores nulos).
* **Visualização:** Implementei dashboards com Matplotlib que exibem a distribuição de preços e destacam as melhores ofertas.

![Gráfico de Preços e Promoções](IMAGEM_2_AQUI)
*Figura 2: Análise visual da distribuição de preços e produtos em promoção.*

## 🔧 Como Executar
1. Clone o repositório.
2. Instale as dependências: `pip install -r requirements.txt`
3. Execute o scraper: `python main.py`
4. Os dados coletados serão salvos em `dados.csv` e os dashboards gerados automaticamente.

![Fluxo de Coleta e Visualização](IMAGEM_3_AQUI)
*Figura 3: Pipeline do projeto — da coleta na Amazon até a geração dos dashboards.*

---

https://github.com/gabriel-tino/projetoscraping
