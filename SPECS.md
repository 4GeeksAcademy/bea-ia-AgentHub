# AGENTHUB

## Descripcion del producto
Este documento es como una guía detallada que explica cómo debe ser y cómo debe funcionar el panel de administración de AgentHub (solo frontend). Una maqueta funcional


## Stack técnico
- HTML semantico
- TailwindCSS (CDN)
- JavaScript Vanilla


## Requerimientos
- toggle de modo oscuro/claro en la barra superior cambia todo el panel entre esquemas de color usando utilidades dark de tailwind. el modo elegido se conserva al navegar entre secciones
-todos los drpdowns de acciones se cierran al hacer clic fuera de su area
-todos los modales se cierran al hacer clic en background
- una sidebar persistente con enlacesde navegacion a las 6 secciones

### secciones
-Dashboard
-Gestión de usuarios
-Gestión de agentes
-Skills
-Contrataciones de agentes
-Log de errores
#### dashboard
-cuatro tarjetas metricas (ingresos totales, perdidas por descuentos, agentes activos y agentes fallando)
-área de ancho completo debajo de las tarjetas que representa un grafico de actividad semanal

#### Gestion de usuarios
-tabla de almenos 5 filas de usuarios nhardcodeados mostrando nombre, email, plan y badge de estado
-cada fila tiene un dropdown con "Ver detalle" y "Eliminar"
-"Ver detalle abre un modal con el registro de usuario. El modal cierra con el boton cierre y haciendo clic en el backdrop.

#### Gestion de agentes
-liatado de almenos 4 con nombre, propietario, badge de estado y lista de skills colapsadas
- hacer click en el control explandible revela las skills del agente con una transicion suave; volver a hacer click colapsa
-cada agente tiene un dropdown con "configurar" y "eliminar". "configurar abre un modal con el prompt de sistema del agente en un <texarea> editable

#### Skills 
-catalogo de 4 skills con nombre, descripcion y numero de agentes que la tienen habilitada
-explicacion breve dentro del panel de que es una skill en el contexto de AgentHub
-cad skill dropdown "ver detalle" y "eliminar"-

#### contratacion de agentes
-tabla de almenos 4 contratos mostrando cliente. agente, skills contratadas, fechas de inicio/fin e importe pagado
- cada fila un drpdown: "ver detalle" abre un modal con desglose del contrato incluyendo skills desglosadas y sus precios

#### Log de errores
-almenos 6 entradas de error hardcodeadas mostrando timestamp, nombre del agente, badge de tipo error de codigo de color y descripcion breve
-cada entrada un dropdown: "ver detlle" y "marcar como resuelto"



## restricciones
-Sin frameworks y sin backend
-sin CSS personalizados y sin atributos stylr rn linea



