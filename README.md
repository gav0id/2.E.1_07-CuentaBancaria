Ejercicio 2.E.1 07 - Cuenta Bancaria

Lógica del programa
Para este ejercicio, diseñé la clase `CuentaBancaria` e implementé el concepto de encapsulamiento. Para lograrlo, definí los atributos `titular` (String) y `saldo` (double) utilizando el modificador de acceso `private`, lo que protege los datos para que no puedan ser modificados directamente desde afuera de la clase.

Para interactuar con estos atributos de forma segura, generé los métodos públicos *getters* y *setters*. Además, implementé un constructor para inicializar el titular y el saldo al momento de crear la cuenta.

El comportamiento central de la clase lo definí en dos métodos:
1. `depositar(double monto)`: Incluye una validación (`if`) para asegurar que el monto ingresado sea mayor a 0 antes de sumarlo al saldo actual e imprimir el comprobante.
2. `retirar(double monto)`: Verifica si el saldo disponible es mayor o igual al monto que se desea extraer. Si hay fondos suficientes, realiza la resta; de lo contrario, bloquea la operación y muestra un mensaje de "fondo insuficiente".

Dentro del método `main`, desarrollé la siguiente lógica de prueba:
1. Instancié un objeto `CuentaBancaria` a nombre de "Benjamin" con un saldo inicial de 670.
2. Realicé un depósito válido de 30 (llevando el saldo a 700).
3. Intenté realizar una extracción de 750 para forzar la validación de fondos insuficientes y comprobar que la lógica de seguridad funciona.
4. Finalmente, utilicé el método `getSaldo()` para imprimir el saldo restante y confirmar que la extracción denegada no alteró mi dinero.

Ejecución en consola
<img width="1366" height="722" alt="imagen" src="https://github.com/user-attachments/assets/ec413df5-3827-4b6f-9557-715a64ff8432" />

