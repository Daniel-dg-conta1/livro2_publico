# Enhanced Teoria da Usinagem Site

Conteúdo:
- `index.html` — versão do seu site com visualizador de PDF (pdf.js) e pipeline de extração de texto (Tesseract.js).
- Instruções para integrar ao seu repositório GitHub.

## Como usar
1. Baixe este diretório e substitua o `index.html` do seu projeto (ou coloque numa nova branch).
2. Para abrir localmente, basta servir o arquivo com um servidor simples:
   - Python 3: `python -m http.server 8000` (no diretório do arquivo) e abra `http://localhost:8000`.
3. Para importar o PDF do livro, use o botão "Importar Livro (PDF)" e selecione `livro2.pdf` localmente.
4. Após carregar o PDF, clique em "Extrair Texto" para o app tentar estruturar capítulos automaticamente. Se for scan, o OCR rodará no navegador (pode ser lento).
5. Para produção, recomendo executar OCR server-side e gerar `chapters.json` com o conteúdo limpo; depois substitua o array `db.chapters` por esse JSON.

## Nota sobre o GitHub repo
- Eu tentei acessar o repositório que você indicou, mas não consegui (404). Se quiser que eu abra um PR diretamente, me torne colaborador ou torne o repositório público e forneça o link correto.

## Quer que eu faça isso por você?
- Posso:
  1) Extrair o texto do PDF servidor-side e gerar `chapters.json` pronto.
  2) Criar um branch com os arquivos e abrir um PR (preciso de acesso ao repo).
  3) Melhorar a heurística de divisão de capítulos se me enviar amostras do índice do livro.

Responda qual opção prefere (1, 2 ou 3) ou faça o merge manual substituindo o `index.html`.

