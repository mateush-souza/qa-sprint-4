MotoConnect - Testes Automatizados e Manuais
Mostrar Imagem
Mostrar Imagem
Este repositório contém a documentação e artefatos dos testes manuais e automatizados desenvolvidos para a aplicação MotoConnect como parte da entrega do 4º Sprint.

📋 Visão Geral
O projeto de testes abrange validações completas das funcionalidades principais do sistema, incluindo gerenciamento de usuários e veículos. A estratégia de testes combina abordagens manuais e automatizadas para garantir cobertura adequada e qualidade do software.

🧪 Testes Manuais
Os testes manuais foram planejados e documentados no Azure Boards, cobrindo cenários de uso das funcionalidades principais:

Módulo de Usuários (Users)
Módulo de Veículos (Vehicles)

Acesso aos Testes
Os casos de teste e planos de execução estão disponíveis no Azure DevOps:
👉 Plano de Testes no Azure Boards

🤖 Testes Automatizados
Os testes automatizados foram implementados utilizando Postman e cobrem os seguintes endpoints da API:
EndpointMétodoDescrição/UserPOSTCriar novo usuário/UserGETListar todos os usuários/VehiclesPOSTCadastrar nova motocicleta/VehiclesGETListar todas as motocicletas
Recursos Implementados

✅ Headers padrão configurados
✅ Variáveis de ambiente para facilitar configuração
✅ Validação de status codes
✅ Testes de resposta da API
✅ Scripts de pré-requisição quando necessário

Demonstração em Vídeo
Um vídeo completo demonstrando a configuração e execução dos testes está disponível:
🎥 Vídeo - Testes Automatizados no Postman

📁 Estrutura do Repositório
MotoConnect-Tests/
│
├── postman-collection/
│   └── MotoConnect_API_Tests.json    # Coleção Postman para importação
│
├── docs/
│   └── plano_testes_manuais.pdf      # (Opcional) Exportação do Azure Boards
│
└── README.md                          # Este arquivo

🚀 Como Executar os Testes Automatizados
Pré-requisitos

Postman instalado
Acesso à API do MotoConnect
Credenciais válidas para autenticação

Passo a Passo

Importe a Coleção

Abra o Postman
Clique em Import
Selecione o arquivo MotoConnect_API_Tests.json da pasta postman-collection/


Configure o Ambiente

Crie um novo ambiente chamado MotoConnect
Adicione as seguintes variáveis:



     baseUrl: <URL_DA_API>
     token: <TOKEN_DE_AUTENTICACAO>

Execute os Testes
Execute as requisições na seguinte ordem:

🔹 Criar Usuário
🔹 Listar Usuários
🔹 Cadastrar Moto
🔹 Listar Motos


Visualize os Resultados
Os resultados dos testes aparecerão na aba Tests de cada requisição no Postman.

Execução em Lote
Para executar todos os testes de uma vez:

Clique em Run collection no menu da coleção
Selecione o ambiente MotoConnect
Clique em Run MotoConnect_API_Tests


📊 Cobertura de Testes
Os testes cobrem os seguintes aspectos:

✅ Validação de Status HTTP - Verifica se os códigos de resposta estão corretos
✅ Validação de Schema - Garante que a estrutura dos dados retornados está correta
✅ Testes de Integração - Verifica o fluxo completo de operações
✅ Manipulação de Dados - Valida criação, leitura e listagem de recursos


📝 Observações Importantes

Todos os testes foram realizados com dados controlados para garantir consistência
A execução automatizada permite validação rápida e repetível dos endpoints principais
Os testes manuais complementam a cobertura com cenários de uso mais complexos
Recomenda-se executar os testes automatizados após cada deploy ou alteração na API


👥 Equipe
Projeto desenvolvido como parte do 4º Sprint da disciplina.

📞 Suporte
Para dúvidas sobre os testes:

Consulte o vídeo de demonstração
Verifique a documentação no Azure Boards
Entre em contato com a equipe do projeto


📄 Licença
Este projeto é parte de um trabalho acadêmico.

Última atualização: Sprint 4 - 2024
