Com este app aprendemos sobre:

O que é navegação e sua importância:
Vimos que a navegação é a funcionalidade em que o usuário pode ir (navegar) de uma tela a outra. No desenvolvimento mobile, precisamos criar as telas e a navegação entre essas telas. Também aprendemos que existem formas diferentes de implementar a navegação em um aplicativo. A navegação é importante, pois permite que o usuário navegue de uma tela para outra e não fique preso em uma única tela, por exemplo.
Tipos de navegação:

1) Empilhada ou stack: o primeiro tipo de navegação, bastante utilizado em aplicativos, envolve uma sequência de telas que vão sendo “empilhadas”, ou seja, armazenadas na memória do app, permitindo que o usuário retorne para uma tela anterior.

2) Aba ou tab: o segundo tipo de navegação de aba ou tab é o mais simples de programar, por isso vamos começar nossos estudos por ele. A princípio, a navegação por tab não permite voltar para uma tela anterior, mas sim mudar de tela criando dois ou mais contextos de navegação.

3) Menu lateral ou drawer: o tipo de navegação drawer abre um menu lateral, permitindo a navegação para outras telas a partir desse menu. A princípio, a navegação drawer, também, não permite voltar para uma tela anterior. E também é muito semelhante a navegação por abas, pois permite a criação de contextos diferentes.

4) Deeplink: os deeplinks são, literalmente, links que permitem o acesso para a aplicação de fora do app. Um exemplo disso é quando recebemos uma notificação de cupom, em um app de delivery, que nos leva diretamente para uma tela em que há uma promoção.

Instalar a biblioteca react-navigation: Vimos como instalar esta biblioteca de navegação na versão 6 no nosso projeto. Seguimos os 4 passos descritos na documentação:

1) Instalar a biblioteca por meio do gerenciador de pacotes npm;

2) Instalar as dependências usando Expo ou React Native puro;

3) Instalar as dependências nativas no iOS;

4) Adicionar o onCreate na MainActivity no código nativo Android para evitar crashes.

Utilizar a biblioteca react-navigation: Para criar o menu inferior, com a navegação por abas (tab), vimos que era necessário, além da biblioteca que já instalamos, instalar também o pacote deste tipo de navegação com o npm. Então, concentramos nossas rotas de navegação dentro da pasta rotas, que são os arquivos que descrevem as regras da nossa navegação.

Instalar a dependência do tipo de navegação stack:

Assim como o botton-tab, precisamos instalar a dependência relacionada à navegação em pilha: a native-stack.
Criar rotas usando a navegação em pilha:

Criamos rotas para navegar entre as telas: Home ou Melhores Produtores, Produtor e Cesta. Adicionamos essa rota dentro dos contextos da navegação em abas.
Passamos os parâmetros do produtor:

Para saber qual produtor exibir, usamos o hook useRoute para receber os parâmetros passados pelo navigation.navigate.
Finalização da tela de Produtor:

Com auxílio de componentes e estilos prontos, implementamos a tela de produtor estilizada, listando também as cestas.

Ocultar os títulos da navegação:

Removemos os títulos desnecessários, passando o parâmetro headerShown: false na screenOptions do Tab.Navigator.
Implementar a ação de voltar:

Executamos a ação de voltar da navegação, quando clicamos no botão de voltar do topo, usando a função navigation.goBack().
Inserir ícones customizados no menu inferior:

Para incrementar a navegação, configuramos ícones SVG por meio da propriedade tabBarIcon na screenOptions do Tab.Navigator.