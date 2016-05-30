# regex-for-web-example

Expressões regulares testadas no site http://regexr.com/

## Listas de Expressões de crawling de HTML

**Recupera conteúdo das propriedades `HREF` e `SRC`:**
```txt
(?:href|src|HREF|SRC)=(?:"|')(.+?)(?:"|')
```
