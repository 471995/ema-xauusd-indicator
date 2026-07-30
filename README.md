# ema-xauusd-indicator
EMA multi-timeframe trading indicator for XAU/USD scalping
EMA Multi-Timeframe Trading Indicator for XAU/USD

Un indicador de trading basado en cruces de medias móviles exponenciales (EMA 10, 20, 50, 200) con lógica de stop loss mediante ATR 2.0x. Diseñado para scalping en XAU/USD en timeframes de 5 minutos.

Características

Soporta operaciones largas y cortas
Filtro de sesión optimizado para overlap Londres-Nueva York
Integración con MetaTrader 5 y almacenamiento en MySQL
Backtesting con datos históricos
Lógica de entrada basada en cruces de EMAs
Stop loss dinámico usando ATR 2.0x

Requisitos

Python 3.8 o superior
MetaTrader 5
MySQL
Librerías: pandas, numpy, ta-lib

Instalación

git clone https://github.com/471995/ema-xauusd-indicator.git
cd ema-xauusd-indicator
pip install -r requirements.txt

Configuración

Edita config.py con tus credenciales de MetaTrader 5
Configura la conexión a MySQL en database.py
Establece los parámetros de la estrategia en strategy_config.py

Uso

python backtest.py

Esto ejecuta el backtester con datos históricos y genera reportes de rentabilidad.

Estructura del Proyecto

src/ - Código principal del indicador
data/ - Scripts para descargar datos históricos
tests/ - Pruebas unitarias
docs/ - Documentación adicional
backtest.py - Script de backtesting
requirements.txt - Dependencias del proyecto

Resultados del Backtesting

XAU/USD 5 minutos: Win rate consistente en overlap Londres-Nueva York
NQ 3 minutos: Optimizado para sesiones Londres y Nueva York
Datos desde enero 2024

Licencia

MIT License - Ver LICENSE para detalles
