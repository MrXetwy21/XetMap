# XetMap

XetMap es una librería de Python diseñada para trabajar con direcciones reales seleccionadas a partir de conjuntos de datos públicos, verificadas mediante servicios de geocodificación como la API de Google Maps. Su propósito es ofrecer datos de direcciones auténticas que se resuelven correctamente al ser geocodificadas, lo que resulta útil para pruebas, simulaciones o demostraciones que requieran ubicaciones verídicas sin comprometer datos personales.

Además de direcciones reales, XetMap también genera datos aleatorios complementarios como nombres, números de teléfono, direcciones de correo electrónico y otros detalles típicos de perfiles, permitiendo crear conjuntos de datos más completos y realistas para entornos de desarrollo o pruebas de sistemas que manejen información personal ficticia pero coherente.

## Instalación

Puedes instalar XetMap usando pip:

```sh
pip install XetMap
```

## Uso

```python
from XetMap import XMap

# Cargar una dirección 
XMap.LoadMap()

# Obtener diferentes datos de la dirección actual
print(XMap.GetMap('address1'))   # Dirección principal
print(XMap.GetMap('city'))       # Ciudad
print(XMap.GetMap('state'))      # Estado
print(XMap.GetMap('PostalCode')) # Código postal
print(XMap.GetMap('Phone'))      # Teléfono 
print(XMap.GetMap('User'))       # Usuario 
print(XMap.GetMap('Mail'))       # Correo 
print(XMap.GetMap('Pass'))       # Contraseña 
print(XMap.GetMap('Fname'))      # Nombre 
print(XMap.GetMap('Lname'))      # Apellido 
```

## Estructura del Proyecto

```
XetMap/
    __init__.py
    Func.py
    data/
        usa.json
README.md
setup.py
```

- `Func.py`: Lógica principal de la clase `XMap`.
- `data/usa.json`: Dataset de direcciones de EE.UU.
- `setup.py`: Script de instalación.
- `README.md`: Este archivo.

## Requisitos

- Python >= 3.10
- [names](https://pypi.org/project/names/)
- Json

## Licencia

MIT

---

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

# XetMap (English)

XetMap is a Python library designed to work with real-world addresses selected from public datasets, verified using geocoding services such as the Google Maps API. Its purpose is to provide authentic address data that resolves correctly when geocoded, making it ideal for testing, simulations, or demonstrations that require realistic locations without compromising personal information.

In addition to real addresses, XetMap also generates complementary random data such as names, phone numbers, email addresses, and other typical profile details—allowing you to create richer, more realistic datasets for development or testing environments involving fictitious but coherent personal information.

## Installation

You can install XetMap using pip:

```sh
pip install XetMap
```

## Usage

```python
from XetMap import XMap

# Load a random address
XMap.LoadMap()

# Get different data from the current address
print(XMap.GetMap('address1'))   # Main address
print(XMap.GetMap('city'))       # City
print(XMap.GetMap('state'))      # State
print(XMap.GetMap('PostalCode')) # Postal code
print(XMap.GetMap('Phone'))      # Random phone
print(XMap.GetMap('User'))       # Random user
print(XMap.GetMap('Mail'))       # Random email
print(XMap.GetMap('Pass'))       # Random password
print(XMap.GetMap('Fname'))      # Random first name
print(XMap.GetMap('Lname'))      # Random last name
```

## Project Structure

```
XetMap/
    __init__.py
    Func.py
    data/
        usa.json
README.md
setup.py
```

- `Func.py`: Main logic of the `XMap` class.
- `data/usa.json`: US address dataset.
- `setup.py`: Installation script.
- `README.md`: This file.

## Requirements

- Python >= 3.10
- [names](https://pypi.org/project/names/)
- Json

## License

MIT

---
