
## ejercicio

## HTML

Define un formulario con campos de entrada para la base y la altura del rectángulo.
Incluye un botón para realizar el cálculo y un párrafo para mostrar el resultado.

## JavaScript:

La función 'calcular()' obtiene los valores de la base y la altura del rectángulo.
Valida que los valores sean números válidos.
Calcula el área y el perímetro del rectángulo.
Muestra el resultado en el párrafo 'resultado'.

## Características:

Validación de entrada.
Formato de salida con dos decimales.
Mensajes de error.

Este código se puede usar para calcular el área y el perímetro de otros rectángulos, o para realizar otras operaciones matemáticas con números.

````Javascript
 function calcular() {
      const baseInput = document.getElementById('base');
      const alturaInput = document.getElementById('altura');
      const base = parseFloat(baseInput.value);
      const altura = parseFloat(alturaInput.value);

      if (isNaN(base) || isNaN(altura)) {
        alert('Ingrese valores numéricos válidos para la base y la altura.');
        return;
      }

      const area = base * altura;
      const perimetro = 2 * (base + altura);

      const resultadoP = document.getElementById('resultado');
      resultadoP.textContent = `El área del rectángulo es: ${area.toFixed(2)} y el perímetro es: ${perimetro.toFixed(2)}`;
    }
```