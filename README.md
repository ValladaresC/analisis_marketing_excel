# analisis_marketing_excel

Este proyecto se llevo a cabo para la empresa "INCOGNITA" la cual estaba manifestando grandes pérdidas en sus campañas de marketing y quería saber hacia donde redirigir sus recursos.

Las etapas del análisis son mostradas a continuación:

## 1. Trasnformación de .csv a .xlsx

## 2. Reconocimiento de los campos:
- c_date: Fecha en que se realizó la campaña o en la que se registraron los datos.

- campaign_name: Nombre de la campaña de marketing.
Ejemplo: facebook_tier1, google_hot, youtube_blogger.

- category: Categoría o tipo de campaña, que indica el canal o el enfoque de marketing.

- campaign_id: Identificador único de la campaña en el sistema de gestión o plataforma de publicidad.

- impressions: Número de veces que los anuncios de la campaña fueron mostrados a los usuarios. Es decir, cada vez que un anuncio aparece en la pantalla de un usuario, se cuenta como una impresión, independientemente de si el usuario interactúa con él o no.

- mark_spent (probablemente "amount spent"): Cantidad de dinero gastada en la campaña, generalmente en la misma moneda.

- clicks: Número de veces que los usuarios hicieron clic en los anuncios.

- leads: Número de contactos o potenciales clientes generados a través de la campaña (por ejemplo, registros, solicitudes de información).

- orders: Número de pedidos o compras realizadas como resultado de la campaña.

- revenue: Ingresos generados por la campaña, generalmente en la moneda correspondiente.

## 3. Limpieza de datos:
- Corrección en la columna campaign_name, dejando solo el nombre principal de la red usada (Facebook, YouTube, etc) y reemplazando facebOOK por FACEBOOK.
- La columna campaign_name se renombro con Platform y la columna separada con Sub_Platform.
- Las columnas campaign_id, impressions, mark_spent, clicks, leads, orders y revenue son formateadas a numero.
- Eliminar columna campaign_id.

## 4. Agregaciones
- Columna con ROI: el ROI (Retorno de la Inversión) es una métrica que mide la eficiencia de una campaña de marketing. Se calcula dividiendo los ingresos generados por la campaña entre el costo de la inversión en la misma. El ROI ayuda a las empresas a entender qué campañas son más rentables y cómo optimizar la inversión en marketing para obtener mejores resultados. El ROI se calcula de la siguiente manera:
ROI = (Ingresos generados - Costo de la inversión) / Costo de la inversión 
- Columna con CPI: el Coste por Interacción es aquel donde los clientes potenciales interactúan durante algunos segundos con alguno de los anuncios o banners publicitarios que promociona una marca o producto sin hacer click. Se calcula:
CPI = Costo / impresiones
- Columna con CPC: el Coste por Click es un modelo de precios en el que los anunciantes pagan una cantidad específica por cada clic que reciben en sus anuncios.
- Columna con CPL: el Coste por Leads es una métrica que indica cuánto cuesta a una empresa obtener un potencial cliente o prospecto. Es decir, el costo de un usuario que ha mostrado interés en un producto o servicio y ha dejado sus datos para ser contactado.
- Columna con CPO: el Coste por Orders es una métrica que calcula el gasto promedio de marketing para obtener una venta.
- Calcular las siguientes medidas que representan diferentes etapas del embudo de conversión o la transición entre ambos:
Imp > Click: Un clic representa que alguien vio el anuncio y luego lo consideró interesante para continuar.
Click > Lead: Se considera un lead cuando alguien no solo hace clic en el anuncio, sino que también deja sus datos de contacto.
Lead > Order: Un lead se convierte en pedido cuando un potencial cliente decide adquirir tu producto o servicio después de haber expresado interés y haber sido contactado.

> [!IMPORTANT]
> El embudo de conversión representa el viaje de un usuario desde la primera exposición a un anuncio (impresión) hasta la compra final, pasando por la fase de interacción (clic) y la generación de interés (lead).

## 5. Análisis por tabla

### Tabla 1.

