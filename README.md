📊 **Análise de Desempenho Estudantil: Tendências e Insights**

🎯 **Objetivo do Projeto**
Este dashboard desenvolvi para analisar o histórico de 12 avaliações de uma base de estudantes, com o objetivo de identificar padrões de aprendizado, prever as quedas de desempenho e destacar alunos com evolução excepcional. O foco é fornecer uma ferramenta de decisão para gestores educacionais.

🚀 **Funcionalidades e KPIs**
Diagnóstico Dinâmico: Um cartão de status que utiliza uma lógica DAX para classificar o desempenho individual (Ex: "Desempenho Crítico", "Evolução Positiva").

Média Móvel (3 Períodos): Gráfico de linha configurado para suavizar flutuações e mostrar a tendência real de aprendizado.

Análise de Extremos (Top N): Rankings automáticos que isolam os 10 alunos com as maiores evoluções e as 10 maiores quedas.

Interatividade Total: Filtros de segmentação por ID de aluno com barra de pesquisa otimizada para grandes volumes de dados.

🛠️ **Tecnologias e Técnicas Aplicadas**
Power Query (ETL): Normalização de dados via Unpivot e criação de índices para ordenação cronológica das avaliações.

DAX Avançado: * Cálculo de % de Variação de Performance (Delta).

Medida de Média Móvel utilizando as funções CALCULATE, FILTER e ALLSELECTED.

Lógica de SWITCH(TRUE()) para a criação de status narrativos.

DataViz & UX: * Aplicação de hierarquia visual com cartões de KPI no topo.

Uso de sombras e bordas arredondadas para um layout moderno (estilo SaaS).

Configuração de Eixo Y fixo para evitar distorções visuais na interpretação das linhas de tendência.

🚧 **Dificuldades Encontradas e Aprendizados**
Ajuste de Escala Visual: Inicialmente, as quedas de desempenho pareciam exageradas devido ao ajuste automático do eixo. A solução foi fixar o intervalo do Eixo Y, trazendo uma perspectiva mais realista desses dados.

Performance com Muitos Alunos: Exibir muitos alunos em um gráfico de barras era inviável. A implementação da técnica **Top N** via painel de filtros resolveu o problema de poluição visual.

📈 **Resultados e Insights Extraídos**
A análise permitiu identificar padrões que antes estavam ocultos nos dados brutos:

Identificação de Retenção: Detectei que a média geral da turma apresentou uma queda de ~7% ao longo das 12 avaliações, sinalizando um possível aumento na complexidade do conteúdo ou fadiga dos alunos.

Mapeamento de Alunos de Elite: Através do ranking de evolução, isolamos os Top 10 alunos que, apesar da tendência de queda da turma, conseguiram manter um crescimento constante superior a 15%.

Alerta Precoce (Early Warning): A integração da Média Móvel permitiu identificar alunos que apresentaram queda de rendimento em 3 avaliações consecutivas, possibilitando uma intervenção pedagógica antes da avaliação final.

Eficiência na Gestão: O uso do dashboard reduziu o tempo de análise individual por aluno de minutos para segundos, permitindo que a coordenação foque em planos de ação.

Segmentação de Risco: O sistema de Status Dinâmico classificou automaticamente X% da base como "Desempenho Crítico", servindo como um filtro de prioridade para reuniões de pais e mestres.

📈 **Como Visualizar**
Baixe o arquivo .pbix disponível neste repositório.

Abra no Power BI Desktop.

Utilize o filtro de Alunos no canto superior esquerdo para navegar pelos dados individuais.
