Curso de Engenharia de Software - UniEVANGÉLICA 
Disciplina de Sistemas Gerenciadores de Banco de Dados 
Dev: Thiago Silva Soares 
DATA: 02/07/2023

1 Evento que desencadeia a requisição no frontend:

O ciclo de vida começa quando o usuário realiza uma ação na interface do usuário, como clicar em um botão ou preencher um formulário. Esse evento aciona um código JavaScript no frontend que captura a ação do usuário e prepara uma requisição HTTP para ser enviada ao servidor backend.

2 Envio da requisição para o servidor backend:

O código JavaScript no frontend cria um objeto de requisição HTTP, que contém informações como o método HTTP (por exemplo, GET, POST, PUT, DELETE), o URL do servidor backend e quaisquer parâmetros ou dados que devem ser enviados junto com a requisição. Em seguida, a requisição é enviada para o servidor backend usando a função apropriada, geralmente fornecida por uma biblioteca ou framework no frontend, como o Axios ou o fetch.

3 Determinação do destino da requisição no servidor backend:

No servidor backend, existem componentes responsáveis por determinar o destino da requisição com base no URL e no método HTTP. O roteador é o componente que analisa o URL da requisição e decide qual controlador deve ser responsável por lidar com a requisição. O roteador mapeia o URL para uma rota específica no aplicativo backend, que é associada a um controlador correspondente.

4 Responsabilidades do roteador e do controlador no backend:

O roteador é responsável por receber a requisição do frontend, analisar o URL e encaminhá-la para o controlador apropriado com base na rota mapeada. O controlador é o componente que contém a lógica de negócios específica para lidar com a requisição. Ele recebe a requisição do roteador, processa os dados e interage com outros componentes do backend, como modelos e serviços.

5 Interação do Model com o banco de dados:

Se a requisição envolver acesso a dados, o controlador pode interagir com o modelo (também conhecido como camada de modelo ou camada de acesso a dados) para recuperar ou modificar informações no banco de dados. O modelo é responsável por realizar operações de leitura/gravação no banco de dados e fornecer os dados relevantes para o controlador.

6 Criação e envio da resposta no backend:

Com base nas informações processadas pelo controlador e pelo modelo, o controlador cria uma resposta adequada para a requisição. A resposta pode conter dados formatados, mensagens de status HTTP e cabeçalhos adicionais. Em seguida, o controlador envia a resposta de volta ao frontend, normalmente retornando-a como uma resposta HTTP.

7 Processamento da resposta no frontend e atualização da interface do usuário:

O frontend recebe a resposta HTTP do servidor backend. O código JavaScript no frontend é responsável por processar a resposta e atualizar a interface do usuário de acordo. Isso pode envolver a extração de dados da resposta e a exibição desses dados na interface do usuário, bem como a manipulação de erros ou mens