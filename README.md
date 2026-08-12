# PHP POO — Fundamentos de Programación Orientada a Objetos en PHP

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Composer](https://img.shields.io/badge/Composer-885630?style=for-the-badge&logo=composer&logoColor=white)
![PSR-4](https://img.shields.io/badge/PSR--4-009688?style=for-the-badge&logo=php&logoColor=white)
![License](https://img.shields.io/badge/Licencia-MIT-green?style=for-the-badge)

> **Base de práctica para aprender POO en PHP: autoloading PSR-4 listo para escribir clases, herencia, interfaces y composición.**

Proyecto base de **Programación Orientada a Objetos en PHP** con autoloading **PSR-4** configurado. El namespace `App\` está mapeado a la carpeta `src/` — crea tus clases y empieza a practicar sin configuración adicional.

## ✨ Características

- **Autoloading PSR-4** — `App\` → `src/`, sin `require` manuales
- **Composer listo** — `composer.json` con autoload y metadatos del autor
- **Base limpia** — estructura mínima para centrarse en el código
- **Ideal para cursos y ejercicios** — clases, herencia, interfaces, traits y composición

## 🛠 Stack

| Capa | Tecnología |
|---|---|
| Lenguaje | PHP |
| Gestión de dependencias | Composer |
| Autoloading | PSR-4 (`App\` → `src/`) |

## 🚀 Inicio rápido

```bash
composer install        # genera vendor/autoload.php
```

Escribe tu primera clase en `src/`:

```php
<?php
namespace App;

class Usuario
{
    public function __construct(
        private string $nombre,
    ) {}

    public function nombre(): string
    {
        return $this->nombre;
    }
}
```

Y úsala:

```php
<?php
require 'vendor/autoload.php';

use App\Usuario;

$usuario = new Usuario('Ana');
echo $usuario->nombre(); // Ana
```

## 📁 Estructura

```
phppoo/
├── composer.json         # Autoload PSR-4: "App\\": "src/"
└── src/                  # Tus clases (namespace App)
```

## 🧠 Conceptos para practicar

- Clases y objetos, constructores y propiedades con promoción
- Encapsulamiento (public / private / protected) y métodos
- Herencia, clases abstractas e interfaces
- Traits y composición
- Namespaces y autoloading

<!-- Agrega capturas en docs/screenshots/ -->

---

## Desarrollado por Francisco Javier Laguna

Full-stack developer · React · Vue · .NET · PHP

[GitHub](https://github.com/jlaguna553) · [LinkedIn](https://www.linkedin.com/in/francisco-javier-laguna-mondrag%C3%B3n-80a798154/) · [CV Online](https://cv-online.jlaguna553.workers.dev/v/xrdcnyej)
