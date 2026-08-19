# 10-infra

Lab 10 · Montando la infraestructura, para `iasi-book-II`.

Este lab marca la frontera entre los laboratorios `0x-*`, que no requieren una infraestructura específica, y los laboratorios posteriores, que pueden asumir un entorno IASI Labs preparado.

Orden de construcción:

1. Software base
2. Desarrollo
3. Docker y servicios
4. IASI
5. Productos IASI

Principios de esta adaptación:

- infraestructura separada de `iasi-dev`;
- `Autounattend.xml` en lugar de `OOBE\BYPASSNRO`;
- Go incluido en la capa de desarrollo;
- productos IASI instalados, no repositorios fuente clonados;
- rango Docker `20xxx`;
- red Docker `iasi-labs`;
- checkpoints de referencia para el ciclo de labs.

## Estilos

`iasi-book-II` carga siempre:

```yaml
css:
  - resources/css/iasi.scss
  - resources/css/labs.scss
```

`iasi.scss` contiene el lenguaje visual común de IASI. `labs.scss` se reserva para componentes específicos de los laboratorios.
