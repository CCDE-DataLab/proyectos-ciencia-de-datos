# 📊 Área de Proyectos: Ciencia de Datos
**Círculo de Ciencia de Datos y Econometría (CCDE) - UNMSM**

> *"De la teoría en el aula al modelo en producción."*

Bienvenido al repositorio oficial del **Área de Proyectos de Ciencia de Datos** del CCDE. Este espacio funciona como nuestro "Laboratorio Core", donde alojamos el código fuente, los datasets y la documentación técnica de todas nuestras iniciativas aplicadas.

## 🎯 Nuestro Propósito
El objetivo de este repositorio no es la simple experimentación académica, sino la **simulación de entornos corporativos y de políticas públicas reales**. Desarrollamos proyectos estructurados (de extremo a extremo) orientados a resolver problemas de negocio mediante Machine Learning, Inteligencia Artificial y flujos de trabajo MLOps.

Priorizamos:
- **Código Limpio y Eficiente:** Evitamos los notebooks desordenados. Promovemos el uso de funciones, clases y programación orientada a objetos (POO).
- **Prevención de Fuga de Datos:** Uso riguroso de `Pipelines` y validaciones cruzadas.
- **Enfoque de Negocio:** Cada modelo debe traducirse en *insights* accionables.

## 🗂️ Estructura del Repositorio
Cada iniciativa se desarrolla en una carpeta independiente con su propio entorno, datasets y documentación.

| Directorio | Descripción | Estado | Herramientas Clave |
| :--- | :--- | :---: | :--- |
| `01_proy_cd_credit_scoring/` | Sistema de clasificación de riesgo crediticio comparando Regresión Logística (WoE) vs. Random Forest. | 🟢 Completado | `Scikit-Learn`, `Optuna`, `MLOps` |
| `02_prediccion_demanda/` | *(Próximamente)* Modelo de proyección de demanda para sector retail. | ⚪ Planificado | `XGBoost`, `Pandas` |
| `03_pricing_inmobiliario/` | *(Próximamente)* Algoritmo de valuación de activos utilizando datos geolocalizados. | ⚪ Planificado | `GeoPandas`, `ML` |

## 🛠️ Stack Tecnológico
Nuestro equipo trabaja principalmente con el siguiente ecosistema:
- **Manipulación de Datos:** `Pandas`, `NumPy`
- **Machine Learning & MLOps:** `Scikit-Learn`, `XGBoost`, `Joblib`
- **Optimización:** `Optuna`
- **Visualización:** `Matplotlib`, `Seaborn`

## 👥 Metodología de Trabajo (Para Miembros)
Si eres miembro del CCDE y vas a colaborar en este repositorio, seguimos el flujo de trabajo ágil estándar de la industria tecnológica:
1. **Nunca trabajes en la rama `main`:** Crea una rama (`branch`) con tu nombre o el de tu tarea (ej. `feat/limpieza-datos-credito`).
2. **Control de Versiones:** Realiza *commits* descriptivos detallando qué cambios hiciste.
3. **Revisión de Código:** Sube tus cambios y abre un *Pull Request* (PR) para que los Directores del área validen la eficiencia de tu código antes de fusionarlo al proyecto principal.

---
**¿Quieres saber más de nosotros?**  
🔗 [Visita nuestra página en LinkedIn](#) *(Nota: Colocar aquí el link cuando la creen)*  
✉️ Contacto: ccde.unmsm@gmail.com
├── credit_scoring_pipeline.joblib  # Pipeline final serializado (Listo para Producción)
└── README.md                       # Documentación del proyecto
