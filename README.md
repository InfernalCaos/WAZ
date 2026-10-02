<p align="center"><img src="extension/icons/logo.png" width="220" alt="WAZ" style="background:#000;padding:20px;border-radius:16px"></p>

# WAZ · Glass

Wallpapers animados em loop na **Nova Guia** do Chrome, com busca em vidro, atalhos, relógio e cores personalizáveis.

## Recursos
- Vídeo (MP4/WebM), GIF e imagem como wallpaper, em loop e com transição suave
- Galeria de wallpapers, com troca automática opcional
- Busca em vidro que brilha com a cor do vídeo (ou a cor que você escolher)
- Relógio opcional com fonte do computador ou enviada por você
- 100% local: nenhum dado sai do seu navegador

## Instalar (fácil)
1. Abra a aba **[Releases](../../releases/latest)** e baixe o arquivo **WAZ-chrome-store.zip**.
2. Clique com o botão direito no zip e escolha **Extrair tudo**.
3. Abra `chrome://extensions` e ative o **Modo do desenvolvedor**.
4. Clique em **Carregar sem compactação** e selecione a pasta extraída (a que contém o `manifest.json`).
5. Abra uma nova aba.

> Se baixar pelo botão verde **Code > Download ZIP**, extraia e selecione a pasta `extension/`.

## Estrutura
```
extension/   código da extensão (manifest, html, css, js, ícones)
docs/        termos de uso e política de privacidade (GitHub Pages)
store/       textos e checklist para a Chrome Web Store
scripts/     build.sh gera o .zip para enviar à loja
```

## Gerar o pacote da loja
```bash
bash scripts/build.sh   # cria dist/WAZ-chrome-store.zip
```

## Limitações
O Chrome não permite que extensões alterem a barra de abas/endereço, apenas a Nova Guia. O rodapé "Personalizar o Chrome" é nativo e pode ser ocultado pelo usuário (clique direito no rodapé).

[Termos de Uso](docs/terms.md) · [Política de Privacidade](docs/privacy.md) · Licença MIT
