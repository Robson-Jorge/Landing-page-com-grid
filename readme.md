# DevQuest - Landing page com grid

Este é um exercício focado em display grid para ajudar a melhorar suas habilidades de codificação criando projetos realistas.

## Índice

- Visão geral
	- Captura de tela
- Meu-processo
	- Construído com
	- O-que-aprendi
- Autor 
- Agradecimentos

## Visão geral 

### Captura de tela 

![](./src/design/gif-landing-page.gif)

## Meu processo

### Construído com

- Marcação HTML5 semântica
- Propriedades personalizadas CSS
- Flexbox
- CSS Grid

### O que aprendi

Nesse projeto recordei sobre a utilização de alguns recursos em formas diferentes do que uso com mais frequência.
Aprendi como usar e estilizar da melhor forma um menu do tipo hambúrguer para responsividade em telas menores, o que já fica como aprendizado para utilização em outras oportunidades e formas.
Também aprendi formas de animação com o css, apenas usando o rotate em alguns elementos e outra forma com a tag animation.

```html
    <input type="checkbox" id="menu-hamburguer">
    <label for="menu-hamburguer">
        <div class="menu">
            <span class="hamburguer"></span>
        </div>
    </label>
```
```css
.header input:checked ~ label .hamburguer{
    transform: rotate(45deg);
}
.header input:checked ~ label .hamburguer:before{
    transform: rotate(90deg);
    top: 0;
}
.header input:checked ~ label .hamburguer:after{
    transform: rotate(90deg);
    bottom: 0;
}
```
```css
.hero::after{
    content: url(../images/seta_preta.png);
    position: absolute;
    height: 35px;
    bottom: 40px;
    animation: downarrow 0.6s infinite alternate ease-in-out;
}
@-webkit-keyframes downarrow{
    0%{ -webkit-transform: translateY(0) ; opacity: 0.4;}
    100%{ -webkit-transform: translateY(0.4em) ; opacity: 0.9;}
}
```

## Autor

- Frontend Mentor - [@Robson-Jorge](https://www.frontendmentor.io/profile/Robson-Jorge)
- Linkedin - [@Robson-Jorge](https://www.linkedin.com/in/robson-jorge-62a12a26a/)

## Agradecimentos

Agradeço ao curso DevQuest, aos meus professores e as monitorias que me deram uma capacitação para desenvolver um projeto como esse.
