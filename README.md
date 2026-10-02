# Sistema de Gestión de Cuentas Bancarias (Java y Swing)

## Descripción
Aplicación de escritorio desarrollada en Java con interfaz gráfica mediante Swing, diseñada para simular la administración y transacciones de cuentas bancarias. El proyecto aplica principios fundamentales de la Programación Orientada a Objetos (POO), como herencia, encapsulamiento y polimorfismo, para estructurar diferentes productos financieros.

## Objetivo
Proporcionar una herramienta para gestionar operaciones bancarias esenciales, tales como registro de titulares, depósitos, retiros, consulta de saldo y cálculo automático de intereses para Cuentas de Ahorro y Cuentas de Crédito, validando reglas de negocio en cada operación.

## Estructura de clases
- **Cuenta (Clase base):** Contiene los datos del titular y el saldo. Define los métodos para depósitos y retiros con control parametrizado sujeto a la disponibilidad de fondos.
- **Ahorro (Subclase):** Aplica una tasa de interés predefinida para calcular el incremento del saldo acumulado.
- **Crédito (Subclase):** Incorpora líneas de crédito parametrizadas y sobrescribe el método de retiro para evaluar la disponibilidad de crédito del usuario.

## Habilidades y conceptos aplicados
- **Programación Orientada a Objetos:** Diseño de clases, encapsulamiento de datos y modelado de relaciones jerárquicas mediante herencia.
- **Desarrollo de Interfaces Gráficas (GUI):** Construcción de vistas interactivas utilizando `javax.swing` y gestión de eventos de usuario.
- **Lógica de negocio:** Implementación de validaciones de saldo, cálculo de tasas financieras y flujos de control para transacciones de depósitos y retiros.
