# 🔓 Estratégia de Saída e Mitigação de Vendor Lock-in — Bubble

## 📝 Descrição do Projeto
Este projeto documenta a **estratégia de mitigação de Vendor Lock-in** para aplicações desenvolvidas na plataforma Bubble (no-code). O objetivo principal é garantir a soberania sobre os dados e viabilizar uma futura migração para tecnologias tradicionais, eliminando a dependência exclusiva de uma plataforma fechada para a continuidade do software.

Desenvolvido como projeto pessoal/profissional, o trabalho analisa o risco inerente ao uso do Bubble — uma plataforma *closed-source* que retém o código-fonte gerado e a infraestrutura de execução — e propõe um plano de extração programática via API, com scripts em Python para persistência dos dados em banco relacional independente e reaproveitamento da lógica documentada para uma futura reescrita em **React + Node.js**.

![Diagrama de estratégia de migração]


## 🚀 Tecnologias Utilizadas
* **Plataforma de origem:** Bubble (no-code)
* **Linguagem de extração:** Python (`requests`)
* **Banco de destino:** PostgreSQL
* **Stack alvo (pós-migração):** React (frontend) + Node.js (backend)
* **Formato de transporte:** JSON (via Data API do Bubble)

## 📊 Resultados e Aprendizados
O projeto entrega um plano estruturado e replicável para qualquer aplicação Bubble que precise garantir independência de plataforma.

* **Análise de risco documentada:** O Bubble não permite exportar código-fonte, criando dependência total de sua infraestrutura e política de preços — risco mapeado e endereçado com plano concreto.
* **Extração via Data API:** Habilitando a API nas configurações do Bubble (`Settings > API`), é possível acessar endpoints REST para tabelas críticas como Usuários, Clientes e Orçamentos via requisições GET.
* **Pipeline de migração:** Script Python realiza requisições nos endpoints (`/api/1.1/obj/orcamento`), parseia o JSON retornado e insere os dados em PostgreSQL de forma independente.
* **Reaproveitamento de lógica:** Os Workflows e Privacy Rules documentados no Bubble funcionam como "Manual de Requisitos" e "Dicionário de Dados" para a equipe de desenvolvimento da versão em código puro.



## 🔧 Como Executar
1. No Bubble, habilite a Data API em `Settings > API` para as tabelas desejadas.
2. Clone o repositório e instale as dependências:
```bash
pip install -r requirements.txt
```
3. Configure as variáveis de ambiente com a URL e token da sua aplicação Bubble.
4. Execute o script de extração:
```bash
python extract.py
```
5. Os dados serão extraídos em JSON e persistidos automaticamente no PostgreSQL configurado.

![Exemplo de extração JSON para PostgreSQL](IMAGEM_3_AQUI)
*Figura 3: Exemplo de dados extraídos via API do Bubble e inseridos no banco relacional.*

---
