# Relatórios de Progresso
Este relatório tem o objetivo de demonstrar a importância da análise dos dados de um projeto de desenvolvimento de software ao longo de uma semana. Os dados fornecidos permitirão ao proprietário da equipe de desenvolvimento obter insights sobre o progresso do projeto, identificar possíveis áreas de melhoria e tomar decisões informadas para garantir o sucesso do projeto.

## O que foi feito?

### 1. Relatório de progresso diário para mostrar o quão produtivo está sendo o trabalho dos funcionários e incluindo no relatório outros itens como:
- Total de Horas Trabalhadas.
- Média Diária de Horas Trabalhadas.
- Total de Bugs Corrigidos.
- Média Diária de Bugs Corrigidos.
- Total de Tarefas Concluídas.
- Média Diária de Tarefas Concluídas.
- Produtividade Diária (Tarefas Concluídas por Hora).

### 2. Apresentação de Resultados
- Descrições do passo a passo da análise em Markdown.
- Apresentação dos dados e resultado em Matplotlib com insights gerados.
- Exemplo de um gráfico gerado:
  
```
#import da biblioteca matplotlib
from matplotlib import pyplot as plt

# Criando o gráfico de barras
ax = base_relatorio.plot(kind='bar', title='Taxa de Produtividade diária', x='Dia', y='x')

# Ocultando as bordas superior e direita do gráfico corretamente
plt.gca().spines[['top', 'right',]].set_visible(False)

# Removendo a legenda
ax.legend().set_visible(False)

# Adicionando rótulos de dados no topo das colunas
for p in ax.patches:
ax.annotate(str(p.get_height()), (p.get_x() + p.get_width() / 2., p.get_height()), ha='center', va='bottom')
# Adicionando o texto informativo diretamente ao objeto de eixo
info_text = "Média total de " + str(tarefas_hora.round(1)) + " tarefas\nconcluídas por hora"
ax.text(0.90, 0.87, info_text, horizontalalignment='left', verticalalignment='top', transform=ax.transAxes, bbox=dict(facecolor='white', alpha=0.7, boxstyle='round,pad=0.4'), fontsize=10) # Ajuste o valor de pad conforme necessário

# Exibindo o gráfico
plt.show()
```

## Execução do Projeto
1. Clone este repositório: 
>git clone https://github.com/Gabrielsoaresdm/Relatorio_progresso
2. Baixe o arquivo e relatoriosdeprogresso.py e relatorio.xlsx.
3. Utilize as consultas SQL para responder às perguntas estratégicas e adicionais.
4. Execute o Script importando o arquivo em excel.

## Considerações Finais

Este relatório enfatiza a importância da análise contínua de dados ao longo de um projeto de desenvolvimento de software. Os dados coletados ao longo de uma semana oferecem insights cruciais para os proprietários da equipe de desenvolvimento, permitindo que identifiquem áreas de melhoria e tomem decisões informadas para garantir o sucesso do projeto.

A análise de dados é essencial para entender o progresso do projeto, detectar padrões e tendências, e abordar quaisquer obstáculos rapidamente. Ao priorizar a análise de dados, os proprietários podem tomar decisões estratégicas, resultando em um produto final de alta qualidade e uma experiência satisfatória para todas as partes envolvidas.

Este relatório destaca a importância de integrar a análise de dados como parte integral do processo de desenvolvimento de software, destacando seu valor para o sucesso do projeto.


