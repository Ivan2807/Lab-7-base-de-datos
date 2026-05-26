# Lab-7-base-de-datos

Lab 7 – Visualización de Datos | RetailMax
Área 7: Estrategia y Expansión Comercial

Cómo levantar el ambiente
bash# 1. Clona el repositorio
git clone <url-del-repositorio>
cd lab7-retailmax

# 2. Copia los archivos SQL originales a la carpeta init/
cp DDL.sql  init/02_ddl.sql
cp DATA.sql init/03_data.sql

# 3. Levanta el ambiente
docker compose up

# 4. Abre Metabase en tu navegador
# http://localhost:3000
# Usuario: calificar@uvg.edu.gt
# Contraseña: secret123+

Credenciales de Metabase
CampoValorCorreocalificar@uvg.edu.gtContraseñasecret123+

Estructura del repositorio
.
├── docker-compose.yml        # Ambiente completo PostgreSQL + Metabase
├── init/
│   ├── 01_setup.sh           # Crea base de datos 'metabase'
│   ├── 02_ddl.sql            # Esquema RetailMax (copiar DDL.sql aquí)
│   └── 03_data.sql           # Datos RetailMax (copiar DATA.sql aquí)
├── metabase-data/            # Volumen persistido con el dashboard construido
├── informe.pdf               # Documentación de los 12 indicadores KPI
└── README.md                 # Este archivo

Dashboard
Tab 1 – Desempeño Global del Negocio
#Indicador1Ingresos Totales por Mes
2Ingresos por Región y Tienda
3Top 10 Productos por Ingreso Total
4Tasa de Conversión por Canal
5Margen Bruto Promedio por Categoría6Evolución de Pedidos por Estado
Tab 2 – Expansión Comercial
#Indicador
7Ciudades con Mayor Potencial de Expansión
8Rentabilidad por Tienda (ROI Operativo)
9Crecimiento Interanual por Tienda
10Distribución de Clientes por Segmento y Región
11Tiendas con Stock Crítico (Riesgo de Quiebre)
12Ticket Promedio por Segmento y Canal

Video de presentación
