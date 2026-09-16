# meu-projeto

Exportado pelo Navegador 3D em 2026-09-16.

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
- `ar.html`: a realidade aumentada.
- `meu-projeto.glb`: o modelo completo, abre em qualquer visualizador glTF.
- `imagem-alvo.png`: **imprima este arquivo**. O modelo aparece sobre ele.
- `alvo.mind`: a mesma imagem, preparada para o rastreio.
- `projeto.json`: câmera, grade e configuração de AR.
- `preview.png`: captura da cena.
- `.nojekyll`: evita que o GitHub Pages esconda arquivos.

Tamanho na AR: 1 (1 = o modelo aparece do tamanho da imagem).
Dá para ajustar na hora, pelos botões Maior e Menor.

## Se a AR não funcionar

- A câmera só abre em endereços https:// ou em localhost. Abrir o arquivo direto do
  computador mostra o modelo 3D, mas não a AR.
- Navegadores embutidos do Instagram e do WhatsApp bloqueiam a câmera: toque em
  "Abrir no navegador".
- Se a imagem não é reconhecida: imprima maior, use boa luz, evite reflexo e enquadre
  ela inteira. Imagens com bastante detalhe e contraste funcionam melhor.

Convenção: Y para cima, metros.
