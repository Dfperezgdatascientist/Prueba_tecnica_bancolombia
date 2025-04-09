![BC](Bancolombia.png)
# **Prueba Técnica - Analítico/a de Ecosistemas**
## Prueba Analítica: Modelo Opciones de Pago
### Científico de Datos:

* Daniel Felipe Pérez Grajales . dfperezg@unal.edu.co<br>

<br><br>

En el siguiente repositorio se pondrá a disposición el desarrollo de la prueba técnica para el puesto de Analítico/a de Ecosistemas en Bancolombia

**Objetivo**

Desarrollar una solución analítica E2E que permita poner en producción un modelo que genere un indicador de propensión a la aceptación de opción de pago de cada obligación de un cliente en mora.

### Archivos solución prueba:


1. **Prueba_Tecnica_BC_DsC_DFPG.ipynb** : jupyter notebook con el desarrollo de la construcción(ETL) y modelado<br>

2. **Solucion_desarrollo_prueba_DFPG.docx** : Documentación solución del problema<br> 

3. **resultado_prueba.csv** : Resultado predicción del modelo seleccionado fuera de muestra 30% <br>

4. **submision.csv** : Resultado predicción del modelo seleccionado fuera de muestra completa <br>

5. **AutoML_Model_pob_ob_pg.pkl** :  Pipeline con el modelo seleccionado, pesos del modelo<br>

6. **presentación: pendiente a la reunión**<br>

7. **diseña un sistema de manera teórica que bosqueje una solución que permita hacer disponibles los resultados de tu modelo analítico, y que sean fácilmente consumibles por servicios externos, como páginas web, servicio móvil, etc:** <br><br>

Para este caso se propone como solución orquestar la producción del modelo predictivo con MLflow y se podria construir un dashboard open sourse con el framework  shiny dashboard disponible para python y R donde se puede llevar a la medida de negocio, combinando variables palancas, estrategicas, sociodemograficas, transaccionales y hacerle seguimiento al  modelo, frente a temas de backtesting, falsos positivos, etc.La construccion de Kpi's, como el impacto que genera el modelo en producción frente al el índice de cartera vencida del banco.

Ejemplo:

![Dasboard](ejemplo_dashboard_aplicativo.png)

[URL](https://jjallaire.github.io/stock-explorer-dashboard/)

Esto se puede llevar a api's donde se dispone todo el proyecto en una VM ya sea(azure,aws,GCP) y se configura la IP publica,el DNS para darle nombre a la URL:(https://www.Bancolombia_seguimiento_opciones_pago.com) y dentro del la api se configuran temas de ciberseguridad como darle credenciales a la api y recapcha
