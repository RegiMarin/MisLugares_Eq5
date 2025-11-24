# MisLugares_Eq5
Aplicación móvil Android para la gestión personal de lugares de interés.

## Descripción del proyecto

**Mis Lugares** es una aplicación móvil diseñada para registrar, organizar y consultar puntos de interés personales. Resuelve la dispersión de información permitiendo guardar la ubicación, datos de contacto, notas y contenido multimedia, todo en un solo lugar.

### La aplicación permite:
- Guardar información clave: nombre, categoría, dirección, contacto, sitio web y comentarios.
- Adjuntar fotografías y asignar una valoración numérica.
- Realizar acciones como visualizar la ubicación en mapas, hacer llamadas o abrir sitios web.

### Propósito del proyecto
Tiene un propósito **funcional** y **académico**:
- Proveer una herramienta útil para administrar lugares personales.
- Servir como práctica de aprendizaje para:
  - Interfaces de usuario (UI)
  - Activities y Fragments
  - Intents (Cámara, Maps, Teléfono, Web)
  - Persistencia de datos
  - Arquitectura por capas en Android


##  Requisitos e instalación

### Requisitos previos
- Android Studio actualizado
- Android SDK
- Emulador o dispositivo físico Android
- Google Play Services (para mapas)

### Instalación
1. Clonar el repositorio:
   ```bash
   git clone https://github.com/RegiMarin/MisLugares_Eq5.git
   cd MisLugares_Eq5
   ```
2. Abrir Android Studio → **Open an Existing Project**  
3. Esperar la sincronización de Gradle  
4. Configurar un emulador o conectar un dispositivo físico  
5. Ejecutar con **Run ▶**  


### Cómo usarlo

Para realizar la ejecución del proyecto se requieren seguir lo siguientes pasos:   

- Descargar el proyecto. 
- Abrir Android Studio e ir a la opción para abrir un proyecto. 
- Seleccionar el proyecto respectivo de “mis lugares”. 
- Esperar las sincronizaciones necesarias que requiere hacer Android Studio. 
- Conectar el dispositivo físico o hacer uso del emulador. 
- Ejecutar el proyecto 


## Estructura del proyecto

El proyecto sigue una arquitectura por capas.

```
/casos_uso        → Acciones principales: mapas, llamadas, permisos, navegación
/datos            → Repositorio, CRUD, filtrado, carga y guardado
/modelo           → Clases de datos: Lugar, GeoPunto, TipoLugar
/presentacion     → Activities, Fragments, AdapterLugares, vistas UI


## Contribuciones

### ¿Cómo contribuir al proyecto?

1. **Fork del repositorio**  
   https://github.com/RegiMarin/MisLugares_Eq5

2. **Clonar tu fork**
   ```bash
   git clone https://github.com/<tu-usuario>/MisLugares_Eq5.git
   cd MisLugares_Eq5
   ```

3. **Crear una rama**
   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```

4. **Hacer cambios** siguiendo la estructura:
   ```
   casos_uso/
   datos/
   modelo/
   presentacion/
   ```

5. **Probar la app** ejecutándola en emulador o dispositivo.

6. **Subir cambios**
   ```bash
   git add .
   git commit -m "Agrega [descripción breve de la mejora]"
   git push origin feature/nueva-funcionalidad
   ```

7. **Crear un Pull Request** hacia el repo original  
   Describir claramente qué se modificó y por qué.

---

## 📘 Resumen técnico del sistema

En resumen, el proyecto Mis Lugares desarrollado es una aplicación Android desarrollada en Kotlin y java utilizando Android Studio y las librerías estándar del SDK. Tiene integrado Google Maps mediante Google Play Services para mostrar ubicaciones en un mapa, tambien para registrar nuevos puntos marcados por el usuario. La arquitectura del proyecto sigue el modelo básico de una Activity principal que gestiona el ciclo de vida de la interfaz y coordina la comunicación con los servicios de mapas. No se hizo uso de backend ni servidor, todo el funcionamiento ocurre de forma local en el dispositivo. La app está diseñada para ser ligera, fácil de compilar y totalmente compatible con dispositivos Android desde versiones recientes del SDK. 
---

## FAQ
**1. ¿Necesito una API Key de Google Maps para ejecutar el proyecto?**
Sí, es necesario agregar tu propia Google Maps API Key en el archivo correspondiente para que el mapa funcione correctamente. 

**2. ¿Puedo ejecutar la app sin un dispositivo físico?**
Sí, siempre y cuando utilices un emulador de Android que tenga los servicios de Google Play instalados. 

**3. ¿La aplicación guarda los lugares de forma permanente?** 
En esta versión, los lugares se manejan de manera local, por lo que aunque no se utilice una base de datos, los lugares quedan guardados dentro de la aplicación. 

**4. ¿Puedo agregar nuevas funciones al proyecto?** 
Sí, aunque el proyecto ya cuente con el funcionamiento básico esperado, se pueden implementar mejoras. 

**5. ¿Necesito instalar dependencias externas?** 
No, solo se utilizan componentes incluidos en Android SDK y Google Play Services. 
