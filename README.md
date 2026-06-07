# Teste Pulsador Balde ao Pé v2.3

App PWA offline-first para avaliação prática de campo das pulsadas do pulsador de ordenhadeira balde ao pé.

## Arquivos

- `index.html`: app completo.
- `manifest.json`: instalação como PWA no Android/Chrome.
- `service-worker.js`: cache offline do app.
- `icons/`: ícones 192 e 512 px.

## Como subir no GitHub Pages

1. Crie um repositório no GitHub, por exemplo `teste-pulsador`.
2. Envie todos os arquivos deste pacote para a raiz do repositório.
3. Vá em **Settings > Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/root`.
6. Salve.
7. Abra a URL publicada pelo GitHub Pages.

## Mensagem de commit sugerida

```text
Publicar Teste Pulsador Balde ao Pé v2.3 como PWA
```

## Teste obrigatório

1. Abrir no Chrome Android pela URL do GitHub Pages.
2. Fazer teste manual com 15 segundos, inserir pulsadas e gerar resultado.
3. Verificar se o histórico foi salvo.
4. Exportar CSV e JSON.
5. Instalar como app pelo menu do Chrome.
6. Abrir o app instalado sem internet para confirmar cache offline.
7. Testar microfone apenas pela URL HTTPS/GitHub Pages ou app instalado. Em `file://`, o microfone pode ser bloqueado pelo navegador.

## Observação técnica

A medição por microfone é uma triagem de campo e depende do ruído ambiente. Para diagnóstico técnico completo, usar vacuômetro, pulsógrafo ou técnico especializado.
