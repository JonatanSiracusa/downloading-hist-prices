[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-green?logo=GitHub)](https://github.com/JonatanSiracusa/download-historical-series)
[![Connect on LinkedIn](https://img.shields.io/badge/LinkedIn-Connect_on_LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/ajsiracusa/)
[![Read on Medium](https://img.shields.io/badge/Medium-Read_on_Medium-blueviolet?logo=medium)](https://jonatansiracusa.medium.com/)
[![View on Website](https://img.shields.io/badge/GitHub-View_on_Website-red?logo=GitHub)](https://jonatansiracusa.github.io/2024/11/14/Download-historical-series/)


# Downloading Historical Prices

This notebook allows us to download historical price series in a scalable way, including many types of prices (Adj Close, Close, High, Low, Open, Volume). Additionally, it calculates simple and continuous returns, determines volatility based on adjusted prices, and saves the data in downloadable files for offline use.


## Contact

If you have any questions about this project, feel free to contact me:

- **LinkedIn:** [linkedin.com/in/ajsiracusa](https://www.linkedin.com/in/ajsiracusa)
- **GitHub:** [github.com/JonatanSiracusa](https://github.com/JonatanSiracusa)
- **Medium:** [jonatansiracusa.medium.com](https://jonatansiracusa.medium.com/)
- **GitHub Page:** [jonatansiracusa.github.io](https://jonatansiracusa.github.io/)


## Table of Contents:

1. [Features](#Features)
2. [Requirements](#Requirements)
3. [Installation](#Installation)
4. [Usage](#Usage)
5. [Technologies](#Technologies)
6. [License](#License)


## Features

* Download financial data from `yfinance`.
* Convert data into a time series Dataframe.
* Calculates simple and continuous returns, and determines volatility based on adjusted prices.
* Export data to `.csv` and `.xlsx` files.


## Requirements

Python 3.11 or higher was used in development.


## Installation

1. Clone the repository:

```
git clone https://github.com/JonatanSiracusa/downloading-historical-prices.git
cd downloading-historical-prices
```

2. Create a virtual environment:

```
python -m venv env
```

3. Activate the virtual environment:

- On Windows:
	```
	.\env\Scripts\activate
	```
- On macOS/Linux:
	```
	source env/bin/activate
	```

4. Install libraries:

```
pip install -r requirements.txt
```

## Usage

Run the main notebook after configuring the required parameters to generate two files:

1. A dataset with the selected assets and their adjusted closing prices.
2. A dataset containing the calculated returns and volatility for the selected assets.


**Example Input**:

```
TICKERS = ["BBAR", "BMA", "VALO"]
TICKERS_YF = ["BBAR.BA", "BMA.BA", "VALO.BA"]
START_DATE = "2023-01-01"
END_DATE = ""  # Defaults to the current date if left empty
EXPORT_DATA = True
OUTPUT_NAME_1 = "adjusted_prices"
OUTPUT_NAME_2 = "returns_volatility"
```

**Expected Output**:

Two `.xlsx` files and two `.csv` files::

1. `adjusted_prices.xlsx` and `adjusted_prices.csv` – Contains the adjusted closing prices for the selected tickers.
2. `returns_volatility.xlsx` and `returns_volatility.csv` – Includes the calculated returns and volatility metrics.


## Technologies

- Python (Pandas, NumPy)
- Datetime and time Modules
- YahooFinance API


## License

This project is under the MIT License. See the `LICENSE` file for details.

--

*If you find this repository useful, give it a star ⭐ on GitHub and follow me on [LinkedIn](https://www.linkedin.com/in/ajsiracusa) and [GitHub](https://github.com/JonatanSiracusa).*


---


# Descargando Precios Históricos

Este notebook permite descargar series de precios históricos de manera escalable, incluyendo varios tipos de precios (Adj Close, Close, High, Low, Open, Volume). Además, calcula los retornos simples y continuos, determina la volatilidad basada en los precios ajustados y guarda los datos en archivos descargables para su uso sin conexión.

## Contacto

Si tenes preguntas sobre este proyecto, no dudes en contactarme a través de:

- **LinkedIn:** [linkedin.com/in/ajsiracusa](https://www.linkedin.com/in/ajsiracusa)
- **GitHub:** [github.com/JonatanSiracusa](https://github.com/JonatanSiracusa)
- **Medium:** [jonatansiracusa.medium.com](https://jonatansiracusa.medium.com/)
- **GitHub Page:** [jonatansiracusa.github.io](https://jonatansiracusa.github.io/)


## Tabla de Contenidos:

1. [Características](#Características)
2. [Requisitos](#Requisitos)
3. [Instalación](#Instalación)
4. [Uso](#Uso)
5. [Tecnologías](#Tecnologías)
6. [Licencia](#Licencia)


## Características

* Descarga datos financieros utilizando `yfinance`.
* Convierte los datos en un DataFrame de series temporales.
* Calcula retornos simples y continuos, y determina la volatilidad basada en precios ajustados.
* Exporta los datos en archivos `.xlsx` y `.csv`.

## Requisitos

Este proyecto fue desarrollado con **Python 3.11 o superior**.


## Instalación

1. Clonar el repositorio:

```
git clone https://github.com/JonatanSiracusa/downloading-historical-prices.git
cd downloading-historical-prices
```

2. Crear un entorno virtual:

```
python -m venv env
```

3. Activar el entorno virtual:

- En Windows:
	```
	.\env\Scripts\activate
	```
- En macOS/Linux:
	```
	source env/bin/activate
	```

4. Instalar librerías:

```
pip install -r requirements.txt
```


## Uso

Ejecuta el notebook principal tras configurar los parámetros necesarios para generar dos archivos:

1. Un dataset con los activos seleccionados y sus precios de cierre ajustados.
2. Un dataset con los cálculos de retornos y volatilidad de los activos seleccionados.


**Ejemplo de entrada**:

```
TICKERS = ["BBAR", "BMA", "VALO"]
TICKERS_YF = ["BBAR.BA", "BMA.BA", "VALO.BA"]
START_DATE = "2023-01-01"
END_DATE = ""  # Defaults to the current date if left empty
EXPORT_DATA = True
OUTPUT_NAME_1 = "adjusted_prices"
OUTPUT_NAME_2 = "returns_volatility"
```

**Salida esperada**:

Se generarán dos archivos `.xlsx` y dos `.csv`:

1. `adjusted_prices.xlsx` and `adjusted_prices.csv` – Contienen los precios de cierre ajustados de los activos seleccionados.
2. `returns_volatility.xlsx` and `returns_volatility.csv` – Incluyen los cálculos de retornos y métricas de volatilidad.


## Tecnologías

* Python (Pandas, NumPy)
* Módulos de fecha y tiempo (datetime, time)
* YahooFinance API


## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

--

*Si el respositorio te resulta útil, dale una estrella ⭐ en GitHub y seguime en [LinkedIn](https://www.linkedin.com/in/ajsiracusa) y [GitHub](https://github.com/JonatanSiracusa).*
