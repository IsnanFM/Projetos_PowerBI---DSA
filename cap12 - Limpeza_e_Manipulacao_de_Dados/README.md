# Correção de Dados no PowerBI

## Identificamos alguns problemas na base de dados importada:

- 🔄 **Duplicatas na coluna `ID_Cliente`:** Cada cliente deveria ter um ID único, mas encontramos linhas duplicadas.
- ❌ **Valores ausentes em `idade` e `peso`:** Antes de qualquer análise, precisamos lidar com esses campos vazios.
- 📊 **Outliers na altura:** Observamos valores extremos na coluna de altura, que precisam ser tratados.
## Visão geral:
![vg](./Visão_Geral_Tabela.png)
## Corrigindo problemas:

- ✨ **Removendo Duplicatas:** Facilmente podemos corrigir o primeiro problema pois o PowerBI já nos oferece uma opção para isso. Clicando com o botão direito na coluna `ID_Cliente`, conseguimos notar uma função "Remover Duplicadas", e com um click todos os ID's duplicados são excluídos.
- 📝 **Tratamento de Valores Ausentes:** Nesse ponto, não queremos excluir linhas caso haja "null"(valores ausentes) nos campos. Portanto, temos duas opções, ou substituimos pela média ou pela mediana. Porém, para fazermos isso para a média, precisariamos fazer um teste estatístico pra verificar a distribuição dos dados. Entretanto, só usaremos PowerBI nesse caso, que não permite tal teste, então vamos substituir pela mediana da `idade` e `peso`, que no caso vale `40 anos` e `70 kg`, respectivamente, verificado no próprio PowerBI.
- 📏 **Correção de Outliers:** No gráfico de dispersão abaixo, notamos que a coluna de idade há 2 outliers, muito esstranhos por sinal. Duas alturas acima de 260 cm, uma de `277 cm` e outra de `278 cm`, em pesquisas não há registros de pessoas que mediram essa altura. Portanto, teremos que corrigir esse erro, que pode ter sido causado por diversos fatores, incluindo erro de digitação. Para corrigir isso vamos adotar a mesma solução da questão anterior, vamos substituir pela mediana que é de `172 cm`.

## Demonstração Visual

| ![Outliers](./Gráfico_dispersão.png) | ![Apos_correcao](./Altura_correção.png) |
|:---:|:---:|
| *Outliers* | *Após correção* |
## Visão geral após alterações:
![vg](./Apos_alteracao.png)

## Contribuição

Contribuições são bem-vindas! Se você tiver sugestões de melhorias ou novas ideias, sinta-se à vontade para abrir uma issue ou enviar um pull request.

