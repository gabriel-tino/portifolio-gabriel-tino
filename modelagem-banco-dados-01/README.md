💊 Sistema de Gestão de Farmácia — Banco de Dados PostgreSQL
📝 Descrição do Projeto
Este projeto consiste em um script DDL completo em PostgreSQL para um sistema de gestão de farmácia. O objetivo principal é estruturar e otimizar o banco de dados relacional que sustenta as operações do estabelecimento, cobrindo desde o cadastro de clientes e produtos até o controle de estoque, pedidos e validações farmacêuticas.
Desenvolvido como projeto pessoal/profissional, o banco de dados modela entidades reais do ambiente farmacêutico — como colaboradores com CRF obrigatório para farmacêuticos, controle de receitas, localização física de produtos no estoque e validações por lote —, aplicando boas práticas de modelagem relacional com constraints, índices, triggers automáticos e views analíticas.
Mostrar Imagem
Figura 1: Diagrama entidade-relacionamento do sistema de gestão de farmácia.
🚀 Tecnologias Utilizadas

Linguagem: SQL (DDL)
Banco de Dados: PostgreSQL
Recursos utilizados: Constraints, Indexes, Triggers, Functions (PL/pgSQL), Views
Tabelas principais: cliente, produto, colaborador, pedido, item_pedido, localizacao_estoque, validacao_produto

📊 Resultados e Aprendizados
O projeto entrega uma base de dados robusta, validada e pronta para uso em ambiente de produção.

7 tabelas modeladas com integridade referencial completa via chaves estrangeiras e constraints de domínio (validação de CPF, e-mail, telefone, preços, categorias e cargos).
Triggers automáticos: O valor total do pedido é recalculado automaticamente a cada inserção, atualização ou exclusão de itens, eliminando inconsistências manuais.
5 Views analíticas prontas para uso: produtos com estoque baixo, produtos próximos ao vencimento (90 dias), resumo de pedidos, validações pendentes e performance de vendas por colaborador.
Boas práticas aplicadas: Índices estratégicos em colunas de busca frequente, comentários em tabelas e colunas, constraints nomeadas e separação clara de responsabilidades entre entidades.


Figura 2: Estrutura das views analíticas e triggers automáticos implementados.
🔧 Como Executar

Certifique-se de ter o PostgreSQL instalado e rodando.
Clone o repositório.
Execute o script no banco de dados desejado:

bashpsql -U seu_usuario -d seu_banco -f schema.sql

As tabelas, índices, triggers e views serão criados automaticamente.

Figura 3: Representação visual dos relacionamentos entre as tabelas do sistema.
