# teste4

Exportado pelo Navegador 3D em 2026-09-24.

## Abrir no computador, sem publicar nada

Aberta direto do disco, a página não carrega o modelo: o navegador bloqueia por segurança.
Use um servidor local. Em `localhost` tudo funciona, inclusive a câmera.

Com o Node instalado, dentro desta pasta:

```
npx --yes serve .
```

Ou, de dentro da pasta do editor Navegador 3D:

```
npm run servir -- caminho/desta/pasta
```

Depois abra o endereço que aparecer, algo como http://localhost:8080/.

## Publicar no GitHub Pages

1. Envie **todos** os arquivos desta pasta para um repositório, mantendo-os no mesmo nível.
2. Em Settings, Pages, escolha o branch e a pasta (raiz ou /docs).
3. Abra o endereço do Pages. A página inicial mostra o modelo em 3D e o botão de AR.

Os caminhos são todos relativos, então funciona na raiz do site ou em qualquer subpasta.
Não separe os arquivos em subpastas: a página de AR procura o modelo e a imagem ao lado dela.

## Arquivos

- `index.html`: página inicial. Mostra o modelo em 3D (funciona no computador), a imagem
  para imprimir e os botões de AR.
- `ar.html`: a realidade aumentada, por câmera, apontando para a imagem impressa.
- `teste4.glb`: o modelo completo, abre em qualquer visualizador glTF.
- `imagem-alvo.jpg`: **imprima este arquivo**. O modelo aparece sobre ele.
- `alvo.mind`: a mesma imagem, preparada para o rastreio.
- `projeto.json`: câmera, grade e configuração de AR.
- `preview.png`: captura da cena.
- `.nojekyll`: evita que o GitHub Pages esconda arquivos.

Tamanho: a imagem impressa representa 1,437 m da cena.
Imprimir com essa largura deixa o modelo em tamanho real; maior ou menor, o modelo acompanha o papel.
Na AR dá para ajustar na hora: botões Maior, Menor e Girar, ou pinça e arrastar com o dedo.

## Se a AR não funcionar

- A câmera só abre em endereços https:// ou em localhost. Abrir o arquivo direto do
  computador mostra o modelo 3D, mas não a AR.
- Navegadores embutidos do Instagram, WhatsApp e afins bloqueiam a câmera: toque nos três
  pontinhos e escolha "Abrir no navegador".
- Se a imagem não é reconhecida: imprima maior (pelo menos do tamanho de uma folha A5),
  use boa luz sem reflexo no papel, e enquadre a imagem inteira, não só um pedaço.
- Imagens com bastante detalhe, contraste e textura são reconhecidas melhor que uma arte
  lisa ou muito clara; o editor já avisa isso na hora de escolher a imagem.

Convenção: Y para cima, metros.