![image](https://github.com/user-attachments/assets/952ec666-56c6-4fea-93f8-754bb5cfee9d)

- La categoría "Influencer" tiene el ROI más alto, lo que indica que es la canalización que más retorno está generando en relación a la inversión realizada. Por otro lado, "Social" tiene el ROI más bajo, sugiriendo que genera menos retorno comparado con las otras categorías.
- La categoría "Media" tiene el CPI más bajo, lo que significa que en promedio cuesta menos conseguir una impresión o evento. "Search" tiene el CPI más alto, reflejando que es más costoso en promedio.
-  Los costos por clic son similares en las categorías de "Influencer" y "Social", ligeramente más altos que en "Media" y "Search". Esto indica cuánto cuesta en promedio obtener un clic en cada canal.
- "Media" tiene el CPL más bajo, lo que indica que es más eficiente en convertir clics en clientes potenciales. "Social" tiene el CPL más alto, siendo más costoso en ese aspecto.
- La categoría "Media" tiene el costo por orden más bajo, lo que sugiere que es más eficiente en términos de convertir leads en ventas finales. "Social" tiene el CPO más alto, lo que indica un menor rendimiento en la conversión final en ese canal.

En resumen, la categoría "Influencer" destaca por tener el mayor ROI, pero también un alto CPO y CPL, lo que puede indicar que aunque genera mucho retorno, también es costosa.
La categoría "Media" muestra ser la más eficiente en costo total, con bajos CPI, CPL y CPO, además de un ROI moderado. "Search" tiene costos elevados en CPI y CPO, pero un ROI relativamente bueno. "Social" tiene los menores ROI y mayores costos en CPL y CPO, lo que sugiere que puede no ser la estrategia más eficiente en términos de retorno y costos finales.

### Tabla 2.

![image](https://github.com/user-attachments/assets/cf028a2a-8c71-434e-9ee3-9dcde92b4b67)

YouTube en la categoría Influencer destaca por tener un ROI extremadamente alto y costos relativamente bajos en CPI, CPC, CPL y CPO, lo que indica que es la plataforma más efectiva en tu campaña.

Instagram en la categoría Influencer destacada en comparación con la categoría Social, en ambos casos tiene un buen ROI, aunque mucho menor que YouTube, y costos bajos en las otras medidas. Por otra parte Facebook presenta los resultados menos favorables en términos de ROI y costo por acción, siendo menos eficiente.

### Tabla 3.

![image](https://github.com/user-attachments/assets/6b5dd01f-5c96-42fc-b3e0-1ec600513e11)


En la categoría Social, las plataformas Facebook e Instagram presentaron las peores rentabilidades en sus campañas lai con -88% y tier2 con -40% respectivamente. Sin embargo la campaña retargeting de Facebook es la segunda campaña mas rentable entre todas las demás categorías con un ROI de 145%.

### Tabla 4.

Analizando las variables de conversión, es necesario acotar que mientras menor sea el numero será mejor. 

![image](https://github.com/user-attachments/assets/f275a346-1ed7-47ec-8408-bdea69db90d9)

En la categoría Social de la plataforma Facebook se encontró lo siguiente:
- Imp > Click: indica que necesitas menos impresiones para conseguir un clic. La campaña "retargeting" es la más eficiente en esta métrica (33 impresiones por clic).
- Click > Lead: menor número indica que menos clics se necesitan para convertir en un lead. Aquí, "tier2" tiene la mejor relación (53 clics por lead).
- Lead > Order: menor número significa que menos leads se necesitan para realizar una venta. "retargeting" también tiene la mejor tasa en esta métrica (4 leads por orden).
En resumen la campaña retargeting es la más eficiente en convertir impresiones en clics y leads, y también en cerrar ventas a partir de leads; mientras que la campaña lal requiere muchas impresiones para un clic (107) y muchos clics para un lead (161), lo que indica menor eficiencia. Y por último las campañas tier1 y tier2 quedarían descartadas ya que muestran diferentes balances entre estas métricas, pero en general "tier2" tiene una buena tasa en clics por lead, aunque requiere más leads para una venta en comparación con "retargeting".

### Tabla 5.

Se amplió la tabla con un campo calculado llamado Average Order Value (AOV) que es el valor promedio de ingresos por orden. Es decir, estás calculando el ingreso promedio por orden o valor promedio del pedido. Este indicador es útil para entender cuánto dinero, en promedio, genera cada orden de compra en tu negocio.

![image](https://github.com/user-attachments/assets/7bb6b2a1-e9aa-458c-8efe-dba57504702a)

Este indicador muestra que los mejores valores promedios de ingreso por orden pertenecen a retargeting, tier1  y tier2, sin embargo estas dos últimas presentan un desbalance en la etapa de cliente potencial (Click > Lead) ya que se requieren muchos clicks para obtener un lead. Además, queda evidenciado por mark_spent que hay mucho gasto en estas dos campañas con AOV similares a retargeting, por lo tanto la inversión en campañas debería dirigirse hacia retargeting.

### Tabla 6.

![image](https://github.com/user-attachments/assets/67329a38-31c8-4506-a8b3-5fee5d696b18)

Adicional se contaron la cantidad de campañas llevadas a cabo porque una sola campaña por cada tipo de campaña no sería representativa al comparar la rentabilidad con las demás campañas, sin embargo se obtuvo que por cada tipo de campaña realizada en Facebook fueron realizadas 28 campañas. Quiere decir entonces que 84 campañas pertenecientes a "lal", "tier1" y "tier2" tuvieron ROI negativos y solo 28 campañas pertenecientes a "retargeting" obtuvieron ROI positivos.

## Visualización de Resultados

![analisis_marketing_resultados](https://github.com/user-attachments/assets/39f0cf50-26f4-46b0-840b-79ad906e4ccc)

