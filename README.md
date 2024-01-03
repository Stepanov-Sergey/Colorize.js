<style>
r { color: Red }
o { color: Orange }
g { color: Green }
</style>


English:
The script defines a Colorize class with methods for applying foreground and background colors to text in the terminal. It includes a set of predefined colors for both foreground and background. Additionally, it provides a checkColor method to verify if a specified color is defined.

Русский:
Скрипт определяет класс Colorize с методами для применения цветов переднего и заднего плана к тексту в терминале. Он содержит набор предопределенных цветов как для переднего, так и для заднего плана. Кроме того, скрипт предоставляет метод checkColor для проверки, определен ли указанный цвет.

```bash
node app.js


const Colorize  = require('./colorize.js');
console.log(Colorize.bg.green(`This text is green background color.`));<br>
Colorize.checkColor('red', 'fg');<br>
Colorize.checkColor('blue', 'bg');<br>
Colorize.checkColor('purple', 'fg');<br>


Output
<r>This text is green background color.</r>
Background color 'blue' is not defined.
Foreground color 'purple' is not defined.
