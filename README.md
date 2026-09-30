# Informe de Auditoría de Red Wi-Fi Insegura
## Parte 1 – Exploración de Tráfico Web (HTTP)

En esta primera etapa utilicé las herramientas de desarrollador del navegador (**F12**), específicamente la pestaña **Network (Red)**, para capturar e inspeccionar la primera petición realizada al cargar el sitio `http://neverssl.com`.

### Datos de la Petición

* **URL solicitada:** `http://beautifulgrandclearverse.neverssl.com/online/`
* **Método HTTP:** `GET`
* **Status Code:** `200 OK`
* **Host:** `beautifulgrandclearverse.neverssl.com`
* **Remote Address (IP y Puerto):** `34.223.124.45:80`
* **Protocolo utilizado:** `HTTP/1.1` (sin cifrado / texto plano sobre el puerto 80)

### Headers Enviados (Request Headers)

Entre las cabeceras enviadas por el navegador se destacan:
* **Host:** `beautifulgrandclearverse.neverssl.com`
* **User-Agent:** `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/154.0.0.0 Safari/537.36`
* **Accept:** `text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,...`
* **Accept-Encoding:** `gzip, deflate`
* **Accept-Language:** `es-ES,es;q=0.9,en;q=0.8`
* **Connection:** `keep-alive`
* **Upgrade-Insecure-Requests:** `1`

### Evidencia

![Inspección de Red en NeverSSL](01_Network_NeverSSL.png)
