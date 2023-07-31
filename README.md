# Retención de clientes
En este repositorio, hemos realizado un análisis exploratorio de datos de extremo a extremo e identificado las características de los clientes que tienen más probabilidades de abandonar, y las he usado sabiamente para crear e implementar modelos.


### 🟢 Para EDA, consulte: EDA.ipynb
### 🟢 Para la construcción de modelos, consulte: Modelos.ipynb
### 🟢 Para la implementación del modelo, consulte app.py

### 🔵 Creando flask API

```
app = Flask("__name__")
```

El método loadPage llama a nuestro home.html.
```
@app.route("/")
def loadPage():
	return render_template('home.html', query="")
```

El método de predicción es nuestro método POST, que básicamente se llama cuando pasamos todas las entradas de nuestro front-end y hacemos clic en SUBMIT.
```
@app.route("/", methods=['POST'])
def predict():
```
  
El método run() de la clase Flask ejecuta la aplicación.
```
app.run()
```


El script de Python dado anteriormente se ejecuta desde el shell de Python.
```
python app.py
```

Se ve el siguiente mensaje en el shell de Python, lo que indica que nuestra aplicación ahora está alojada en http://127.0.0.1:5000/ o localhost:5000
```
* Ejecutándose en http://127.0.0.1:5000/ (Presione CTRL+C para salir)
```

