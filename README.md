<p align="center"><img src="logo.png" alt="WAZ" width="420"></p>

<h1 align="center">WAZ · Glass</h1>

<p align="center">Wallpapers animados em loop na <b>Nova Guia</b> do Chrome, com busca em vidro, atalhos, relógio e cores personalizáveis.</p>

---

## ✨ Recursos
- Vídeo (MP4/WebM), GIF ou imagem como wallpaper, em loop e com transição suave
- Galeria de wallpapers, com troca automática opcional
- Busca em vidro que brilha com a cor do vídeo (ou a cor que você escolher)
- Relógio opcional com fonte do computador ou enviada por você
- Controle de tamanho da busca, dos atalhos e do relógio
- Relógio digital ou **analógico** com neon, sombras, moldura de vidro, gradiente metálico e ponteiros suaves
- Modo desempenho para vídeos mais fluidos (ativa sozinho se detectar travadas)
- Funciona no **Chrome** e no **Firefox**
- 100% local: nenhum dado sai do seu navegador

## 📥 Instalação passo a passo

### 1. Baixar
1. Acesse a aba **[Releases](../../releases/latest)** deste repositório.
2. Em **Assets**, clique em **WAZ-chrome-store.zip** para baixar.

### 2. Extrair
1. Abra a pasta **Downloads**.
2. Clique com o botão direito em `WAZ-chrome-store.zip` e escolha **Extrair tudo...**
3. Clique em **Extrair**. Confira se, dentro da pasta, aparecem os arquivos `manifest.json`, `newtab.html` e `newtab.js`.

> ⚠️ O Chrome **não** lê arquivos de dentro do zip. É preciso extrair antes.

### 3. Carregar no Chrome
1. Abra o Chrome e digite `chrome://extensions` na barra de endereço.
2. Ative o **Modo do desenvolvedor** (canto superior direito).
3. Clique em **Carregar sem compactação**.
4. Selecione a pasta extraída (a que contém o `manifest.json`) e clique em **Selecionar pasta**.

### 4. Usar
1. Abra uma nova aba (`Ctrl + T`).
2. Passe o mouse no canto inferior direito e clique no botão de vídeo para abrir o painel.
3. Clique em **+ Adicionar vídeo, GIF ou imagem** (ou arraste o arquivo para a tela).
4. Ajuste cores, tamanhos e relógio como quiser.

> Instalou pelo botão verde **Code > Download ZIP**? Extraia e selecione a pasta `extension/`.

## 🦊 Instalação no Firefox
1. Em **[Releases](../../releases/latest)**, baixe **WAZ-firefox.zip** e extraia.
2. No Firefox, abra `about:debugging#/runtime/this-firefox`.
3. Clique em **Carregar extensão temporária...** e selecione o arquivo `manifest.json` da pasta extraída.
4. Abra uma nova aba.

> No modo temporário o Firefox remove a extensão ao ser fechado. A instalação permanente exige assinatura pelo [addons.mozilla.org](https://addons.mozilla.org) (gratuito).
> Limitações do Firefox: o cursor fica na barra de endereço ao abrir a aba (clique na busca para digitar) e a opção "Fontes do PC" não existe (use "Enviar fonte").

## ❓ Problemas comuns
| Problema | Solução |
|---|---|
| "O arquivo de manifesto está faltando" | Você selecionou a pasta errada. Selecione a que contém o `manifest.json` diretamente. |
| O vídeo não toca | Use MP4 (H.264) ou WebM. Vídeos em HEVC/H.265 não são suportados pelo Chrome. |
| Aparece "Personalizar o Chrome" embaixo | É um rodapé nativo do Chrome. Clique com o botão direito nele e escolha **Ocultar rodapé na página Nova guia**. |
| Erro depois de atualizar | Substitua os arquivos na pasta que o Chrome usa, clique em **↻** na extensão e depois em **Remover tudo** na tela de erros. A versão aparece no fim do painel da extensão. |
| Perdi meus wallpapers | O Chrome guarda os dados por instalação. Ao carregar de uma pasta nova, adicione-os de novo. |

## 🔄 Atualizar
Baixe a nova versão em **Releases**, substitua os arquivos da pasta antiga e clique em **↻ Recarregar** na extensão em `chrome://extensions`.

## 🗂 Estrutura
```
extension/   código da extensão (manifest do Chrome, html, css, js, ícones)
firefox/     manifest.json específico do Firefox
docs/        termos de uso e política de privacidade
store/       textos e checklist para a Chrome Web Store
scripts/     build.sh gera os .zip (Chrome e Firefox)
```

## ⚠️ Limitações
O Chrome só permite que extensões personalizem a **Nova Guia**, não a barra de abas e de endereço.

---
[Termos de Uso](docs/terms.md) · [Política de Privacidade](docs/privacy.md) · Licença MIT
