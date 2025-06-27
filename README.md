![Captura de tela 2025-06-27 030318](https://github.com/user-attachments/assets/ad323966-f378-41e0-ac03-dbc8dd2f5402)
![Captura de tela 2025-06-27 030323](https://github.com/user-attachments/assets/760cb6a6-2716-42d7-ae00-dc966fee6549)
![Captura de tela 2025-06-27 030327](https://github.com/user-attachments/assets/f9a4ff04-1b1a-4b65-a232-f457904253d5)
![Captura de tela 2025-06-27 030331](https://github.com/user-attachments/assets/007671a7-e02c-40c4-be0b-ad8cbb6608cb)
Descrição
Este projeto consiste na criação de uma planilha profissional em Excel para controle e organização dos dados necessários à declaração do Imposto de Renda Pessoa Física (IRPF). A ferramenta foi desenvolvida para facilitar o registro de rendimentos, deduções, saldos bancários e simulação do imposto devido, tornando o processo mais prático, seguro e transparente.
Ideal para quem busca uma solução eficiente para centralizar informações fiscais e otimizar o preenchimento da declaração anual, agregando valor ao portfólio profissional.

Funcionalidades
Cadastro do contribuinte: Informações pessoais organizadas na aba TITULAR.

Gestão de rendimentos e saldos bancários: Registro detalhado de contas e valores na aba INFORMAÇÕES.

Controle de entradas e deduções: Lançamentos de rendimentos (holerite, freelance, etc.) e despesas dedutíveis (educacionais, dependentes, imóveis) na aba NOTAS.

Cálculo automático do IR: Simulação do imposto devido, faixa aplicável, deduções e saldo a pagar/restituir na aba SIMULAÇÃO IR.

Validações e navegação facilitada: Estrutura amigável, validações de dados e menus para facilitar o uso.

Recomendações fiscais: Dicas automáticas para planejamento tributário e organização de comprovantes.

Estrutura da Planilha
Aba	Descrição
TITULAR	Dados cadastrais do contribuinte
INFORMAÇÕES	Saldos bancários, total de rendimentos bancários, anexos de comprovantes
NOTAS	Lançamentos de entradas (rendimentos) e deduções, com totalização automática
SIMULAÇÃO IR	Cálculo do IRPF: base de cálculo, faixa, imposto devido, IR retido, saldo, recomendações
Planilha1	Referências de bancos e tipos de deduções
Como Utilizar
Preencha a aba TITULAR com seus dados pessoais.

Registre seus saldos e rendimentos bancários na aba INFORMAÇÕES, anexando comprovantes se necessário.

Lance todos os rendimentos e deduções na aba NOTAS, preenchendo as colunas de acordo com a categoria e valor.

Acesse a aba SIMULAÇÃO IR para visualizar automaticamente:

Total de rendimentos e deduções

Base de cálculo do IR

Faixa aplicável e cálculo do imposto devido

Valor de IR retido na fonte (preencha manualmente com o total dos informes)

Saldo a pagar ou a restituir

Recomendações fiscais

Confira as recomendações para otimizar sua declaração e evitar erros.

Tecnologias Utilizadas
Microsoft Excel (Web e Desktop)

Validações de dados e fórmulas condicionais

Estruturação de abas temáticas

Navegação facilitada e interface amigável

Exemplos de Fórmulas Utilizadas
Total de Rendimentos:
=SOMA(E9:E30) (aba NOTAS)

Total de Deduções:
=SOMA(J9:J30) (aba NOTAS)

Base de Cálculo:
=B5-B6 (aba SIMULAÇÃO IR)

Faixa do IR:
=SE(B7<=22847,76; "1ª Faixa (Isento)"; ...)

Cálculo do IR Devido:
=SE(B7<=22847,76; 0; SE(B7<=33919,80; B7*0,075-1713,58; ... ))

Saldo a Pagar:
=B23-B24 (IR Devido - IR Retido)

Como Rodar o Projeto
Baixe o arquivo Excel deste repositório.

Abra no Microsoft Excel (Web ou Desktop).

Siga as instruções de preenchimento em cada aba.

Consulte as recomendações para otimizar sua declaração.

Capturas de Tela
As imagens do projeto estão disponíveis na pasta /images deste repositório.

Aprendizados e Diferenciais
Aplicação prática de validação de dados e automação de cálculos fiscais.

Organização clara e profissional de informações fiscais.

Documentação detalhada, seguindo boas práticas de Markdown e GitHub.

Projeto pronto para ser incluído em portfólio profissional.

Referências
Documentação Oficial da Receita Federal

Boas práticas para README.md

Exemplo de Controle Financeiro
