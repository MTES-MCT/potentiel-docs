# Installation du ChatBot

**CODE du ChatBot Potentiel :** \
\<script type="text/javascript">window.$crisp=\[];window.CRISP\_WEBSITE\_ID="cb5c5c5f-a671-43cf-b84f-cd514ea51495";(function(){d=document;s=d.createElement("script");s.src="https://client.crisp.chat/l.js";s.async=1;d.getElementsByTagName("head")\[0].appendChild(s);})();\</script>



**Pour que le scénario se déclenche en cliquant sur un bouton :**                                                              Ajoutez le code au handler Onclick de votre bouton

\
**Pour que le scénario se déclenche sans actions, il faut envoyer un message en tant que visiteur via SDK, vous devez utiliser cette syntaxe :**&#x20;

$crisp.push(\["do", "message:send", \["text", "Hello there!"]]);\
Et utiliser un message qui correspond à ce que vous paramétrez dans le scénario.\
[https://docs.crisp.chat/guides/chatbox-sdks/web-sdk/dollar-crisp/](https://docs.crisp.chat/guides/chatbox-sdks/web-sdk/dollar-crisp/)
