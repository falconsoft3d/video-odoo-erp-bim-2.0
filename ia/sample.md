Dada una archivo de una edificio, genera un presupuesto de construcción detallado. Estructura el presupuesto en formato JSON con 20 capitulos.

Para cada capítulo, incluye:
1. **Partidas**: Define cada partida relevante, indicando una breve descripción, unidad de medida y cantidad aproximada.
2. **APUs (Análisis de Precios Unitarios)**: Para cada partida, especifica el precio unitario y el costo total.
3. **Recursos**: Lista los recursos necesarios para cada partida, incluyendo mano de obra, materiales y equipos. Para cada recurso, especifica la cantidad, unidad de medida, costo unitario y costo total.

Solo dame el json no me des ni encabezado ni pie de página porque lo quiero meter en un json.
Solo creame un capitulo y que todas las partidas sean hija de ese capitulo
No me des el json cortado

Devuélveme el resultado en formato JSON con la siguiente estructura:

{
      "concepts": [
        {
          "id": 17,
          "code": "01",
          "name": "CAPITULO 1",
          "type": "chapter",
          "quantity": 1.0,
          "price": 1.0,
          "parent": false,
          "performance": 0.0,
        },
        {
          "id": 72,
          "code": "01.1",
          "name": "Cimentacion corrida de hormigon",
          "type": "departure",
          "quantity": 100,
          "price": 1.0,
          "parent": 17,
          "performance": 0.0,
        },
        {
          "id": 95,
          "code": "012",
          "name": "Ladrillo de 15x20",
          "type": "material",
          "quantity": 1.0,
          "price": 1.0,
          "parent": 72,
          "performance": 0.0,
        },
        {
          "id": 96,
          "code": "0121",
          "name": "Hormigon Armado de 20Pma",
          "type": "material",
          "quantity": 300.0,
          "price": 1.0,
          "parent": 72,
          "performance": 0.0,
        },
        {
          "id": 97,
          "code": "012.2",
          "name": "Ayudante ",
          "product": 6,
          "type": "labor",
          "quantity": 1.0,
          "price": 1.0,
          "parent": 72,
          "performance": 0.0,
        },
        {
          "id": 98,
          "code": "012.3",
          "name": "Motoniveladora",
          "type": "equip",
          "quantity": 2.0,
          "price": 22.0,
          "parent": 72,
          "performance": 0.0,
        }
  ]
}
