# PAC_PRJ002: Panel de Control para Huinche Minero (Mine Hoist)

## 📌 Descripción del Proyecto
Diseño de un tablero de control electromecánico para un sistema de izaje en entornos mineros. El proyecto implementa una lógica de **inversión de giro de motor trifásico pasando por paro**, garantizando la seguridad operativa frente a la inercia de cargas pesadas y protegiendo la integridad mecánica del sistema.

Desarrollado como parte del portafolio de ingeniería de **Prada Automation & Control (PAC)**.

## ⚙️ Características Técnicas y de Seguridad
El circuito ha sido diseñado bajo normativas industriales, integrando múltiples capas de seguridad:
* **Paro de Emergencia (S1):** Circuito principal de seguridad ("guillotina") que desenergiza todo el tablero de forma inmediata.
* **Enclavamiento Eléctrico Cruzado:** Uso de contactos auxiliares Normalmente Cerrados (NC 11-12) para evitar la entrada simultánea de los contactores direccionales, previniendo cortocircuitos bifásicos.
* **Enclavamiento Mecánico:** Traba física especificada en plano entre las bobinas de marcha y reversa.
* **Autonomía Operativa (Memoria):** Implementación de retención mediante contactos auxiliares Normalmente Abiertos (NA 13-14) conectados en paralelo a los pulsadores de mando, permitiendo maniobras continuas sin intervención manual sostenida.
* **Inversión Física de Fases:** Diagrama de potencia estructurado con cruce de fases (L1 a W1, L3 a U1) para el cambio de campo magnético en el motor de inducción.

## 🛠️ Herramientas Utilizadas
* **EPLAN Electric P8:** Para el diseño de detalle, ruteo inteligente, generación de referencias cruzadas y planimetría industrial (V0.1).
* **CADe SIMU:** Para la simulación dinámica, validación de la lógica de contactos y comprobación de la secuencia operativa (Marcha -> Paro -> Reversa).

## 📂 Estructura de Versiones
* **V0.1 (Actual):** Ingeniería lógica completada y simulada. Planos de potencia y control definidos.
* **V1.0 (Próximamente):** Selección de equipos comerciales (Siemens/Schneider Electric), asignación de *Part Numbers* y generación automática del listado de materiales (BOM).

---
*Diseñado por Alexander Prada | Estudiante de Ingeniería Electrónica (UNMSM)*
