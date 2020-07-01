# ProjetoRedeCnpj
Projeto que permite a visualização da rede de ligações entre uma empresa e seus sócios

# Objetivo
Criar um meio visual de identificar uma empresa (CNPJ) e suas ligações com pessoas físicas (CPFs) ou outras empresas.

# Base
Uso de dados abertos da Receita Federal contendo toda a base de empresas e sócios do Brasil.
Todo o serviço tem como base a utilização dados públicos e de acesso irrestrito liberados periodicamente pela Receita Federal, dentro do conceito de DADOS ABERTOS.
http://www.receita.economia.gov.br/orientacao/tributaria/cadastros/cadastro-nacional-de-pessoas-juridicas-cnpj/dados-publicos-cnpj

# Crédito de tecnologia
Uso do projeto https://github.com/fabioserpa/CNPJ-full como base.

# Linguagem
Com exceção do site, que é informativo e criado em WordPress, todo o ambiente de preparação dos dados como o de busca e visualização é realizado em Python, com diversas bibliotecas de apoio.

# Banco de Dados
Inicialmente o projeto se iniciou com o uso do SQLite, para facilitar o desenvolvimento, primeiros testes e liberação de uso em beta-testa.
Após a confirmação do funcionamento, o projeto foi alterado para usar o MySQL.

# Detalhes de funcionamento e explicativo
O site Rede CNPJ (https://redecnpj.com.br/) foi criado com o objetivo de explicar os conceitos, bases, privacidade e uso dos recursos.
A cada liberação de arquivos pela Receita Federal (a cada 3 meses), é executado o download do conjunto de arquivos para ambiente local.
Com base nos arquivos, é executado um processamento de organização dos dados e geração do banco de dados MySQL.
Uma vez que o banco de dados esteja atualizado, é feita a disponibilização do banco no ambiente do provedor de forma que ele seja utilizado para as consultas realizadas.

# Visual final
O relatório final que é obtido com base em grafo dinâmico com ligações entre empresas e sócios.
