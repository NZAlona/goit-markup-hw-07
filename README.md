# goit-markup-hw-07

This repository was created for homework 7

Selector "placeholder" in Sass:

%align { display: flex; justify-content: center; align-items: center; }

.button-base { background-color: #2a2a2a; @extend %align; }

Normally it is based in derictory Utils ---> need to create file \_placeholders.scss and put inside

%align { display: flex; justify-content: center; align-items: center; }

then replace it in scss files and @import in main.scss

Ecли одинаковые свойства и значения которые переиспользуются - используем placeholder(% @extend)

Mixin in Sass is a template with a set of properties thet can be reused. To declare mixin - @mixin
Normally it is based in derictory Utils - need to create file \_mixins.scss and put inside + @import
"./" Шаблон свойств но значения свойств можно передавать. @mixin font
($fw, $fs, $lh) { font-weight:
$fw; font-size: $fs; line-height: $lh ; }

$fs, $fw - переменные название придумываем сами .site-contacts\_\_link { @include font(
500,14px,1.14; letter-spacing: 0.02em; }

.site\_\_link { @include font(300, 12px, 1.15 ); letter-spacing: 0.03em; }

Sass - разделение кода по архитектуре.вложенность селекторов через & (амперсанд).миксины и
плейсхолдеры

Переменные - CSS в них можна записывать какие-то значения и переиспользовать эти значения с помощью
функции var(--). Sass переменные записываем через $ в папке Utils in file \_variables $accent-color:
teal; .menu { background-color: $accent-color; }
