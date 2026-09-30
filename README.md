# Simulador Educativo de Urna Eleitoral Eletrônica

Uma simulação de eleição com urna eletrônica criada para fins educativos.

Este projeto reproduz, de forma simples, a experiência de votação em uma urna eletrônica. Tem como objetivo ser utilizado em aulas, oficinas e outras atividades pedagógicas. Seu diferencial é permitir a personalização dos candidatos e contagem real de votos.

A proposta é ser simples e acessível: não precisa instalar programas ou ter conhecimentos de programação para configurar a urna. O arquivo final pode ser facilmente compartilhado e usado em qualquer dispositivo que possua um navegador de internet, sem precisar baixar aplicativos.

O código foi desenvolvido com assistência de IA (ferramenta Claude Pro) para uso pessoal em uma atividade pedagógica com crianças e adultos. Está disponibilizado abertamente para que outras pessoas possam utilizar para os mesmos fins.

**Atenção:** Não recomendamos o uso desta urna para eleições reais ou votações oficiais. O projeto não foi desenvolvido para garantir segurança, sigilo ou integridade dos votos.

## Funcionalidades:

* Personalização de candidatos com Nome, Legenda (número), Cargo e Foto.
* Configuração de senha para acesso de mesário.
* Emissão de Zerésima e Boletim de Urna.
* Possibilidade de liberação de urna somente com confirmação do mesário.
* Descrições informativas e orientações na própria ferramenta.

## Como usar a urna?

A urna funciona em um arquivo único que pode ser executado em computadores, celulares e tablets utilizando navegadores básicos. Nenhuma instalação adicional é necessária. Internet é necessária somente para carregar as fotos dos candidatos.

Abra o arquivo em um navegador como Chrome, Edge, Firefox ou Safari.

Digite o número da candidatura, confira nome e foto na tela e aperte CONFIRMA. Um número que não existe vira voto nulo. Repita para cada cargo e FIM.

**Observação:** A urna funciona apenas localmente. Portanto, a contagem de votos será válida somente naquele dispositivo. Sair e voltar da página não apaga os dados de votação, que ficam salvos em cachê. 

## Como configurar o mesário?

Antes de iniciar as votações, configure o mesário clicando no botão "Mesário" ao topo. Defina uma senha de 4 dígitos.

Com essa senha, é possível ver quantas pessoas votaram e definir se deseja exigir liberação do mesário a cada voto.

Também é possível acessar o Boletim de Urna e Zerar a urna, emitindo a Zerésima. Você pode "imprimir" a Zerésima e o Boletim de Urna tirando um print no celular ou usando Ctrl+P no computador.

## Como personalizar a urna?

Você pode alterar candidatos, números, cargos e atribuir imagens diretamente no arquivo HTML.

### 1\. Baixe e abra o arquivo

Baixe o arquivo `urna.html` (se for sua primeira vez usando o github, veja como baixar arquivos).

Abra a pasta Downloads do seu computador.

Clique com o botão direito no arquivo baixado e escolha **Abrir com → Bloco de Notas**.

### 2\. Edite o arquivo

Procure no arquivo de texto essa seção:



```
<script>
(function(){
  "use strict";

      // ============================================================
      // ✏️ CONFIGURAÇÃO DA URNA — EDITE SOMENTE ESTA PARTE
      //      Atente-se para não apagar as aspas, colchetes e vírgulas ao editar.
      // EXEMPLO: \["12","Maria Silva","Deputada","https://exemplo.com/maria.jpg"]
      // ============================================================

  var DADOS=/\*DADOS\*/\[
    \["Deputado",\[
      \["00","Nome da candidata","Deputada","https://link.com/foto.jpg"],
      \["00","Nome do candidato","Deputado","https://link.com/foto.jpg"],
      \["00","Nome du candidate","Deputade","https://link.com/foto.jpg"]
    ]],
    \["Governador",\[
      \["00","Nome da candidata","Governadora","https://link.com/foto.jpg"],
      \["00","Nome do candidato","Governador","https://link.com/foto.jpg"],
      \["00","Nome du candidate","Governadore","https://link.com/foto.jpg"]
    ]],
    \["Presidente",\[
      \["00","Nome da candidata","Presidenta","https://link.com/foto.jpg"],
      \["00","Nome do candidato","Presidente","https://link.com/foto.jpg"]
    ]]
  ];

  // Opcional: Editar título que aparece no topo da urna e no boletim.

  var TITULO="Eleição simulada";

    // ============================================================
    // ⛔ FIM DA ÁREA DE CONFIGURAÇÃO — NÃO EDITE O CÓDIGO ABAIXO DESTA LINHA
    // ============================================================
```



Substitua os dados de exemplo pelas informações desejadas.

Você pode adicionar ou remover candidatos seguindo o mesmo formato.

Mantenha as aspas, colchetes e vírgulas exatamente como estão. Se não tiver familiaridade com código, altere apenas o conteúdo entre aspas.

### 3\. Salve o arquivo

Salve normalmente após concluir as alterações.

Verifique se a extensão continua sendo `.html`.

### 4\. Teste a urna

Abra o arquivo `.html` no navegador para visualizar as alterações. Teste digitando os números inscritos.

Sempre que modificar algo, salve o arquivo e recarregue a página.

## Como adicionar fotos?

As imagens são carregadas a partir de um link público na internet.

Precisa ser o endereço direto do arquivo. Normalmente esses links terminam em .jpg, .jpeg, .png.

Nem todo link que contém uma foto é um link direto para a imagem. Se o endereço abrir uma página inteira em vez do arquivo da imagem, ele poderá não funcionar.

Se a foto estiver no seu computador ou celular, você pode enviá-la para sites como **Imgur** ou **Flickr**, que hospedam imagens gratuitamente. Crie uma conta e faça upload da imagem.

Após o envio, copie o endereço direto da imagem e utilize-o no campo correspondente.

A imagem precisa estar acessível publicamente. Links privados ou que exigem login normalmente não funcionarão.

A foto não é obrigatória. Você pode seguir sem inclui-la no código.

## Licença e finalidade

Este projeto é disponibilizado gratuitamente para **uso não comercial** conforme CC BY-NC 4.0.

Você pode copiar, adaptar, modificar e distribuir o projeto para fins educacionais, pessoais ou outros fins não comerciais, desde que mantenha a indicação de autoria e não utilize o projeto para obter vantagem comercial.

O projeto não pode ser vendido, incorporado a produtos ou serviços comerciais, nem utilizado como parte de uma atividade comercial sem autorização prévia da autora.


