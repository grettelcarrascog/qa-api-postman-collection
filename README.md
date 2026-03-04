# QA API Testing — Postman Collection

Colección de Postman para pruebas de API en un flujo bancario de transferencias.

## Incluye
- Pre-validaciones: estado de cuenta, alias/destinatario, balance
- Transferencias: create, status, cancel
- Estados: PENDING, PROCESSING, SUCCESS, REJECTED, CANCELLED
- Casos de error: INVALID_ALIAS, INSUFFICIENT_FUNDS, DAILY_LIMIT_EXCEEDED, CANNOT_CANCEL_IN_PROCESSING

## Cómo usar
1. Importar la colección en Postman
2. Configurar `baseUrl` con la URL del Mock Server
3. Ejecutar los requests (los responses se basan en Examples)

## Archivo
- `apitesting/Digital_Banking_Transfers.postman_collection.json`

## Mock server
Los responses de la colección se generan utilizando Postman Mock Server para simular distintos estados de transferencias y validar reglas de negocio, códigos de error y consistencia de estados sin depender de un backend real.
