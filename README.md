Introducción

En este proyecto, se analizarán los datos de reservas de una cadena hotelera para investigar las razones detrás de las altas tasas de cancelación y proponer estrategias para reducir estas cancelaciones y asegurar los ingresos. El dataset se obtuvo de Kaggle, una plataforma pública que proporciona acceso a una amplia variedad de datos. El conjunto de datos incluye información sobre dos tipos de hoteles (ciudad y resort) y si las reservas fueron canceladas o no. Cada registro corresponde a una reserva e incluye detalles como la fecha de llegada, duración de la estancia, número de adultos y niños, solicitudes especiales, entre otros.

Problema Planteado

El CEO de una cadena hotelera ha identificado un problema en el contrato con las agencias de marketing. El contrato establece un costo fijo mensual y un costo variable basado en las reservas realizadas. El CEO sospecha que están pagando por reservas canceladas, y no se ha verificado si la tasa de cancelación ha cambiado desde que se firmó el contrato. Las cancelaciones de última hora pueden llevar a pérdidas de ingresos significativas. El objetivo de este proyecto es analizar los datos de reservas, investigar los patrones de cancelación y sugerir medidas para reducirlas y proteger los ingresos.

Descripción de los Campos

hotel: Tipo de hotel (Ciudad o Resort)

is_canceled: Indicador de cancelación (1 = Cancelado, 0 = No Cancelado)

lead_time: Tiempo de anticipación en días para la reserva

arrival_date_year: Año de llegada

arrival_date_month: Mes de llegada

arrival_date_week_number: Número de semana de llegada

arrival_date_day_of_month: Día del mes de llegada

stays_in_weekend_nights: Noches de fin de semana en la estancia

stays_in_week_nights: Noches de semana en la estancia

adults: Número de adultos

children: Número de niños

babies: Número de bebés

meal: Tipo de comida

country: País de origen del huésped

market_segment: Segmento de mercado

distribution_channel: Canal de distribución

is_repeated_guest: Indicador de huésped recurrente (1 = Sí, 0 = No)

previous_cancellations: Número de cancelaciones anteriores

previous_bookings_not_canceled: Número de reservas anteriores no canceladas

reserved_room_type: Tipo de habitación reservada

assigned_room_type: Tipo de habitación asignada

booking_changes: Número de cambios en la reserva

agent: Agente de reservas

company: Compañía asociada con la reserva

days_in_waiting_list: Días en lista de espera

customer_type: Tipo de cliente

adr: Tarifa diaria promedio

required_car_parking_spaces: Espacios de aparcamiento requeridos

total_of_special_requests: Número total de solicitudes especiales

reservation_status: Estado de la reserva

reservation_status_date: Fecha del estado de la reserva

Preguntas de Investigación

¿Cuál es el porcentaje total de cancelaciones en la cadena hotelera?
¿En qué tipo de hotel ocurren con mayor frecuencia estas cancelaciones?
¿En qué mes del año se producen la mayor cantidad de cancelaciones?
¿De qué continente proviene el mayor porcentaje de cancelaciones? ¿Y de qué países?
¿Cuál es la tarifa media (ADR) para las reservas canceladas frente a las reservas cumplidas?
Según el gráfico del punto 4, ¿qué metodología de reservas se utiliza para las reservas en Portugal?
¿Hay muchas cancelaciones provenientes de agencias?

Hipótesis

A partir de enero, se observa un aumento en la cantidad de reservas hasta agosto, acompañado de un incremento en las cancelaciones. Los datos sugieren una tendencia de ADR más alta en las cancelaciones. Se podría suponer que las tarifas más altas están relacionadas con un mayor número de cancelaciones.
Según el problema planteado por el CEO, se observa un alto porcentaje de cancelaciones entre los huéspedes de Portugal, con la mayoría de estas reservas gestionadas por agencias. Esto sugiere que podrían estar pagando costos variables por reservas canceladas.
Posibles Soluciones
Requerir depósitos con tarjeta de crédito/débito o efectivo para evitar cancelaciones.
Ofrecer tarifas más bajas o descuentos para reservas directas y reducir la dependencia de reservas a través de agencias para disminuir el costo variable.
Revisar el contrato para eliminar el costo asociado a reservas canceladas.
Implementar una estrategia de overbooking cautelosa para maximizar la ocupación.

Storytelling

Introducción al Proyecto: Este proyecto se centra en predecir las cancelaciones de reservas de hotel y en cómo esta información puede ser utilizada para mejorar la gestión de ingresos en la industria hotelera.


Obtención del Conjunto de Datos: Utilizamos un conjunto de datos obtenido de Kaggle que proporciona información detallada sobre las reservas de hotel, incluyendo datos demográficos de clientes y detalles de las reservas.


Exploración del Conjunto de Datos y Limpieza: Realizamos una exploración exhaustiva del conjunto de datos para entender su estructura y características. Se limpian los datos eliminando registros faltantes o irrelevantes.


Proceso de Aprendizaje Automático: Describimos el proceso de entrenamiento del modelo utilizando librerías de scikit-learn para evaluar distintos modelos y ajustar sus parámetros.

División de Entrenamiento/Prueba: Se divide el conjunto de datos en conjuntos de entrenamiento y prueba para evaluar el rendimiento del modelo.


Evaluación del Rendimiento del Modelo: Se evalúa el modelo usando métricas como precisión y puntuación F1 para determinar su efectividad en la predicción de cancelaciones.

