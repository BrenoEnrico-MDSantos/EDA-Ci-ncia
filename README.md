[índice]: https://divvy-tripdata.s3.amazonaws.com/index.html

# Estudo de caso de clientes da Cyclistic (PT-BR)

 Realizado como projeto final do curso de Análise de Dados da Google na Coursera, este estudo tem como objetivo apresentar diferenças entre os tipos de cliente - casuais e membros - de uma **fictícia** empresa de aluguéis de biciletas que atua em Chicago, a fim de moldar um _business plan_ voltado à fidelização dos usuários casuais, uma vez que membros apresentam maior lucratividade e constância na aquisição dos serviços disponíveis. O período observado para estudo compreende 12 meses (Maio de 2024 a Abril de 2025), compreendidos em 12 tabelas `csv.`, sendo cada tabela relativa a um mês.

 Com foco no MKT de fidelização, os executivos e gestores da Cyclistic solicitam do time de análise de dados uma apresentação de _insights_ para guiar as decisões quanto aos clientes, utilizando quaisquer noções e ferramentas capazes de conduzir as etapas _Ask, Prepare, Process, Analyze, Share, Act_. 3 _business tasks_  nortearão o time de MKT e suas medidas futuras; 
 - **1. Como membros e casuais usam as _bikes_ de maneira diferente?**
  2. Por que casuais assinariam a anualidade?
  3. Como a mídia digital pode influenciar na fidelização dos casuais?

- Na proposta do estudo, apenas a pergunta de número 1 foi endereçada a mim, mas decidi analisar o período de forma mais ampla e propor medidas para cada _task_. Cada gráfico será acompanhado de uma análise descritiva (o que aconteceu) e diagnóstica (hipótese de causa); ao fim do estudo, constará a visão prescritiva (como ir adiante).

- Todo o projeto foi conduzido no RStudio, pois construí mais familiaridade com o prgrama na trajetória do curso e julguei ser o software mais veloz no processamento de milhões de linhas, bem como apto a construção de visualizações estáticas mas suficientes para complementar as hipóteses.

> ## Integridade dos dados - ROCCC

 [x] Reliable: os dados não têm viés e são próprios para uso no estudo, tendo origem em uma empresa real (Motivate International Inc.).
 [] Original: os _sets_ provêm de uma terceirizada (Divvy), então não são exatamente originais.
 [] Comprehensive: informações básicas como tipo de membro, data e hora e tipo de bike alugada estão presentes e possibilitam uma compreensão intermediária do caso, mas não são compartilhados dados financeiros (nem mesmo do plano de assinatura), e boa parte das colunas não têm relevâcia alguma na análise, tornando a massa de mais de 5 milhões de entradas desnecessariamente pesada.
 [x] Current: a cada mês são anonimizados e postados no índice [índice] os registros correspondentes.
 [x] Cited: as fontes são seguras, e com recomendação pela Google.

