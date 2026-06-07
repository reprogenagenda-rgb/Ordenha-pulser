# Teste Pulsador Balde ao Pé v2.5

App PWA offline-first para avaliação prática de campo das pulsadas do pulsador de ordenhadeira balde ao pé.

## Objetivo

Medir, depurar e comparar o som do pulsador com o padrão prático de campo:

- referência: 60 pulsadas/minuto;
- padrão regular ideal: 56 a 60 ppm;
- regularidade sonora mínima recomendada: 85%;
- falhas detectadas: 0 para aprovação funcional.

## Arquivos

- `index.html`: app completo.
- `manifest.json`: instalação como PWA no Android/Chrome.
- `service-worker.js`: cache offline do app.
- `icons/`: ícones 192 e 512 px.

## Novidades da v2.5

- Módulo **Depuração do Som Coletado**.
- Redução prática de ruído via envelope/RMS suavizado.
- Limiar automático combinado com sensibilidade manual.
- Detecção de picos compatíveis com pulsação.
- Ignora picos muito próximos para evitar contagem dupla.
- Calcula intervalo médio entre pulsos.
- Calcula regularidade percentual.
- Detecta falhas/pausas anormais.
- Compara o som depurado com o padrão de 60 ppm.
- Resultado exibe: ruído de fundo, qualidade do sinal, regularidade sonora, falhas, diferença para 60 ppm e compatibilidade.

## Como subir no GitHub Pages

1. Crie um repositório no GitHub, por exemplo `teste-pulsador`.
2. Envie todos os arquivos deste pacote para a raiz do repositório.
3. Vá em **Settings > Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/root`.
6. Salve.
7. Abra a URL publicada pelo GitHub Pages.

## Estrutura correta

```text
index.html
manifest.json
service-worker.js
README.md
icons/
  icon-192.png
  icon-512.png
```

## Mensagem de commit sugerida

```text
Atualizar Teste Pulsador para V2.5 com som depurado
```

## Teste obrigatório

1. Abrir no Chrome Android pela URL do GitHub Pages.
2. Fazer teste manual com 15 segundos, inserir pulsadas e gerar resultado.
3. Testar o botão de som padrão regular 60 ppm.
4. Ir em Microfone e gravar 15 a 30 segundos próximo ao pulsador.
5. Confirmar se aparecem ruído, qualidade do sinal, intervalo médio, regularidade, falhas e diferença para 60 ppm.
6. Gerar resultado e conferir se os dados sonoros aparecem no relatório.
7. Conferir se o histórico foi salvo.
8. Exportar CSV e JSON.
9. Instalar como app pelo menu do Chrome.
10. Abrir o app instalado sem internet para confirmar cache offline.

## Observação técnica

A comparação sonora é triagem prática de campo. O app não substitui vacuômetro, pulsógrafo, avaliação de vácuo, teste de relação de pulsação ou técnico especializado.
