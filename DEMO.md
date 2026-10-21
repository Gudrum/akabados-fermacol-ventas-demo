# Akabados × Grupo Fermacol — demo comercial

Demo: https://gudrum.github.io/akabados-fermacol-ventas-demo/

## Guion de reunión (7 minutos)
1. Presentar: el vendedor toma el pedido durante la visita; Odoo gobierna condiciones e inventario.
2. Configurar venta: Distribuidora Andes B2B; observar tarifa del cliente.
3. River White: 30 m², 10% adicional, 23 cajas = 33,12 m². Agregar al pedido.
4. Agregar adhesivo y revisar entrega, cantidades e IVA ilustrativo.
5. Simular cambio de stock, ajustar y enviar nuevamente.
6. Ver Mis pedidos y repetir; mostrar aprobación con descuento adicional de 8% o cupo de Constructora Horizonte.
7. Mostrar Visión Odoo y acordar piloto: usuarios, bodega, catálogo, reglas y alojamiento.

## Alcance
Catálogo de 12 referencias; búsqueda/categorías/marca; selección cliente y bodega; precios por cliente; cálculo cajas; carrito; entrega; simulación sin conexión; borradores; aprobación crédito/descuento; conflicto stock; historial local; repetición, impresión y JSON.

## Límites
Aplicación estática sin backend. No autentica, no procesa pagos, no conecta con Odoo y no reserva inventario. El selector de roles es demostrativo. El modo sin conexión es una simulación, no una PWA offline instalada. Datos guardados únicamente en localStorage del navegador. Stock/precios/reglas son ficticios. Las ilustraciones son conceptuales. Los nombres de algunas referencias proceden del catálogo público de Akabados; otras son ilustrativas.

## Producción
Definir versión y alojamiento Odoo, empresas, unidades, conversiones, tarifas, impuestos, crédito y política de reservas. Implementar servidor con autenticación, autorización, validación transaccional, idempotencia y pruebas de concurrencia. Evitar credenciales en frontend.

## Ejecución
Servir index.html por HTTP. Sin compilación ni dependencias JavaScript. Tipografías remotas opcionales con fallback local. Publicación GitHub Pages desde main / raíz.
