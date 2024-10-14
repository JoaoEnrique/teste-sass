# Teste com SASS

style.scss
```scss
@import './variaveis';
@import './_header'; 

*{
    padding: 0;
    margin: 0;
    font-family: sans-serif;
    box-sizing: border-box;
}

main{
    @include flexCenter(0 100px);
    @extend *;
    margin-top: 40px;
}
```

_variaveis.scss
```scss
$principal: #5bb4ff;
$nome: "Mundo";
```

_header.scss
```scss
@mixin flexCenter($padding){
    display: flex;
    flex-direction: column;
    padding: $padding;
}

header{
    @include flexCenter(100px);
    background: $principal;
    color: #fff;
    transition: 0.3s;

    h1{
        text-align: center;

        &::after{
            content: " " + $nome;
        }
    }

    p{
        font-size: 20px;
    }

    &:hover{
        color: #000;
        background-color: #fff;
    }
}
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello World</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <h1>Olá</h1>
    </header>

    <main>
        <p>Aula de SASS</p>
    </main>
</body>
</html>
```