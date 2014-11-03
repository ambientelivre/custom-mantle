simple-mantle
=============

Ambiente Livre - Simple Custom Mantle Interface for Basic and Business Users

Funcionalidades implementadas:
- Inibe painel de administração do Pentaho BI-Server.
- Inibe edição / exclusão de artefatos de BI (Dashboards,Reports, Analises ).
- Mescla a perspectiva Browser com a Opened em uma mesma perspectiva.
- Mantem funcionalidades nativas do mantle
- Adaptação do Tema Onyx
- Mantém a interface nativa para o usuário Admin
- Aculta barra lateral de navegação ( Browser )
- Dispara Saiku no Login
- Dispara Dashboard Home no Login


Instalação
- Altere o tema padrão do Pentaho biserver para Onix.
- Renomeie o apague o diretório ../biserver-ce/tomcat/webapps/pentaho/mantle
- crie um diretório mantle em branco no mesmo local e copie todo o conteúdo desto git na mesma
- cria na pasta public um dashboard com CDE com o nome home (home.wcdf)
- Reinicie o biserver
- Limpe os caches do browser.

Dependências
- Saiku
- CDE

Versão Pentaho BI-Server
5.1 ou Superior


Suporte: http://www.ambientelivre.com.br 


