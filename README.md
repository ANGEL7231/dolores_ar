# Dolores AR · Evidencias TDD

App turística con realidad aumentada para visitar Dolores Hidalgo desarrollada en Flutter aplicando Desarrollo Guiado por Pruebas (TDD): GPS, brújula, cámara, trigonometría, modelos 3D y pasaporte turístico.

---

## Rondas de Desarrollo (TDD)

### Ronda 0 — Preparar el taller (`Paso 0.1`)
* **Crear proyecto `dolores_ar` (`Paso 0.1`):**
  ![Crear proyecto dolores_ar](capturas/image1.png)
* **Instalar paquetes `camera`, `geolocator`, `flutter_compass` y `model_viewer_plus` (`Paso 0.1`):**
  ![Instalar paquetes](capturas/image2.png)

### Ronda 1 — ¿A qué distancia está? (Haversine)
* **🔴 Rojo — `test/ayudas_geo.dart` (`Ciclo 1.1`):**
  ![Ciclo 1.1 Rojo ayudas_geo](capturas/image3.png)
* **🔴 Rojo — `test/geo_test.dart` distancia (`Ciclo 1.1`):**
  ![Ciclo 1.1 Rojo geo_test](capturas/image4.png)
* **🟢 Verde — `distanciaMetros` (`Ciclo 1.2`):**
  ![Ciclo 1.2 Verde distanciaMetros](capturas/image5.png)


For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

[Manual_TDD_RealidadAumentada_Dolores.docx](https://github.com/user-attachments/files/34796554/Manual_TDD_RealidadAumentada_Dolores.docx)
=======
### Ronda 2 — ¿Hacia dónde queda? Rumbo y ángulos
* **🔴 Rojo — `rumboGrados` y `ángulos` (`Ciclo 2.1`):**
  ![Ciclo 2.1 Rojo rumbo y ángulos](capturas/image6.png)
* **🟢 Verde — `rumboGrados` y suavizado (`Ciclo 2.2`):**
  ![Ciclo 2.2 Verde rumbo y ángulos](capturas/image7.png)

### Ronda 3 — De ángulo a pantalla: el campo de visión y catálogo
* **🔴 Rojo — `posicionHorizontal` y `formatearDistancia` (`Ciclo 3.1`):**
  ![Ciclo 3.1 Rojo campo de visión](capturas/image8.png)
* **🟢 Verde — `posicionHorizontal` y `nombreCardinal` (`Ciclo 3.2`):**
  ![Ciclo 3.2 Verde campo de visión](capturas/image9.png)
* **🟢 Verde — `lugar.dart` y `catalogo.dart` (`Ciclo 3.3`):**
  ![Ciclo 3.3 Verde catálogo](capturas/image10.png)

### Ronda 4 — El motor de realidad aumentada (`lib/dominio/motor_ar.dart`)
* **🔴 Rojo — `motor_ar_test.dart` (`Ciclo 4.1`):**
  ![Ciclo 4.1 Rojo motor AR](capturas/image11.png)
* **🟢 Verde — `calcularVisibles` (`Ciclo 4.2`):**
  ![Ciclo 4.2 Verde motor AR](capturas/image12.png)

### Ronda 5 — El pasaporte turístico (`lib/dominio/pasaporte.dart`)
* **🔴 Rojo — `pasaporte_test.dart` (`Ciclo 5.1`):**
  ![Ciclo 5.1 Rojo pasaporte](capturas/image13.png)
* **🟢 Verde — `Pasaporte` (`Ciclo 5.2`):**
  ![Ciclo 5.2 Verde pasaporte](capturas/image14.png)

### Ronda 6 — Fuentes de datos y el ViewModel (`lib/presentacion/ar_viewmodel.dart`)
* **🔴 Rojo — `ar_viewmodel_test.dart` (`Ciclo 6.1`):**
  ![Ciclo 6.1 Rojo ViewModel](capturas/image15.png)
* **🟢 Verde — `ArViewModel` (`Ciclo 6.2`):**
  ![Ciclo 6.2 Verde ViewModel](capturas/image16.png)
* **🟢 Pruebas de fuentes y simulación (`Paso 6.3`):**
  ![Paso 6.3 Pruebas fuentes](capturas/image17.png)

### Ronda 8 — RA de superficie: modelo 3D en tu espacio
* **Pantalla de inicio de `Dolores AR` (`Paso 8.2`):**
  ![Pantalla de inicio Dolores AR](capturas/image18.png)
