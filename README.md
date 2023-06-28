# DesafioSQLSpecialist2
Projeto do zero referente ao Desafio do Diagrama EER do Bootcamp SQL Specialist

Contexto da Metodologia:
-
. Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
. Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas
. Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
. A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
. O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços
. A mesma equipe avalia e executa os serviços
. Os mecânicos possuem código, nome, endereço e especialidade
. Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.

Contexto da MINHA Metodologia:
- 
Entidade Fortes e criadas a partir de análise: Clientes, Ordem de Serviço, Veículo, Funcionário, Especialidade, Peça, Estoque e Fornecedor;

Entidades Fracas: Disponibilidade de Veiculos por Cliente(gerada na relação de Cliente e Veiculo), Peças por OS(gerada pela relação de valor entre Peça(custo da loja) incrementada a OS), Peças por Fornecedor(gerada pela relação de valor entre Peça(custo da loja) incrementeada ao Valor Unitário do Fornecedor.

Relacionamentos:

1 - Veiculos são consertados ou passam por revisão, sendo que um cliente pode ter vários veiculos contendo uma ordem de serviço para cada um deste.
2 = Ordem de Serviços são executadas por uma equipe de funcionários que podem ter diferentes especialidades e que influeciam o preço final da OS então optei por tabelar a especialidade com a mão de obra que pode ser desempenhada pelo mesmo funcionário.
3 - Diferente peças de diferentes fornecedores podem ser usadas nas OS e exigem o seu cálculo final.

