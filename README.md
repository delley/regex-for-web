# regex-for-web

Expressões regulares testadas no site http://regexr.com/

## Listas de Expressões de raspagem(scraping) em HTML

**Recupera conteúdo das propriedades `HREF` e `SRC`:**
```txt
(?:href|src|HREF|SRC)=(?:"|')(.+?)(?:"|')
```

**Recupera os cabeçalhos HTML representados pelas tags `<h1>,<h2>,<h3>,<h4>,<h5>`:**
```txt
<(?:h|H)\d{1}.+?>(.+?)<\/(?:h|H)\d{1}>
```
