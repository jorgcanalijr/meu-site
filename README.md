````markdown name=README.md
```markdown
# Rei das 2 Rodas — assets + index.html

O que está aqui:
- index.html — página pronta com 25 cards (títulos já preenchidos).
- convert-images.sh — script que gera versões 600/1200/1920 em JPG + WebP.
- Instruções rápidas abaixo.

Passos para usar (rápido):
1. Crie a pasta `assets/originals/` no mesmo diretório do `index.html`.
2. Coloque as 25 imagens originais nessa pasta com nomes:
   - moto-1.jpg
   - moto-2.jpg
   - ...
   - moto-25.jpg
   (Se suas imagens forem .png, mantenha a extensão .png — o script aceita .jpg/.jpeg/.png.)
3. Instale dependências:
   - macOS: `brew install imagemagick webp`
   - Ubuntu/Debian: `sudo apt install imagemagick webp`
4. Rode o script:
   - `bash convert-images.sh`
   - O script criará `assets/images/motos/` com:
     - moto-N-600.jpg, moto-N-1200.jpg, moto-N-1920.jpg
     - moto-N-600.webp, moto-N-1200.webp, moto-N-1920.webp
5. Abra localmente para testar:
   - `python -m http.server 8000`
   - Abra http://localhost:8000

Observações importantes:
- Nenhum preço é mostrado no HTML. O botão "Solicitar Info" abre WhatsApp com mensagem pré-preenchida.
- Se quiser títulos/categorias diferentes, edite o array `bikes` no `index.html`.
- Se quiser que eu faça o commit no seu repositório GitHub, me passe `owner/repo` e `branch` e eu preparo o commit para você (não preciso da sua senha). Você pode também me autorizar a subir as imagens originais que você enviou na conversa; eu cuidarei do resto.
```
````
