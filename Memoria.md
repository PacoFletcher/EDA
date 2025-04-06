# Evolución de la renta en Euskadi, un vistazo a la distribución de la riqueza en Bilbao.

En este análisis exploratorio de datos se pretende estudiar cómo ha evolucionado la riqueza en el municipio de Bilbao en el periodo que abarca desde 2006 hasta 2022, teniendo encuenta el desglose de diferentes factores que influyen en la Renta de las Personas Físicas.

## Fuente de datos, metodología y definiciones

Los datos han sido extraídos de la base de datos oficial de Euskadi, a través de este enlace: https://www.eustat.eus/bankupx/pxweb/es/DB/-/PX_173402_crpf_rpf_rp22_2p.px/table/tableViewLayout2/.

Además, se han extraído los datos referentes a la evolución de los precios de alquiler y compra de los diferentes barrios de Bilbao de los datos públicos de [Idealista](https://www.idealista.com/sala-de-prensa/informes-precio-vivienda/venta/euskadi/vizcaya/bilbao/), así como los relativos a la evolución del IPC en el país vasco del [INE](https://www.ine.es/jaxiT3/Tabla.htm?t=50940&L=0). 


Según la propias fuentes, la fiabilidad de estos resultados es del 89,62%.

>La RPF mantiene la correspondencia entre los ficheros procedentes de las Haciendas Forales y el Registro de Población de Eustat. El indicador de la Tasa de Fusión Bruta, que mide la media ponderada de porcentajes de fusión del Registro de Población con cada fuente utilizada, en 2022 ha sido de 89,62%.

En este conjunto de datos se ha tomado teniendo en cuenta únicamente a la población de más de 18 años, lo cual permite que la mayor o menor abundacia menores de edad no influya en la distribución de la renta.

Variables y definiciones:
* **Renta personal total**: Resulta de la agregación, para cada persona de 18 y más años, de sus rentas del trabajo, rentas derivadas de actividades económicas, transferencias o prestaciones sociales y las percibidas por el capital, tanto mobiliario como inmobiliario.
* **Renta del trabajo** : Se entiende por renta del trabajo la remuneración total, monetaria o no monetaria, que paga un empleador a su asalariado como contrapartida del trabajo realizado por éste durante el período de referencia de los ingresos.
* **Renta del capital mobiliario**: Se consideran rendimientos del capital mobiliario los intereses de cuentas bancarias, bonos, obligaciones y, en general, títulos de renta fija, los dividendos de acciones y las plusvalías obtenidas por la transmisión de cualquier tipo de valores mobiliarios, percibidos durante el período de referencia. En la práctica los rendimientos del capital mobiliario lo conforman los intereses, dividendos, plusvalías, etc. sin descontar las retenciones efectuadas. Sólo se tienen en cuenta intereses declarados de cuantía superior o igual a 5 euros. <nl> 
Bajo este epígrafe también se incluyen los rendimientos obtenidos en EPSVs (Entidades de Previsión Social Voluntaria). Se toma el 35% del rescate como estimación de las ganancias obtenidas. <nl>
También dentro de este epígrafe se incluyen las ganancias y pérdidas patrimoniales derivadas de la transmisión de participaciones en fondos de inversión colectiva, acciones, seguros, etc.
* **Renta del capital inmobiliario**: Se consideran rendimientos del capital inmobiliario los que se derivan del arrendamiento o de la constitución o cesión de derechos o facultades de uso o disfrute sobre bienes inmuebles rústicos y urbanos, percibidos durante el período de referencia.
* **Renta de actividades económicas**: Se entienden por rendimientos de actividades económicas aquéllos que, procediendo del trabajo personal y del capital conjuntamente o de uno sólo de estos factores, suponen por parte del contribuyente la ordenación por cuenta propia de medios de producción o de recursos humanos con la finalidad de intervenir en la producción o distribución de bienes y servicios. 
* **Transferencias**: Se entienden por transferencias las prestaciones sociales monetarias de cobertura obligatoria o basadas en el principio de solidaridad social (quedan excluidas por tanto las prestaciones sociales voluntarias).

* **Renta disponible**: Resulta de descontar a la renta personal total los gastos de Seguridad Social y la cuota líquida o las retenciones a cuenta.

## Hipótesis

1. Pese al aparente aumento de la renta, al ajustar esta a la inflación, se observa una pérdida del poder adquisitivo de los ciudadanos.

2. Las diferencias entre los barrios con mayor poder adquisitivo respecto a aquellos más desfavorecidos se acentúan, aumentando las desigualdades.

3. La vivienda es un factor determinante respecto al incremento de la renta.

