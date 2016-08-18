# manso_grafico
Javascript para crear gráficos (no terminado aún)

Uso
--------------------------
Recibe un JSON con las coordenadas y rangos


```sh

// JSON CON LAS COORDENADAS DEL GRÁFICO
// ------------------------------------
var coords = {
	"rango_general": {
		"min": 40,
		"max": 120
	},
	"rango_normal": {
		"min": 63,
		"max": 85
	},
	"evaluaciones":{
		"punto1": {
			"x": 0,
			"y": 90,
			"fecha": "03 de mayo"
		},
		"punto2":{
			"x": 0,
			"y": 90,
			"fecha": "07 de mayo"
		},
		"punto3":{
			"x": 0,
			"y": 100,
			"fecha": "27 de junio"
		},
		"punto4":{
			"x": 0,
			"y": 70,
			"fecha": "14 de septiembre"
		},
		"punto5":{
			"x": 0,
			"y": 66,
			"fecha": "03 de noviembre"
		},
		"punto6":{
			"x": 0,
			"y": 50,
			"fecha": "20 de diciembre"
		},
		"punto7":{
			"x": 0,
			"y": 50,
			"fecha": "03 de octubre"
		}
	}
}

// CREACIÓN DEL OBJETO Y GRÁFICO
// -----------------------------
var miGrafico = new MansoGrafico(coords);
miGrafico.crearPuntos();
miGrafico.crearRangoGeneral();
miGrafico.crearRangoNormal();
miGrafico.arrastrando();
miGrafico.toolTipValorPunto();
miGrafico.triangulos();
miGrafico.traerFechas();

```


Demo del Gráfico
---------------------
[http://cajonarium.cl/github/manso-grafico/](http://http://cajonarium.cl/github/manso-grafico/)

Espero que les sirva.
