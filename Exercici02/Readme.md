2. Que creieu que és millor mostrar els logs per exemple a la terminal durant l'execució del programa o bolcar-los en un fitxer de text?

La elección de mostrar los registros en la terminal o guardarlos en un archivo depende de las necesidades específicas de la aplicación. Mostrar los registros en la terminal es útil durante el desarrollo, ya que permite observar en tiempo real los eventos que ocurren mientras el programa está en ejecución. Esto facilita la depuración y el monitoreo instantáneo del comportamiento del programa. Sin embargo, los registros mostrados en la terminal se pierden cuando el programa termina, lo que puede ser problemático si es necesario consultarlos más tarde o realizar un análisis posterior.

Guardar los registros en un archivo ofrece la ventaja de conservarlos, lo que permite hacer un seguimiento a largo plazo, revisar errores pasados o realizar auditorías. Además, los archivos de registro pueden ser analizados o procesados con herramientas externas. Sin embargo, esta opción requiere algo más de configuración, especialmente si la aplicación genera una gran cantidad de datos, lo que obliga a gestionar el tamaño de los archivos y a configurar rotación de logs.

Una práctica común es utilizar ambos métodos: mostrar los registros importantes en la terminal durante la ejecución para visibilidad inmediata, y guardar los registros más detallados en archivos para consultas o análisis posteriores. Esto asegura que se tenga acceso a la información en tiempo real mientras se mantiene un archivo completo para un seguimiento más exhaustivo.

3. Omple la següent taula amb expmple, avantantges, i desavantatges de les següents maneres de fer logs:


|        Mètode       |       Exemple      |      Avantatges     |      Desavantatges     |
| ------------------- | ------------------ | ------------------- | ---------------------- |
| **Configuració      | `logging.basicConfig()`
| per defecte**       | `logging.basicConfig()` | Ràpid i senzill. No requereix configuració addicional. | Menys flexibilitat i configuracions globals. |
| **Instanciant un logger manualment** | `logger = logging.getLogger('my_logger')` | Control detallat de la configuració, múltiples loggers. | Més codi i configuració, difícil en aplicacions grans. |
| **Instanciant un logger des de fitxer** | `logging.config.fileConfig('logging.conf')` | Separació entre codi i configuració, fàcil de gestionar configuracions complexes. | Requereix fitxer extern, pot ser difícil de mantenir. |

