# Projeto Automação de Processo

### Objetivo
Construir um projeto que automatize os processos realizados diariamente pela equipe de análise de dados de uma rede com 25 lojas, em um cenário hipotético.

### Créditos e inspirações
Este projeto foi desenvolvido no curso "Python Impressionador" coordenado e ministardo por João Paulo Lira da empresa Hashtag.

### Tecnologia utilizada
Python

### Sobre o projeto
Processos realizados diariamente pela equipe de análise de dados:
- calcular os One Pages de cada loja.
- enviar um email para os gerentes de cada loja com os respectivos One Pages no corpo do email e em anexo o arquivo com os dados utilizados para calculá-los.
- enviar um email para a diretoria, informando no corpo do email a melhor e a pior loja do dia e também a melhor e pior loja do ano. Além disso, anexar dois arquivos: um com o ranking do dia e o outro ranking do ano.
- no diretório "Backup Arquivos Lojas", salvar o arquivo com os dados da loja em sua respectiva pasta.

O One Page, é um resumo com os principais indicadores de cada loja e permite em uma página comparar quais indicadores aquela loja conseguiu cumprir naquele dia/ano ou não. O One Page apresentará os seguintes indicadores com as repectivas metas:

- Faturamento -> Meta Ano: 1.650.000 / Meta Dia: 1000
- Diversidade de Produtos (quantos produtos diferentes foram vendidos naquele período) -> Meta Ano: 120 / Meta Dia: 4
- Ticket Médio por Venda -> Meta Ano: 500 / Meta Dia: 500

Exemplo de OnePage:

![onepage_2](https://github.com/FernandaDamaceno/Imagens/blob/f222ea5f86d5a123f712e27a424dd9d9aa771277/Automacao_Processos/onepage_2.png)

Exemplo de email enviado para um gerente de uma loja:

![emailgerente](https://github.com/FernandaDamaceno/Imagens/blob/f222ea5f86d5a123f712e27a424dd9d9aa771277/Automacao_Processos/emailgerente.png)

Exemplo de email enviado para diretoria:

![emaildiretoria](https://github.com/FernandaDamaceno/Imagens/blob/f222ea5f86d5a123f712e27a424dd9d9aa771277/Automacao_Processos/emaildiretoria.png)

Sobre o diretório "Backup Arquivos Lojas", inicialmente deverá estar vazio e, após rodar o código, serão criadas as pastas das lojas com os respectivos arquivos.

Exemplo do diretório "Backup Arquivos Lojas":

![diretorio_backup](https://github.com/FernandaDamaceno/Imagens/blob/45fb0a5e70271d0266ba7515d5755d4725f2906d/Automacao_Processos/diretorio_backup.png)



Sobre as bases de dados, serão utilizadas três: "Emails", "Lojas" e "Vendas". As bases estão no diretório Bases_Dados

A base "Emails"  apresenta os seguintes campos:
- loja: nome da loja.
- gerente: nome dos gerentes.
- email: e-mail do gerente. Para fins de teste do código, o e-mail do gerente pode ser o seu email + o nome do gerente, sendo necessário que seu e-mail esteja vinvculado ao Outlook. Exemplo: emailqualquer+helena@gmail.com.

A base "Lojas"  apresenta os seguintes campos:
- ID Loja: número de identificação da loja.
- nome da loja.

A base "Vendas"  apresenta os seguintes campos:
- Código Venda: número de identificação da venda.
- Data: data na qual a venda foi realizada.
- ID Loja: número de identificação da loja.
- Produto: nome do produto.
- Quantidade: quantidade vendida do produto.
- Valor Unitário: valor unitário do produto.
- Valor Final: valor final do produto (Quantidade x Valor Unitário).
