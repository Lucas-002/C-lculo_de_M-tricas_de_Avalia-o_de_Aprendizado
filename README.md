# Métricas de Classificação

Este projeto implementa funções para calcular as principais métricas de avaliação de modelos de classificação com base em uma matriz de confusão.

## Métricas Implementadas
- **Sensibilidade (Recall)**: VP / (VP + FN)
- **Especificidade**: VN / (FP + VN)
- **Acurácia**: (VP + VN) / N
- **Precisão**: VP / (VP + FP)
- **F-score**: 2 * (Precisão * Sensibilidade) / (Precisão + Sensibilidade)

## Como Usar
1. Defina os valores da matriz de confusão:
   - VP: Verdadeiros Positivos
   - VN: Verdadeiros Negativos
   - FP: Falsos Positivos
   - FN: Falsos Negativos

2. Use a função `calcular_metricas(vp, vn, fp, fn)` para obter as métricas.

3. Execute o script para visualizar os resultados calculados.

## Exemplo
```python
vp = 50
vn = 40
fp = 10
fn = 5

metricas = calcular_metricas(vp, vn, fp, fn)

for metrica, valor in metricas.items():
    print(f"{metrica}: {valor:.2f}")
```

## Requisitos
- Python 3.6 ou superior
- Bibliotecas: `numpy`, `pandas`

## Autor
Desenvolvido por Lucas Márcio Chaves Gomes
