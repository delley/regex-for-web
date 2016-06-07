# regex-for-web

Expressões regulares testadas no site http://regexr.com/

## Lista de Expressões de raspagem(scraping) em HTML

**Recupera conteúdo das propriedades `HREF` e `SRC`:**
```txt
(?:href|src|HREF|SRC)=(?:"|')(.+?)(?:"|')
```

**Recupera os cabeçalhos HTML representados pelas tags `<h1>,<h2>,<h3>,<h4>,<h5>,<h6>`:**
```txt
<(?:h|H)\d{1}.+?>(.+?)<\/(?:h|H)\d{1}>
```

```txt
	String __EVENTTARGET = "<[^>].*name=\"__EVENTTARGET\"[^>].*value=\"(.*)\"[^>].*";

	String __EVENTARGUMENT = "<[^>].*name=\"__EVENTARGUMENT\"[^>].*value=\"(.*)\"[^>].*";

	String __VIEWSTATE = "<[^>].*name=\"__VIEWSTATE\"[^>].*value=\"(.*)\"[^>].*";

	String __VIEWSTATEENCRYPTED = "<[^>].*name=\"__VIEWSTATEENCRYPTED\"[^>].*value=\"(.*)\"[^>].*";

	String __EVENTVALIDATION = "<[^>].*name=\"__EVENTVALIDATION\"[^>].*value=\"(.*)\"[^>].*";

	String CONTEUDO_BTN_CONSULTAR_PROCESSO = "<[^>].*name=\"ctl00\\$conteudo\\$btnConsultarProcesso\"[^>].*value=\"(.*)\"[^>].*";

	String CLEAR_TAGS = "<[^<]+?>";

	String EVENTOS_CONTENT_PASSO_1 = "<td>\\W*\\d+\\s-\\s\\w.*\\W*</td><td[^>].*>\\W+\\d{2}/\\d{2}/\\d{4}\\W.*</td>";

	String EVENTOS_CONTENT_PASSO_2 = "(\\W.*?(\\d+)\\s-\\s(\\w.*?)\\W.*?(\\d{2}/\\d{2}/\\d{4})\\W.*?)+?";

	String EVENTOS_CONTENT_PASSO_3 = "(\\d+)\\s-\\s(.*?)(\\d{2}/\\d{2}/\\d{4})";
	
	String LABEL_TIPO_REQUERIMENTO = "<span.*lblTipoRequerimento[^<>]>([^<>]*)</[ ]?span>";
	
	String LABEL_FASE_ATUAL = "<span.*lblTipoFase[^<>]>([^<>]*)</[ ]?span>";
	
	String LABEL_ATIVO = "<span.*lblAtivo[^<>]>([^<>]*)</[ ]?span>";
	
	String LABEL_SUPERINTENDENCIA = "<span.*lblDistrito[^<>]>([^<>]*)/([^<>]*)</span>";
	
	String LABEL_UNIDADE_PROTOCOLIZADORA = "<span.*lblUnidadeProtocolizadora[^<>]>([^<>]*)</span>";
	
	String LABEL_DATA_PROTOCOLO = "<span.*lblDataProtocolo[^<>]>([^<>]*)</span>";
	
	String LABEL_DATA_PRIORIDADE = "<span.*lblDataPrioridade[^<>]>([^<>]*)</span>";
	
	String LABEL_NUMERO_PROCESSO_CADASTRO_EMPRESA = "<span.*lblNumeroProcessoCadastroEmpresa[^<>]>([^<>]*)</span>";
	
	String EXTRACT_TD = "<td[^<>]*>([^<>]*)</td>";
	
	String TABLE_PESSOAS_RELACIONADAS = "<table[^<>]*gridPessoas[^<>]*>(.*?)</table>";
	
	String TABLE_TITULOS = "<table[^<>]*gridTitulos[^<>]*>(.*?)</table>";
	
	String TABLE_SUBSTANCIAS = "<table[^<>]*gridSubstancias[^<>]*>(.*?)</table>";
	
	String TABLE_MUNICIPIOS = "<table[^<>]*gridMunicipios[^<>]*>(.*?)</table>";
```
