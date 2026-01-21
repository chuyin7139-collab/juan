 # Gestor de tareas
 <img width="310" height="163" alt="descarga" src="https://github.com/user-attachments/assets/54fb1971-edee-4a7c-bb41-72df6bb3c77c" />
 
# Autor
juan pablo gloria villanueva

## 1. Contexto y Justificación (El "Por qué")

### Problemática:
Los usuarios de gestores de tareas tradicionales carecen de asistencia inteligente y proactiva. Las aplicaciones actuales solo registran y muestran tareas, pero no ayudan a priorizarlas, estimar tiempos, sugerir desgloses automáticos de tareas complejas ni alertar sobre sobrecarga de trabajo. Esto resulta en una gestión pasiva e ineficiente del tiempo
 
### Valor Agregado del Framework (React + IA):
React permite una interfaz reactiva y en tiempo real que se actualiza instantáneamente cuando la IA sugiere cambios, reordena tareas o alerta al usuario. La combinación de un estado dinámico con llamadas asíncronas a APIs de IA (como OpenAI) permite crear una experiencia interactiva y adaptativa, imposible con HTML/CSS/JS tradicional.

## 2. Requerimientos Funcionales (El "Qué hace")

1. RF1: Agregar tarea con título, descripción y prioridad (alta/media/baja).
2. RF2: Marcar/desmarcar tarea como completada (toggle visual inmediato).
3. RF3: IA - Sugerir desglose automático** de tareas complejas en subtareas.
4. RF4: IA - Alertar sobre tareas atrasadas** o próximas a vencer (con base en fecha límite).
5. RF5: IA - Recomendar orden de ejecución** basado en prioridad y tiempo estimado.

## 3. Requerimientos No Funcionales (El "Cómo funciona")

| Categoría       | Especificación Técnica                                                                 |
|-----------------|---------------------------------------------------------------------------------------|
| **Adaptabilidad** | Diseño Responsive con **Tailwind CSS + Flexbox** para móviles y escritorio.           |
| **Rendimiento**   | **Lazy Loading** de módulos de IA + **Debouncing** en búsquedas inteligentes.         |
| **Persistencia**  | **LocalStorage** + **IndexedDB** para caché de sugerencias de IA y tareas offline.    |
| **Accesibilidad** | Roles ARIA + **modo alto contraste** para alertas visuales de IA.                    |
| **IA/API**        | Consumo de **OpenAI API** (o similar) con manejo seguro de API keys desde backend.   |

## 4. Tecnologías y Herramientas del Ecosistema

- **Framework Principal**: React con **TypeScript** (para tipado seguro en respuestas de IA).
- **Manejo de Estado Global**: **Zustand** (ligero y rápido, ideal para estado complejo de tareas + sugerencias de IA).
- **Consumo de Datos**: **Axios** + **React Query** para manejo eficiente de llamadas a API de IA y caching.
- **IA/Backend**: **OpenAI API** (GPT-4) para análisis de tareas + **backend en Node.js/Express** como proxy de seguridad.
- **Estilizado**: **Tailwind CSS** + **Headless UI** para componentes accesibles.
- **Despliegue**: **Vercel** (frontend) + **Railway** (backend proxy para IA).


 

