Biblioteca Apócrifa — versão estática sem API

Arquivos principais:
- index.html
- data/books-pt.js: contém os 96 livros/textos em português.
- data/books-en.js: preparado para receber os textos em inglês.
- data/books-es.js: preparado para receber os textos em espanhol.

O que mudou:
- Não existe mais chamada para Claude, GPT, Gemini ou qualquer API externa.
- Não precisa configurar API key na Vercel.
- A página funciona como entrega digital estática.
- PT está completo.
- EN e ES ficam desativados até que os arquivos books-en.js e books-es.js sejam preenchidos.

Como adicionar uma tradução:
1. Copie a estrutura de data/books-pt.js.
2. Cole em data/books-en.js ou data/books-es.js.
3. Troque apenas textos visíveis: name, desc, chapterLabels, chapterNavLabels e text.
4. Mantenha os mesmos IDs dos livros e as mesmas chaves dos capítulos/partes.
5. Ao salvar, a interface libera automaticamente o botão do idioma.

Deploy na Vercel:
- Suba a pasta inteira para a Vercel.
- Não configure ANTHROPIC_API_KEY, OPENAI_API_KEY ou outras chaves.
