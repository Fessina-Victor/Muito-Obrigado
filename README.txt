# WebAR — Muito Obrigado

Projeto de Realidade Aumentada usando MindAR + A-Frame.

## Estrutura

- `index.html` — página WebAR corrigida, usando o robô da versão 2.
- `targets.mind` — target compilado para `marcador_webAR.png`.
- `marcador_webAR.png` — imagem que deve ser reconhecida pela câmera.

## Fluxo

QR Code → página WebAR → câmera → reconhecimento da imagem → robô holográfico + “MUITO OBRIGADO!”

## Publicação no GitHub Pages

Envie os três arquivos principais (`index.html`, `targets.mind` e `marcador_webAR.png`) para o repositório e ative o GitHub Pages.

Importante: teste pelo endereço HTTPS do GitHub Pages em um celular, permitindo o acesso à câmera.

## Correção aplicada

A versão recebida tinha a configuração do renderer do A-Frame escrita com separadores incorretos:

`colorManagement: true, physicallyCorrectLights; antialias: true`

Ela foi corrigida para:

`colorManagement: true; physicallyCorrectLights: true; antialias: true`

O arquivo `targets.mind` recebido também foi verificado: ele contém 1 target e informa imagem de 1024 × 1536, compatível com o marcador enviado.
