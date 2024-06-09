# Análise de Turnover - People Analytics

Neste estudo, realizaremos uma análise usando estatística descritiva para compreender quais fatores explicam a incidência de turnover na empresa alvo deste estudo e, consequentemente, a propisção de ações que visam mitigar a frequência de turnover.

## Introdução

No contexto de Recursos Humanos, o  _turnover_  (ou rotatividade de pessoal) é o nome dado ao fluxo de entrada e saída de colaboradores em uma empresa. Esse índice é calculado a partir da relação entre o desligamento e a admissão de novas pessoas colaboradoras em um período de tempo (geralmente anual). Essa rotatividade engloba tanto os desligamentos voluntários como involuntários. O indicador de _turnover_  tem grande relevância para o sucesso do setor de RH, portanto, deve ser acompanhado de perto.

Para o cálculo efetivo do  _turnover_, usa-se a fórmula Total= (número de colaboradores contratados + número de colaboradores desligados de um mês) / 2;  _Turnover_  = [Total / (número total de colaboradores do mês anterior)] x 100. No geral, uma taxa de  _turnover_  de até 10% ao ano é considerada boa e possibilita que haja renovação na equipe.

## Objetivo

O objetivo deste projeto foi calcular a taxa de _turnover_, observando sua relação com as variáveis qualitativas e quantitativas presentes no banco de dados.

## Compreendendo a base de dados

Para esta análise, vamos utilizar a base de dados chamada "base_turnover.csv", O arquivo contem 1471 linhas e 21 colunas, sendo a primeira o identificador único de cada colaborador (ID) e as demais, variáveis qualitativas e quantitativas, sendo as seguintes variáveis.

- ID;
- Funcionário_deixou_a_empresa;
- Idade;
- Frequência_de_Viagens;
- Distância_do_trabalho	Formação;
- ESat;
- Gênero;
- Estado_Civil;
- Salário;
- Qte_Empresas_Trabalhadas;
- Faz_hora_extras?;
- Perc_de_aumento;
- Qte_ações_da_empresa;
- Tempo_de_carreira;
- Horas_de_treinamento;
- Equilibrio_de_Vida;
- Tempo_de_empresa;
- Anos_no_mesmo_cargo;
- Anos_desde_a_ultima_promocao;
- Anos_com_o_mesmo_chefe.

## Execução do projeto

Para a execução desta análise, foi utilizado um Jupyter Notebook. Logo, recomenda-se que as seguintes bibliotecas Python estejam previaente instaladas para que a exeução do projeto ocorra conforme esperado. As bibliotecas são as seguintes:
- Pandas;
- NumPy;
- Pyplot;
- Seaborn;
- Scorecardpy.

O detalhamento da ordem de execução do projeto, assim como os resultados obtidos em cada etapa, pode ser encontrado no Jupyter Notebook 'analise_turnover.ipynb'.

## Conclusão e Sugestões para Análises Futuras

A partir das análises realizadas pudemos ver que os fatores que mais influenciam o  _turnover_  da empresa são a idade, o tempo de carreira e empresa, além de fazer horas extra. Foi possível chegar a esta conclusão utilizando, além da análise descritiva, o _Information Value (IV)_. O IV tem como objetivo analisar a explicabilidade de cada variável para que o nosso _target_ (variável de interesse) tenha o comportamento alvo do estudo. Neste caso, ter _turnover_.  

Avaliando-se a idade e o tempo de carreira, percebe-se que os mais jovens (e com menos tempo de carreira) estão mais propensos a saírem da empresa, Ao incluirmos o tempo de empresa neste contexto, há uma série de ações que podem ser feitas para aumentar o índice de retenção destes talentos. Das quais, podemos destacar:

- Ciclos de feedbacks mais curtos para acompanhar o nível de satisfação destes colaboradores e ações de retenção possam ser mais intencionais e preventivas;

- Construção de PDIs individuais que sejam acompanhados com regularidade;

- Estruturação de plano de carreira sólido e claro para todos os colaboradores;

- Utilização de programas de incentivo a capacitação e também por tempo de empresa.

No mesmo sentido, as políticas de horas extra deverão ser revistas, evitando que elas aconteçam, ou sendo compensadas ou remuneradas de forma adequada. É importante considerar que possa estar havendo um excesso de volume de trabalho ou uma má distribuição do mesmo.

Para estudos futuros, propõe-se a realização de análises de correlação para a identificação de quais são os critérios com maior possibilidade de mitigação e que esses sejam priorizadas nas iniciativas de recursos humanos. Além disso, a definição e validação de modelos de _Machine Learning_ que pontuem os colaboradores com maior risco e que ações direcionadas possam ser tomadas pelo RSH e lideranças.
