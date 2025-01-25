# Firebase User Management

## **Overview**
Este proyecto proporciona herramientas administrativas para gestionar datos en Firebase que no se pueden modificar directamente desde la consola. Esto incluye tareas como la actualización de correos electrónicos de usuarios y la sincronización de datos entre Firebase Authentication y Firestore.

Está diseñado para facilitar la manipulación de datos críticos que requieren lógica avanzada y no pueden resolverse manualmente.

---

## **Core Features**
- **Gestión de usuarios en Firebase Authentication:**
  - Actualización de correos electrónicos.
  - Eliminación y creación de usuarios específicos.

- **Sincronización con Firestore:**
  - Actualización de datos relacionados con los usuarios.

- **Integración con Firebase Admin SDK:**
  - Interacciones avanzadas con Firebase Authentication y Firestore.

---

## **Project Structure**
El proyecto sigue una estructura modular para facilitar su mantenimiento y escalabilidad:

firebase-user-management/
├── scripts/                   # Scripts para tareas específicas
│   ├── updateEmail.js         # Actualiza correos electrónicos de usuarios
├── utils/                     # Funciones reutilizables
│   ├── firebaseAdmin.js       # Inicialización del Firebase Admin SDK
│   └── logging.js             # Funciones de logging para depuración
├── config/                    # Archivos de configuración
│   └── serviceAccountKey.json # Credenciales del Admin SDK
├── package.json               # Dependencias del proyecto
├── .gitignore                 # Archivos ignorados por Git
├── README.md                  # Documentación del proyecto
└── tsconfig.json              # Configuración de TypeScript (si aplica)

Getting Started

Prerequisites

Node.js: Instala la última versión desde nodejs.org.
Firebase CLI: Instala la Firebase CLI globalmente:

npm install -g firebase-tools

Credenciales de Firebase Admin SDK: Descarga el archivo serviceAccountKey.json desde la consola de Firebase:
Ve a Configuración del proyecto > Cuentas de servicio.

Genera una nueva clave privada y guárdala en config/serviceAccountKey.json.


Clona este repositorio:

git clone https://github.com/yourusername/firebase-user-management.git

cd firebase-user-management

Instala las dependencias del proyecto:

npm install
Configura las variables de entorno:

Crea un archivo .env en el directorio raíz con las siguientes variables:

FIREBASE_CONFIG=your_firebase_config
Running the Application
Para ejecutar los scripts, utiliza node.

Ejemplo: Actualizar correo electrónico

node scripts/updateEmail.js
Scripts disponibles

1. Actualizar correo electrónico
updateEmail.js: Cambia el correo electrónico de un usuario específico en Firebase Authentication.

Built With

Firebase Admin SDK: Para la gestión avanzada de usuarios y bases de datos en Firebase.
Node.js: Entorno de ejecución para el backend.

TypeScript (opcional): Para tipado estático y mayor robustez del código.

Contributing

Contribuciones son bienvenidas. Sigue estos pasos para colaborar:

Haz un fork del repositorio.

Crea una nueva rama para tu funcionalidad:

git checkout -b feature/NuevaFuncionalidad
Realiza tus cambios y haz commits:

git commit -m "Descripción de los cambios"
Haz un push de tus cambios:

git push origin feature/NuevaFuncionalidad

Abre un Pull Request.

License

Distribuido bajo la licencia MIT. Consulta el archivo LICENSE para más información.
