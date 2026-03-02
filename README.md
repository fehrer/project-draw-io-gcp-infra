📌 Desafio – Modelagem de Organização e Grupos de Acesso
📖 Objetivo

Este projeto tem como objetivo representar, por meio de diagrama criado no Draw.io, uma estrutura organizacional com segregação de departamentos, sistemas e ambientes, aplicando conceitos de controle de acesso baseado em grupos (RBAC – Role Based Access Control).

🏢 Estrutura Organizacional

A organização modelada é a Tecnologia Fehrer, composta por dois departamentos principais:

Helpdesk

Financeiro

Cada departamento é responsável por um sistema específico:

Helpdesk → GLPI

Financeiro → ERP

🌎 Separação de Ambientes

Cada sistema foi segmentado em dois ambientes distintos:

DEV (Desenvolvimento)

PROD (Produção)

Essa separação garante:

Isolamento entre ambiente de testes e ambiente produtivo

Redução de riscos operacionais

Maior controle de mudanças

Aplicação de políticas de segurança distintas

🔐 Modelo de Controle de Acesso

Foi adotado o modelo RBAC (Role Based Access Control), onde:

Usuários não recebem permissões diretamente

O acesso é concedido através de grupos

Cada grupo possui uma função específica dentro de um ambiente


Exemplo de Grupos Criados:

Para o sistema GLPI:


GRP_GLPI_DEV_READ

GRP_GLPI_DEV_ADMIN

GRP_GLPI_PROD_READ

GRP_GLPI_PROD_ADMIN


Para o sistema ERP:

GRP_ERP_DEV_READ

GRP_ERP_DEV_ADMIN

GRP_ERP_PROD_READ

GRP_ERP_PROD_ADMIN
