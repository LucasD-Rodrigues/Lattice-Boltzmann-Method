---
name: sci-dos
description: Atualiza a documentacao cientifica do projeto Lattice-Boltzmann. Use quando teoria, equacoes, hipoteses, metodos ou resultados da simulacao forem alterados ou precisarem ser documentados.
---

# Documentacao cientifica

Mantenha `docs/report.md` como referencia para a teoria e `docs/results.md` como registro ilustrado dos resultados.

## Atualizar a teoria

1. Consulte o codigo e a documentacao existentes antes de editar.
2. Atualize `docs/report.md` quando uma mudanca afetar o modelo fisico, as equacoes, as hipoteses, as condicoes de contorno, os parametros ou o metodo numerico.
3. Identifique as equacoes de forma estavel (por exemplo, `(Eq. 1)`) e defina os simbolos, unidades e hipoteses necessarios para interpreta-las.
4. Relacione a teoria com a implementacao existente. Nao apresente uma escolha de implementacao como resultado geral da teoria.
5. Mantenha as docstrings das funcoes que implementam equacoes ligadas aos identificadores correspondentes em `docs/report.md`.

## Registrar resultados

1. Atualize `docs/results.md` quando resultados, figuras ou conclusoes de simulacao forem adicionados ou mudarem.
2. Para cada figura, informe o que esta sendo mostrado, as grandezas e unidades dos eixos, e os parametros relevantes da simulacao.
3. Use resultados e figuras realmente produzidos pelo projeto. Nao invente valores, imagens, validacoes ou conclusoes.
4. Siga as convencoes do repositorio: calculos em scripts `.py`, dados salvos em `.npz` e plots em notebooks `.ipynb`.

## Revisao

- Altere apenas a documentacao afetada pela tarefa; nao atualize resultados sem evidencias.
- Confira que equacoes, simbolos, unidades, parametros e conclusoes estejam consistentes entre `report.md`, `results.md` e o codigo.
- Se faltarem dados para documentar algo com seguranca, indique o que falta em vez de preencher por suposicao.