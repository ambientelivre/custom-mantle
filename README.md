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


FAQ:

Como alterar os nomes e Páginas que abrem no simple-mantle

Para a tela do Saiku
Acesse o arquivo  ../biserver-ce/tomcat/webapps/pentaho/mantle/browser/js/browser.js e no arquivo ../biserver-ce/tomcat/webapps/pentaho/mantle/home/index.jsp  procure pela função window.parent.openURL e   mude os parâmetros desejados da função

Modelo Padrão da Função:

window.parent.openURL('Analise','Analise','content/saiku-ui/index.html?biplugin5=true');

- O primeiro parâmetro e o nome que vai aparece Internamente  ( ex. Analise )
- Segundo parâmetro e o nome que na Aba ( ex. Analise )
- Terceiro parâmetros o atalho do dashboard, visão , report ou tela do PUC que deseja abrir.


Para a tela Home

Acesse o arquivo../biserver-ce/tomcat/webapps/pentaho/mantle/home/index.jsp  procure pela função window.top.mantle_openRepositoryFile e  mude os parâmetros desejados da função

window.top.mantle_openRepositoryFile("/public/home.wcdf", "RUN");

- Primeiro parâmetro  Local do arquivo que será aberto
- Segundo parâmetro deve ser RUN para abrir o artefato.



Suporte: http://www.ambientelivre.com.br 


