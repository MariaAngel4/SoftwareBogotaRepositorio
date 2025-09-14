# 🧩 Guía técnica — Integración Pagos Digitales

**Propietario:** Arquitectura — Laura Díaz  
**Última actualización:** 2025-09-13

## Resumen
Integración de la API de pagos internos: endpoints, autenticación y ejemplos de petición/respuesta.

## Endpoint principal
`POST /api/v1/payments`

### Ejemplo cURL
```bash
curl -X POST "https://api.softwarebogota.com/api/v1/payments" \
  -H "Authorization: Bearer <token>" \
  -H "Content-Type: application/json" \
  -d '{
    "amount": 150000,
    "currency": "COP",
    "customer_id": "CUST-001",
    "method": "card"
  }'
