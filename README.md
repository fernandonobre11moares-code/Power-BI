🔎 Projeto de estudo: análise de vendas de e-commerce no Power BI

Montei esse dashboard como projeto de treinamento, simulando dados de pedidos e itens de um e-commerce fictício. Mas o que mais aprendi não foi sobre gráficos — foi sobre os problemas que aparecem numa base de dados real antes dela virar um dashboard bonito.

Alguns dos desafios que encontrei e resolvi:

📌 Duas linhas de pedidos diferentes compartilhando o mesmo ID (uma colisão de identificador, não uma duplicata simples) — precisei atribuir um novo ID único e atualizar as referências na tabela de itens, na ordem certa, para não quebrar o relacionamento.

📌 Um produto cadastrado duas vezes com IDs diferentes, ambos já com vendas registradas — precisei unificar as referências antes de poder excluir o duplicado com segurança.

📌 Uma taxa de devolução de -13,91% identificada através de três medidas DAX complementares (Total Bruto, Valor Devolvido e Total Líquido), que juntas contam uma história mais completa do que qualquer número isolado.

O dashboard final traz Total Bruto, Total Líquido, % de Devolução, evolução de vendas no tempo, vendas por categoria e uma tabela de status para investigação contínua.

Dados fictícios, gerados para fins de estudo — mas os problemas de qualidade de dados que resolvi são exatamente do tipo que aparece em bases reais.
