# Automatización de Testing Web - SauceDemo

## Descripción del Proyecto

Este proyecto fue desarrollado como pre-entrega del curso de automatización de pruebas, con el objetivo de aplicar los conocimientos adquiridos hasta la Clase 8.

La automatización fue realizada sobre **:contentReference[oaicite:0]{index=0} SauceDemo**, una plataforma web creada para practicar testing funcional.

El proyecto automatiza flujos básicos de navegación e interacción con productos utilizando Selenium WebDriver y Python.

Las funcionalidades implementadas incluyen:

- Inicio de sesión en la aplicación.
- Navegación al catálogo de productos.
- Validación del catálogo.
- Obtención de información de productos.
- Agregado de productos al carrito.
- Validación del producto agregado.

---

## Objetivo del Proyecto

Aplicar conceptos de automatización web, localización de elementos, interacción con interfaces y validaciones funcionales utilizando buenas prácticas de testing.

---

## Tecnologías Utilizadas

- **Python** → Lenguaje principal.
- **:contentReference[oaicite:1]{index=1} Pytest** → Framework para ejecutar y organizar pruebas.
- **:contentReference[oaicite:2]{index=2} Selenium WebDriver** → Automatización de pruebas web.
- **:contentReference[oaicite:3]{index=3} Git** → Control de versiones.
- **:contentReference[oaicite:4]{index=4} GitHub** → Almacenamiento del repositorio.

Sitio web utilizado:

https://www.saucedemo.com

---

## Estructura del Proyecto

```bash
Nemeth-Rocio-PreEntrega/
│
├── tests/
│   └── test_saucedemo.py
│
├── utils/
│   └── helpers.py
│
├── conftest.py
├── requirements.txt
└── README.md
```

### Descripción de archivos

### test_saucedemo.py
Contiene los casos de prueba automatizados.

### helpers.py
Contiene funciones auxiliares reutilizables, como el proceso de login.

### conftest.py
Contiene la configuración de Pytest y fixtures.

---

## Instalación del Proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/rocionemeth/Nemeth-Rocio-PreEntrega.git
cd Nemeth-Rocio-PreEntrega
```

### 2. Crear entorno virtual (opcional)

En Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

En Mac/Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Instalar dependencias

```bash
pip install -r requirements.txt
```

O instalar manualmente:

```bash
pip install selenium pytest pytest-html
```

---

## Cómo Ejecutar las Pruebas

### Ejecutar todos los tests

```bash
pytest -v
```

### Ejecutar con reporte HTML

```bash
pytest -v --html=reporte.html
```

---

## Casos de Prueba Implementados

## 1. Navegación y Validación del Catálogo

Este test verifica:

✔ Login exitoso  
✔ Título correcto de la página de inventario  
✔ Presencia de productos visibles  
✔ Obtención del nombre y precio del primer producto  

---

## 2. Interacción con Productos

Este test verifica:

✔ Agregado del primer producto al carrito  
✔ Actualización del contador del carrito  
✔ Navegación al carrito  
✔ Validación del producto agregado  

---

## Autor

Proyecto desarrollado por Rocío Nemeth como práctica de automatización QA con Python, Selenium y Pytest.