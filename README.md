# Jogo de Sobrevivência — caderno de desenvolvimento

Área de trabalho para organizar as ideias, as imagens, a história e os personagens de um jogo de sobrevivência. Tudo o que você adiciona aqui aparece num site visual, publicado pelo GitHub Pages.

## Onde fica cada coisa

| Pasta | O que vai nela | Seção do site |
|---|---|---|
| `_historia/` | Um arquivo por capítulo da história | História (linha do tempo) |
| `_personagens/` | Um arquivo por personagem | Personagens |
| `_ideias/` | Um arquivo por ideia (mecânica, mapa, item...) | Ideias |
| `_galeria/` | Um arquivo por foto, com a descrição | Galeria |
| `imagens/` | As fotos em si (.jpg, .png, .webp, .svg) | — |
| `modelos/` | Modelos prontos para copiar (não aparecem no site) | — |

Os arquivos que vêm com **(Exemplo.)** no texto podem ser apagados ou editados.

## Como adicionar uma foto com descrição (pelo site do GitHub)

1. Abra a pasta `imagens/`, clique em **Add file → Upload files** e envie a foto. Use um nome simples, sem espaços nem acentos, por exemplo `cabana-no-lago.jpg`.
2. Abra a pasta `_galeria/` e clique em **Add file → Create new file**.
3. Dê um nome terminado em `.md`, por exemplo `cabana-no-lago.md`.
4. Copie o conteúdo de `modelos/foto.md`, troque o título, o nome da imagem e a descrição, e clique em **Commit changes**.

Para um capítulo, um personagem ou uma ideia, o caminho é o mesmo: crie o arquivo na pasta certa usando o modelo correspondente. A foto é opcional; se não tiver, apague a linha `imagem:`.

Exemplo de um arquivo de personagem:

```
---
nome: "Marta"
papel: "Aliada"
imagem: /imagens/marta.jpg
---
Médica que vive escondida numa estação de rádio abandonada.
```

A parte entre os dois `---` são os dados do cartão. Mantenha as aspas e os dois-pontos. Abaixo do segundo `---` vai o texto livre.

Na história, o campo `ordem` define a posição do capítulo (1, 2, 3...).

## Ligar o site (só uma vez)

1. No repositório, abra **Settings → Pages**.
2. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
3. Em **Branch**, escolha `main` e a pasta `/ (root)`, e clique em **Save**.
4. Depois de 1 ou 2 minutos, o endereço aparece no topo dessa página. Será algo como `https://alexandreborne2354-lab.github.io/jogo_sobrevivecia/`.

Cada mudança que você salvar atualiza o site sozinha em cerca de um minuto.

> **Repositório privado:** no plano gratuito do GitHub, o GitHub Pages só funciona em repositórios públicos. Para manter o repositório privado e ainda ter o site, é preciso o plano GitHub Pro. Sem o site, os arquivos continuam organizados e legíveis aqui no GitHub.

## Mudar o visual

- Título e frase do topo: `_config.yml`.
- Cores: no início de `assets/estilo.css`.
