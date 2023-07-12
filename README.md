# Control de Monotributistas 2.0

Programa asistido con bots para realizar el control de monotributistas de AFIP. los Bots se encargan de descargar los archivos de Mis Comprobantes y Facutas Emitidas, luego el Programa se encarga de procsar y cruzar ambos archivos para emitir un informa acerca de las recategorizaciones a realizar.

---

El licenciamiento es bajo PL (es decir que no se puede distribuir comercialmente, solamente GRATIS). y si se utiliza este el código, su derivado también debe ser distribuido abierta y gratuitamente.

---

## Orden de Ejecución

1. Actualizar el Excel de `Categorias.xlsx` Tanto en la solapa de `categoria` como la de `Rango de Fechas`

2. Actualizar en Excel dentro de la carpeta `BOTS` con el nombre de `Listado Mis Comprobantes 2.0.xlsx` con los datos fiscales de los monotributistas y el rango de fechas a descargar.

2. Se debe ejecutar el bot que se llama `Descarga-MC-AFIP.xaml` (en caso que los archivos no se guarden dentro de la carpeta del bot se debe ejecutar la versión que se llama `Descarga-MC-AFIP Sin ST.xaml`)

3. Una vez descargados los archivos de Mis Comprobantes se debe ejecutar el bot `Descarga Facturas Multiusuario.xaml` (en caso que los archivos no se guarden dentro de la carpeta del bot se debe ejecutar la versión que se llama `Descarga Facturas Multiusuario Sin ST.xaml`)

4. Finalmente una vez que se tienen los archivos de Mis Comprobantes y las Facturas se debe ejecutar el Programa `Control-Monotributistas-2.0.exe` que generará un reporte en la carpeta donde se encuenta en instalador con el nombre `Reporte Recategorizaciones de Monotributistas.xlsx` y `Datos de Facturas PDF.xlsx`

5. Ejecutar el programa `Control-Monotributistas-2.0.exe` para generar el reporte de recategorizaciones.

---

## Ejecución de los Bots

Los pasos para ejecutar los bots son los siguientes:

1. Crearse una cuenta en UiPath ([https://www.uipath.com/](https://www.uipath.com/)).

2. Descargar el Uipath Studio (https://www.uipath.com/studio) en la versión Community (es gratuita).

3. Instalar la version el Studio (no la Studio X).

  - Si se instala la versión Studio X se debe cambiar la versión del proyecto a Studio X con desde las configuraciones

  ![Configuración de versión](https://github.com/abustosp/Configuraciones/blob/master/Uipath/Cambiar-a-Studio.png "Configuración de versión")

  - Si no permite hacer este cambio se debe:

    1. Iniciar sesión en Uipath cloud.

    2. Eliminar la organización.

    3. Crear una nueva organización.

4. Ir a la carpeta BOTS

5. Una vez Descargados los archivos se debe:
   
   1. Abrir el project.json o archivo .xaml
   
   2. Ejecutarlo (hacer click en el boton de "Play").

---

## Particularidades del BOT/Programa:

- El bot corre en Firefox, por lo que se debe tener instalado el Firefox y Uipath.

- El bot Corre bajo windows 10 como mínimo (se puede ejecutar en una VM de linux o MAC con Win10).

- En caso que no se guarden los Archivos con el nombre y/o ubicación definidas en el Excel se debe ejecutar el bot que contiene en su nombre "sin ST"

- Firefox se debe configurar de la siguiente manera:

  1. El idioma tiene que estar en Español de Argentina

  ![Configuración de idioma](https://github.com/abustosp/Configuraciones/blob/master/Firefox/Idioma-Espa%C3%B1ol-ARG.png "Configuración de idioma")

  2. La descarga de archivos debe estar configurada para que se pregunte donde guardarlos

  ![Configuración de descarga](https://github.com/abustosp/Configuraciones/blob/master/Firefox/Ubicacion-de-descargas.png "Configuración de descarga")

  3. La descarga de archivos debe estar configurada para que no se pregunte si se quiere guardar el archivo (si el archivo aparece en la lista tiene que estar configurado con la opción de "Guardar Archivo" por ejemplo en el caso de los PDF y XLSX o planillas de cálculo)

  ![Configuración de descarga](https://github.com/abustosp/Configuraciones/blob/master/Firefox/Descarga-de-Archivos.png "Configuración de descarga")

---

## Aclaraciones

- La utilización del bot corre bajo la responsabilidad del que lo ejecuta.

- Si se comparte debe ser de manera GRATUITA, ya que la licencia es bajo PL. También los bots derivados deben seguir la misma licencia gratuita.

---

## Links de Interés:

- Link de invitación al grupo de RPA en Discord: https://discord.gg/KVYyryvAcD

- Link de invitación al grupo de RPA en WhatsApp: https://chat.whatsapp.com/IekktfvfTNLCkdIagO6xz3

- Tutorial de Descarga de Bots desde Uipath: https://youtu.be/hD5BH7YzABw

- Tutorial de Instalación y descarga de Repositorios con Git: https://youtu.be/ujk27tRdA80

---

Cualquier cosa pueden contactarme en:

- https://www.linkedin.com/in/agust%C3%ADn-bustos-piasentini-468446122/

- https://www.youtube.com/user/agustinbustosp

- whatsapp al https://wa.me/+5493764224695

---

<br/>

## 💰 Acepto donaciones para mantener el proyecto libre y gratuito

<br/>

[![PayPal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/agustinbustosp) <!-- [<img src="http://ketekipo.com.ar/wp-content/uploads/2020/05/mercado-pago.png" alt="Image" height="30" width="100\">](https://paypal.me/paypal.me/agustinbustosp) -->

[![Invitame un café en cafecito.app](https://cdn.cafecito.app/imgs/buttons/button_5.svg)](https://cafecito.app/abustos)

<br/>

## 💰 Y También en Pesos Argentinos

<br/>

[![Mercado Pago](https://img.shields.io/badge/Mercado%20Pago%20100-009ee3?style=for-the-badge&logo=mercadopago&logoColor=white)](https://mpago.la/2JBdGez)

[![Mercado Pago](https://img.shields.io/badge/Mercado%20Pago%20500-009ee3?style=for-the-badge&logo=mercadopago&logoColor=white)](https://mpago.la/2CwfjKE)

[![Mercado Pago](https://img.shields.io/badge/Mercado%20Pago%201.000-009ee3?style=for-the-badge&logo=mercadopago&logoColor=white)](https://mpago.la/21Xvpig)

[![Mercado Pago](https://img.shields.io/badge/Mercado%20Pago%205.000-009ee3?style=for-the-badge&logo=mercadopago&logoColor=white)](https://mpago.la/1s4D4mM)

[![Mercado Pago](https://img.shields.io/badge/Mercado%20Pago%2010.000-009ee3?style=for-the-badge&logo=mercadopago&logoColor=white)](https://mpago.la/1n9cimr)
