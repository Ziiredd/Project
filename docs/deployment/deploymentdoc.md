# Despliegue de modelos

## Infraestructura

- **Nombre del modelo:** Predicción series de tiempo con red neuronal recurrente lstm
- **Plataforma de despliegue:** El modelo será desplegado en un servidor local usando ngrok como método de apretura de puertos.
- **Requisitos técnicos:**
  - versión de Python: python 3.11.3
  - Librerias: fastapi(0.98.0), json(2.0.9), numpy(1.24.3), tensorflow(2.12.0),  sys.
  - Software: Linux base OS (Manjaro Linux X86_64), kernel 6.1.31-MANJARO
  - Hardware: CPU: AMD Ryzen 5 5600X (12) @ 4.200GHz, GPU: NVIDIA GeForce RTX 3060, RAM: 31976 MiB
- **Requisitos de seguridad:** No es necesario la autenticación ni la encriptación de los datos.
- **Diagrama de arquitectura:**
![image](https://github.com/Ziiredd/Project/assets/116692880/158bc700-9c15-4643-a70d-ef57822ee248)


## Código de despliegue

- **Archivo principal:** La aplicación diseñada está en el archivo deploymentAPIs.py
- **Rutas de acceso a los archivos:** El código puede encontrarse en 'src/nombre_paquete/deployment/deploymentAPIs.py'

## Documentación del despliegue

- **Instrucciones de instalación:** Debe considerar la instalación de los paquetes pip asociados a librerías mencionadas.
- **Instrucciones de configuración:** La mayoría de hiperparametros del modelo han sido explorados previamente y por consiguiente no se recomienda ninguna modificación sobre estos.
- **Instrucciones de uso:** Para poder tener acceso a nuestro servicio desde cualquier punto debemos abrir el 8000, no obstante esto se encuentran normalmente restringidos por nuestro operado de internet, para evadir dichas limitaciones usamos el servicio de ngrok. - ./Project/src/nombre_paquete/preprocessing/ngrok http 8000

