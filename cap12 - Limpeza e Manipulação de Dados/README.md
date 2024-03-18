# Correção de Dados no PowerBI

## Problemas Identificados

- 🔄 **Duplicatas na Coluna `ID_Cliente`:** Encontramos linhas duplicadas, o que é um erro, pois cada cliente deve ter um ID único.
- ❌ **Valores Ausentes em `Idade` e `Peso`:** Antes de qualquer análise, precisamos tratar esses campos vazios.
- 📊 **Outliers na Altura:** Observamos valores extremos na coluna de altura, que precisam ser tratados.

## Soluções Propostas

- ✨ **Removendo Duplicatas:** Utilize a função "Remover Duplicatas" no PowerBI para limpar a coluna `ID_Cliente` com facilidade.
- 📝 **Tratamento de Valores Ausentes:** Substitua os valores ausentes pela mediana da idade (40 anos) e do peso (70 kg) para manter a integridade dos dados.
- 📏 **Correção de Outliers:** Substitua os outliers na idade pela mediana da altura (172 cm) para garantir a consistência dos dados.

## Demonstração Visual

[Inserir imagens ou gráficos aqui]

## Como Usar

1. Clone este repositório.
2. Abra o arquivo `data_analysis.pbix` no PowerBI.
3. Siga as instruções fornecidas para corrigir os problemas identificados.
4. Salve as alterações e compartilhe os insights obtidos!

## Contribuição

Contribuições são bem-vindas! Se você tiver sugestões de melhorias ou novas ideias, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
