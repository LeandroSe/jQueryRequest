# jQueryRequest

## Introdução

Plugin jQuery para requisição Ajax facilitada, e com eventos callbacks.

Permite chamada de requisição para formulários, e chamada de requisição ao clica em elementos com o atributo ```data-request``` setada.

## Usos

### Formulários

```
$("form").request()
```

### Elementos

```
<a href="api.json" data-request>Executar</a>
```

ou

```
<button data-request="api.json"></button>
```

### Plugin

```
$.request({
    url: 'api.json',
    data: {
        user: 1,
        name: "Leandro Senni"
    },
    success: function($element, api[, me]) {},
    error: function($element, message, httpRequestCode[, me]) {},
    loading: function($element[, me]) {}
});
```
