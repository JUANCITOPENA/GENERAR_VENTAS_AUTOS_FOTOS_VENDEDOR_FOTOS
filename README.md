# 🚗 Generador de Datos de Ventas

Este proyecto permite generar datos simulados de ventas de vehículos, con información de clientes, vendedores y ciudades en República Dominicana. Es ideal para practicar análisis y visualización de datos.

## 📋 Características
- Generación de datos aleatorios para clientes, vendedores y vehículos.
- Visualización de los datos generados en una interfaz de usuario interactiva con [Streamlit](https://streamlit.io/).
- Integración con la API [RandomUser.me](https://randomuser.me/) para obtener imágenes y datos de vendedores.
- Exportación de los datos generados en formatos estructurados para análisis posterior.

## 🔧 Tecnologías Utilizadas
- **Python**: Lenguaje principal.
- **Streamlit**: Para la creación de una interfaz de usuario interactiva.
- **Faker**: Generación de datos aleatorios como nombres, correos y fechas.
- **Pandas**: Procesamiento y manipulación de datos.
- **Requests**: Para consumir la API de RandomUser.

## 🚀 Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tu_usuario/tu_repositorio.git
   cd tu_repositorio
   ```

2. Instala las dependencias requeridas:
   ```bash
   pip install -r requirements.txt
   ```

3. Ejecuta la aplicación con Streamlit:
   ```bash
   streamlit run app.py
   ```

## 🎮 Cómo Usar

1. **Configura los filtros** desde la barra lateral:
   - Número de clientes.
   - Número de vendedores.
   - Número de vehículos.
   - Fechas de inicio y fin para las ventas.
   - Cantidad de facturas a generar.

2. Haz clic en el botón **Generar** para simular los datos.

3. Visualiza los resultados en la interfaz principal, incluyendo:
   - Datos detallados de ventas.
   - Información de clientes y vendedores con imágenes.

## 📊 Dataset Incluye
- **Clientes**: Nombres generados aleatoriamente.
- **Vendedores**: Información y fotos obtenidas de RandomUser.
- **Vehículos**: Lista predefinida con 35 modelos diferentes, características y precios.
- **Ventas**: Facturas con detalles de productos, cantidades, totales y ciudades de venta.

## 🌍 Ciudades Incluidas
El simulador soporta ventas en múltiples ciudades de República Dominicana, como Santo Domingo, Santiago, La Romana, y más.

## 📦 Ejemplo de Salida de Datos
```json
{
  "id_venta": "123e4567-e89b-12d3-a456-426614174000",
  "vendedor": {
    "nombre": "Juan Pérez",
    "email": "juan.perez@example.com",
    "telefono": "809-555-1234",
    "gender": "male",
    "picture": {
      "url": "https://randomuser.me/api/portraits/men/1.jpg"
    }
  },
  "cliente": "María Gómez",
  "productos": [
    {
      "producto": "Toyota Corolla",
      "cantidad": 1,
      "total_producto": 23500,
      "imagen": "https://di-uploads-pod7.dealerinspire.com/toyotaofnorthmiami/uploads/2022/10/2023-GR-Corolla-1.png"
    }
  ],
  "total_venta": 23500,
  "fecha_venta": "2023-12-01",
  "ciudad_venta": "Santo Domingo"
}
```

## ✨ Autor
- **Ing. Juancito Peña**  
  🚀 Contacto: [LinkedIn](https://www.linkedin.com/in/juancitopeña) | [GitHub](https://github.com/tu_usuario)

## 📜 Licencia
Este proyecto está bajo la Licencia MIT - consulta el archivo [LICENSE](LICENSE) para más detalles.
