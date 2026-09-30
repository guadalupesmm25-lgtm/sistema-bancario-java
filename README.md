# Sistema de Gestión de Cuentas Bancarias (Java & Swing)

## 📝 Descripción
Aplicación de escritorio desarrollada en **Java** con interfaz gráfica de usuario (**Swing**), diseñada para simular la administración y operaciones operativas de cuentas bancarias. El proyecto implementa los pilares fundamentales de la Programación Orientada a Objetos (POO) —como herencia, encapsulamiento y polimorfismo— para modelar diferentes tipos de productos financieros.

## 🎯 Objetivo Principal
Proporcionar una herramienta interactiva que permita a los usuarios gestionar operaciones bancarias esenciales (registro de titulares, depósitos, retiros, consulta de saldo y cálculo automatizado de intereses) para **Cuentas de Ahorro** y **Cuentas de Crédito**, garantizando la validación de reglas de negocio en cada transacción.

## 🏗️ Arquitectura y Estructura de Clases
El sistema utiliza una estructura jerárquica de clases para garantizar la reutilización de código y la extensibilidad:

- **`Cuenta` (Clase Base):**
  - **Atributos:** `nombre` (titular) y `saldo`.
  - **Métodos:** `deposito(Double cantidad)`, `retiro(Double cantidad)`.
  - **Regla de negocio:** Control de retiros parametrizados (hasta $1,000 por transacción) sujeto a disponibilidad de saldo.

- **`Ahorro` (Hereda de `Cuenta`):**
  - **Atributo estático:** Tasa de interés (`tasa = 0.1` / 10%).
  - **Métodos:** `interes()`, incrementa el saldo acumulado aplicando la tasa correspondiente.

- **`Crédito` (Hereda de `Cuenta`):**
  - **Atributos:** Tasa de interés (`tasai = 0.2` / 20%) y `limite` de línea crediticia.
  - **Métodos:** `interes()` para aplicación de cargos/intereses y sobrecarga de `retiro(Double cantidad, Double limite)` para evaluación de disponibilidad en línea de crédito.

## 🛠️ Competencias Adquiridas
- **Programación Orientada a Objetos (POO):** Modelado de jerarquías mediante herencia, encapsulamiento de atributos y diseño de clases.
- **Desarrollo de Interfaces Gráficas (GUI):** Construcción de entornos interactivos orientados al usuario con el paquete `javax.swing` y manejo de eventos (`ActionListener`).
- **Lógica de Negocio y Simulación Financiera:** Implementación de flujos de control para validación de fondos, depósitos, retiros y cálculo de tasas de interés activas y pasivas.
- **Diseño de Software de Escritorio:** Estructuración limpia de código enfocado en mantenibilidad y componentes gráficos responsivos.

