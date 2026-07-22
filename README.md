# Predição da Qualidade do Vinho Tinto

## Objetivo
Prever a qualidade de vinhos tintos com base em suas propriedades físico-químicas,
utilizando técnicas de classificação supervisionada.

## Integrantes
- Guilherme Victório de C. B. Vieira
- Gustavo Tínel V. Fraga
- Laísla O. D. de Souza

## Fonte dos dados
[UCI Machine Learning Repository — Wine Quality](https://archive.ics.uci.edu/dataset/186/wine+quality)  
Arquivo utilizado: `winequality-red.csv` (vinho tinto)

## Tipo da tarefa
Classificação — o atributo-alvo (`quality`) foi agrupado em três faixas:
- **Ruim**: notas ≤ 4
- **Médio**: notas 5 e 6
- **Bom**: notas ≥ 7

## Modelos utilizados
- Baseline: `DummyClassifier` (most_frequent)
- `SGDClassifier`
- `RandomForestClassifier` ← modelo final escolhido

## Principais resultados
| Métrica | Valor |
|---|---|
| Acurácia | 0.838 |
| Precisão (macro) | 0.492 |
| Revocação (macro) | 0.442 |
| F1-score (macro) | 0.454 |

O modelo acerta bem a classe majoritária (Médio: F1 = 0.91), mas tem dificuldade
com as classes minoritárias, especialmente "Ruim", que não foi prevista corretamente
em nenhuma amostra do teste.

## Organização dos arquivos
├── QualidadeVinho.ipynb # Notebook principal

├── README.md

## Como executar
1. Abra o `QualidadeVinho.ipynb` no [Google Colab](https://colab.research.google.com/)
2. Execute todas as células em ordem (Runtime → Run all)
3. Os dados são carregados diretamente da URL da UCI, sem necessidade de upload

## Uso de ferramentas de IA
- **Ferramenta:** Claude (Anthropic)
- **Finalidade:** apoio na estruturação do notebook e revisão das explicações em markdown
- **Partes utilizadas:** seções 5.2, 5.6 e 5.7
- **Verificação:** cada célula gerada foi executada e conferida pelos integrantes.
  Os resultados numéricos (distribuições, métricas, matriz de confusão) foram
  comparados com o esperado com base na teoria vista em aula. As explicações em
  markdown foram revisadas e reescritas onde necessário para refletir a
  interpretação do grupo, não apenas o output da ferramenta.

## Divisão das contribuições
- **Guilherme:** seções 5.2 e 5.3
- **Gustavo:** seções 5.6 e 2.7
- **Laísla:** seções 5.1, 5.4 e 5.5

## Vídeo
🔗 *(inserir link do vídeo aqui)*
