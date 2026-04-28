# 🤖 Batalha de Modelos & Engenharia de Prompt (XML)

## 📝 Descrição do Projeto
Este projeto consiste na construção de um **Prompt Estruturado em XML** para geração de uma página HTML Single Page com CSS integrado, testado e comparado entre as principais ferramentas de IA do mercado.

Desenvolvido como parte da disciplina de **Engenharia de Prompt e Aplicações em IA**, o experimento submeteu o mesmo prompt estruturado a sete modelos diferentes — ChatGPT, Gemini, DeepSeek, Qwen, Grok, Maritaca e Claude — avaliando critérios como precisão do HTML gerado, criatividade no conteúdo, erros de sintaxe e quantidade de tokens consumidos. O objetivo foi identificar qual modelo demonstra maior compreensão de prompts XML e qual se mostra mais adequado para diferentes contextos de uso.

![Comparativo entre modelos](IMAGEM_1_AQUI)
*Figura 1: Quadro comparativo com os resultados de cada modelo de IA avaliado.*

## 🚀 Tecnologias Utilizadas
* **Linguagem de Prompt:** XML Estruturado
* **Saída gerada:** HTML5 + CSS3 (Single Page Application)
* **Ferramentas testadas:** ChatGPT, Gemini, DeepSeek, Qwen, Grok, Maritaca, Claude
* **Critérios de avaliação:** Precisão, criatividade, bugs e consumo de tokens

## 📊 Resultados e Aprendizados
O experimento revelou diferenças expressivas entre os modelos para o mesmo prompt de entrada.

* **Claude se destacou amplamente:** foi o único modelo a receber avaliação **Alta** em precisão, criatividade e qualidade do HTML gerado — entregando um site completo e informativo, ainda que com algumas informações inventadas.
* **Diferença de tokens é drástica:** Claude consumiu ~27.000 tokens, enquanto os demais ficaram entre 1.100 e 4.820 — mostrando que verbosidade e qualidade nem sempre caminham juntas nos outros modelos, mas no Claude a verbosidade correspondeu a um resultado superior.
* **Modelos mais simples (GPT, Qwen, Maritaca, Grok)** entregaram resultados com baixo conteúdo, falta de imagens e estrutura insatisfatória.
* **Aprendizado principal:** a estrutura XML do prompt foi interpretada de formas muito distintas por cada modelo, evidenciando a importância de escolher a ferramenta certa de acordo com a complexidade da tarefa.

![Gráfico de tokens por modelo](IMAGEM_2_AQUI)
*Figura 2: Comparação de tokens consumidos por cada modelo de IA.*

## 🔧 Como Executar
1. Copie o prompt XML abaixo.
2. Cole em qualquer ferramenta de IA de sua escolha (ChatGPT, Claude, Gemini, etc.).
3. Compare o HTML gerado com base nos critérios: precisão, criatividade, bugs e tokens.

```xml
<tarefa>
  <objetivo>Criar uma página HTML5 única com CSS3 interno (single page).</objetivo>
  <tema>[INSIRA O TEMA DA SUA PÁGINA AQUI]</tema>
  <diretrizes_design>
    <layout>Responsivo e minimalista.</layout>
    <paleta_cores>[DEFINA SUAS CORES]</paleta_cores>
    <tipografia>Sans-serif para títulos, Serif para corpo.</tipografia>
  </diretrizes_design>
  <obrigatoriedades_tecnicas>
    <item>Menu de navegação funcional (âncoras).</item>
    <item>Seção de portfólio ou galeria.</item>
    <item>Rodapé com informações de contato simuladas.</item>
    <item>[CRIAR UM ITEM]</item>
  </obrigatoriedades_tecnicas>
  <metrica_obrigatoria>
    Ao final da resposta, informe uma estimativa de quantos tokens foram gerados para este código.
  </metrica_obrigatoria>
</tarefa>
```

![Exemplo de saída HTML gerada](IMAGEM_3_AQUI)
*Figura 3: Exemplo de página HTML gerada a partir do prompt XML pelo modelo Claude.*

---
[Voltar ao início](https://github.com/gabriel-tino/portifolio-gabriel-tino)
