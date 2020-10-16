# angular-emstdv-qppymt

Construindo localmente
Para construir seu aplicativo localmente ou para produção, baixe o código-fonte do seu projeto StackBlitz clicando no ícone no menu esquerdo em frente para baixar seus arquivos.Download ProjectProject

Depois de ter o código-fonte baixado e descompactado, instale e sirva seu aplicativo com o CLI Angular.Node.js

A partir do terminal, instale o CLI Angular globalmente com:

content_copy
npm install -g @angular/cli
Isso instala o comando em seu sistema, que é o comando que você usa para criar novos espaços de trabalho, novos projetos, servir sua aplicação durante o desenvolvimento ou produzir compilações para compartilhar ou distribuir.ng

Crie um novo espaço de trabalho ANGULAR CLI usando o novo comando ng:

content_copy
ng new my-project-name
Em seu novo aplicativo gerado pela CLI, substitua a pasta pela do seu download e, em seguida, execute uma compilação./srcStackBlitz

content_copy
ng build --prod
Isso produzirá os arquivos que você precisa implantar.

Se o comando acima lançar um erro sobre pacotes ausentes, adquiree as dependências ausentes no arquivo do seu projeto local para corresponder ao do projeto StackBlitz baixado.ng buildpackage.json

Hospedagem do projeto construído
Os arquivos da pasta são estáticos. Isso significa que você pode hospedá-los em qualquer servidor web capaz de servir arquivos (como, Java, .NET) ou qualquer backend (como Firebase, Google Cloud ou App Engine).dist/my-project-nameNode.js

Hospedagem de um aplicativo Angular no Firebase
Uma das maneiras mais fáceis de obter o seu site ao vivo é hospedá-lo usando Firebase.

Inscreva-se para uma conta de base de incêndio no Firebase.
Crie um novo projeto, dando-lhe qualquer nome que você gosta.
Adicione os esquemas que lidarão com sua implantação usando .@angular/fireng add @angular/fire
Conecte seu CLI à sua conta do Firebase e inicialize a conexão com o seu projeto usando e .firebase loginfirebase init
Siga as instruções para selecionar o projeto que você está criando para hospedagem.Firebase

Selecione a opção no primeiro prompt.Hosting
Selecione o projeto que você criou anteriormente no Firebase.
Selecione como diretório público.dist/my-project-name
Implante seu aplicativo com .ng deploy
Uma vez implantado, visite https://your-firebase-project-name.firebaseapp.com para vê-lo ao vivo!
