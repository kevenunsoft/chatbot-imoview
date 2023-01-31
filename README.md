## Como utilizar o chatbot integrado com o IMOVIEW em seu site

Veja abaixo os passos necessários utilizar o chatbot do Imoview.

### 1º - Faça login em sistema Imoview e clique em configurações

Link para acessar seu sistema, https://app.imoview.com.br/.

Exemplo:

### 2º - Vá até a seção de chatbot(aba CRM)

Nesta seção é possível configurar o avatar, lado, mensagens e opções que irá aparecer no chatbot em seu site.

![image](https://user-images.githubusercontent.com/78874946/215841322-0f15fb1d-3246-4bd8-bc11-b459355e63f0.png)


### 3º - Copie o script gerado na subseção "Implantação" e solicite ao desenvolvedor do site que instale antes do elemento ```</body>```</br>

Exemplo:

```html {.line-numbers}
<script type="text/javascript">
  IMOVIEW.Exec({
    corFundo: "#533D8B", //Opcional - Cor hexadecimal primária do chat, recomendamos a cor primário do site.
    avatarUrlChat: "https://s3.imoview.com.br/avatar.jpg", //Cole a URL completa do avatar que aparecerá no chat ao abri-lo"
    mensagemChatFechado: "Como podemos <strong>te ajudar</strong> ?", //Texto que irá aparecer para o cliente clicar no chat
    posicao: "direito", //Lado que o botão ficará -- direito ou esquerda
    nomeHeaderChat: "XXX", // Nome que aparecerá do chat ao abri-lo
    rota: "demo", //Rota da imobiliária - é obtido no sistema Imoview clicando no menu canto direito superior e clique em "Detalhes convênio"
  });
</script>
```

**Obs:** o campo rota é obtido no sistema Imoview, clicando no menu canto direito superior e clique em "Detalhes convênio",
