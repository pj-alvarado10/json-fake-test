# json-fake-test
It is a json server fake test to test the server of https://my-json-server.typicode.com/ 

Exactly, the fake service is in https://my-json-server.typicode.com/pj-alvarado10/json-fake-test

# Limits
Remembers the limits to be able to provide a free service to as many people as possible during this phase, the project comes with a few limits:

* Changes are faked and aren't persisted (just like JSONPlaceholder)
* Requests are cached (1 minute)
* db.json has limits
* All servers are public

# Fake data json in https://json-generator.com/
with json:

      
     [
      '{{repeat(5, 25)}}',
      {
        "numeroProducto": '{{guid()}}',
        "numeroRegistro": function(tags, index) { return index+""; },
        "estado": '{{random("vigente", "suspendido", "cancelado", "vencido")}}',
        "fechaVencimiento":'{{date(new Date(2024, 0, 1), new Date(), "YYYY-MM-dd")}}',
        "marcas":'{{lorem(1, "words")}}',
        "condicionesConservacion":'{{lorem(1, "sentences")}}',
        "responsables": [ '{{repeat(1, 3)}}',
          {
            "tipoResponsable": '{{random(1, 2, 3)}}',
            "tipoIdentificacion":'{{random("CC", "NIT", "CE")}}',
            "identificacion": '{{integer(100000000000, 999999999999)}}'
          }
         ]
      } 
    ]

