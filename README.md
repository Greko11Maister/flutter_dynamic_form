# flutter_dynamic_form

# Ejercicio: Formulario Dinámico en Flutter

## Descripción
En este ejercicio, el desarrollador debe construir un formulario dinámico en Flutter que pueda mostrar diferentes tipos de campos en función de una lista proporcionada. El objetivo es que el formulario se adapte según la configuración que recibe, permitiendo agregar múltiples tipos de entradas (como campos de texto y botones de opción).

## Objetivo
Implementar un formulario que reciba una lista de configuraciones de campos en formato JSON.
Renderizar cada campo de forma dinámica en la interfaz.
Asegurarse de que los valores ingresados por el usuario puedan ser recuperados y procesados posteriormente.
Estructura de Datos de Entrada
La lista de configuración se proporcionará como un JSON. A continuación, un ejemplo del formato:

```
[
  { "field": "Nombre", "type": "text" },
  { "field": "Género", "type": "radio_button", "options": ["Masculino", "Femenino", "Otro"] },
  { "field": "Fecha de Nacimiento", "type": "date_picker" },
  { "field": "Recibir Notificaciones", "type": "checkbox" }
]
```

### Requerimientos

#### Campos Dinámicos:

El formulario debe interpretar los siguientes tipos de campos:

- Text: Entrada de texto.
- Radio Button: Botones de opción para seleccionar una opción.
- Date Picker: Selector de fechas.
- Checkbox: Casilla para activar o desactivar una opción.

### Validación Básica:

- Campos de texto no deben estar vacíos.
- Los botones de opción deben tener al menos una opción seleccionada.
- La fecha debe ser válida y seleccionada correctamente.

### Recuperación de Datos:

Al hacer clic en un botón de "Enviar", se deben recuperar todos los valores ingresados y mostrarlos en la consola.

```
flutter_dynamic_form/
│
├── lib/
│   ├── main.dart
│   └── widgets/
│       └── dynamic_form.dart
├── pubspec.yaml
└── README.md
```
