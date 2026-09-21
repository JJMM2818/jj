## Registros de propósito general

| Código | Registro | Función | Tamaño |
|---|---|---|---:|
| `0000` | R0 | Registro general | 64 bits |
| `0001` | R1 | Registro general | 64 bits |
| `0010` | R2 | Registro general | 64 bits |
| `0011` | R3 | Registro general | 64 bits |
| `0100` | R4 | Registro general | 64 bits |
| `0101` | R5 | Registro general | 64 bits |
| `0110` | R6 | Registro general | 64 bits |
| `0111` | R7 | Registro general | 64 bits |
| `1000` | R8 | Registro general | 64 bits |
| `1001` | R9 | Registro general | 64 bits |
| `1010` | R10 | Registro general | 64 bits |
| `1011` | R11 | Registro general | 64 bits |
| `1100` | R12 | Registro general | 64 bits |
| `1101` | R13 | Registro general | 64 bits |
| `1110` | R14 | Registro general | 64 bits |
| `1111` | R15 | Registro general | 64 bits |

## Tabla de registros especiales

| Código | Registro | Función | Tamaño |
|---|---|---|---:|
| `0001 0000` | PC | Contador de programa | 64 bits |
| `0001 0001` | IR | Registro de instrucción | 64 bits |
| `0001 0100` | SP | Puntero de pila | 64 bits |
| `0001 0101` | BP | Puntero base | 64 bits |
| `0001 0110` | PSW | Estado y banderas | 64 bits |
| `0001 0111` | CR | Registro de control | 64 bits |

## Tabla de buses

| Bus | Tamaño | Función |
|---|---:|---|
| Bus de datos | 64 bits | Transporta datos e instrucciones |
| Bus de direcciones | 64 bits | Transporta direcciones de memoria |
| Bus de control | 16 bits | Transporta señales de control |
| Bus de periféricos | 32 bits | Comunica los controladores con los periféricos |

## Tabla de formatos de instrucciones

| Formato | Tamaño | Campos | Distribución |
|---|---:|---|---|
| F1 | 1 byte | CODIGO | 8 bits |
| F2 | 2 bytes | CODIGO + REG1 + REG2 | 8 + 4 + 4 bits |
| F3 | 4 bytes | CODIGO + REG + PUERTO | 8 + 8 + 16 bits |
| F4 | 5 bytes | CODIGO + DESPLAZAMIENTO | 8 + 32 bits |
| F5 | 6 bytes | CODIGO + REG + DESPLAZAMIENTO | 8 + 8 + 32 bits |
**Tabla de formatos**




**Tabla de intrucciones**

| Instrucción | Código binario | Decimal |
|---|---:|---:|
| NOP | 0000 0000 | 0 |
| DETENER | 0000 0001 | 1 |
| MOVER | 0001 0000 | 16 |
| CARGAR | 0001 0001 | 17 |
| GUARDAR | 0001 0010 | 18 |
| CARGARINM | 0001 1001 | 25 |
| EMPUJAR | 0001 1010 | 26 |
| SACAR | 0001 1011 | 27 |
| INTERCAMBIAR | 0001 1100 | 28 |
| SUMAR | 0010 0000 | 32 |
| SUMAR_C | 0010 0001 | 33 |
| RESTAR | 0010 0010 | 34 |
| RESTAR_C | 0010 0011 | 35 |
| MULTIPLICAR | 0010 0100 | 36 |
| DIVIDIR | 0010 0101 | 37 |
| MODULO | 0010 0110 | 38 |
| INCREMENTAR | 0010 0111 | 39 |
| DECREMENTAR | 0010 1000 | 40 |
| NEGAR | 0010 1001 | 41 |
| COMPARAR | 0010 1010 | 42 |
| PRUEBA | 0010 1011 | 43 |
| Y | 0011 0000 | 48 |
| O | 0011 0001 | 49 |
| XOR | 0011 0010 | 50 |
| NO | 0011 0011 | 51 |
| DESP_I | 0011 0100 | 52 |
| DESP_D | 0011 0101 | 53 |
| ROTA_I | 0011 0110 | 54 |
| ROTA_D | 0011 0111 | 55 |
| SALTAR | 0100 0000 | 64 |
| SALTAZ | 0100 0001 | 65 |
| SALTAN | 0100 0010 | 66 |
| SALTAC | 0100 0011 | 67 |
| SALTAV | 0100 0100 | 68 |
| SALTA_NOZ | 0100 0101 | 69 |
| LLAMAR | 0100 0110 | 70 |
| RETORNAR | 0100 0111 | 71 |
| LEER_PUERTO | 0101 0000 | 80 |
| ESCRIBIR_PUERTO | 0101 0001 | 81 |
| DMA_ENTRADA | 0101 0010 | 82 |
| DMA_SALIDA | 0101 0011 | 83 |
| LEER_TECLADO | 0101 0100 | 84 |
| ESCRIBIR_PANTALLA | 0101 0101 | 85 |
| RED_ENVIAR | 0110 0000 | 96 |
| RED_RECIBIR | 0110 0001 | 97 |
| RED_ESTADO | 0110 0010 | 98 |
| RED_CONFIG | 0110 0011 | 99 |
| RED_CERRAR | 0110 0100 | 100 |
| CACHE_LIMPIAR | 0111 0000 | 112 |
| LEER_RTC | 0111 0100 | 116 |
| ESCRIBIR_RTC | 0111 0101 | 117 |
