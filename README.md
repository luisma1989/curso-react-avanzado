# Preparando el entorno de desarrollo
- Hemos cclonado el repositorio e instalado webpack.
- Hemos instalado las dependencias de React y babel.
- Configuracióin de linter, extensiones y deploy con Now

# Styled components
- Estilos css en el JS (https://www.styled-components.com/docs/api)
- Crear los estilos globales de la aplicación:
  import { createGlobalStyle } from 'styled-components'
- react-icons (https://react-icons.netlify.com/#/) para darle una propuesta visual mucho más amigable a nuestro proyecto con íconos como Font Awesome, Ionicons, Material Design Icons y mucho más que podremos usar.
- maketext.io para crear nuestro logo y descargarlo en SVG. Posteriormente a esto utilizaremos SVGOMG para optimizar nuestro logo y tener una mejor versión para usarla en nuestro proyecto. Luego para convertir nuestro logo svg en un componente utilizaremos SVGR. (https://www.smooth-code.com/open-source/svgr/playground/)

# Hooks
¿Qué son los Hooks?
Funciones que nos permiten acceder a casi todas las características de react desde componentes funcionales.
Las características que por ahora no se pueden acceder son:
getSnaphotBeforeUpdate
componentDidCatch
🔧
Los hooks principales son
- useState: para añadir un estado local en el componente
- useEffect: permite ejecutar una funcion cada vez que rendericemos nuestro componente
- useContext: permite acceder a context API para obtener valores que se utilizaran en toda la aplicacion de forma global, sin necesidad de pasarla por las props.(https://es.reactjs.org/docs/hooks-reference.html#usecontext)
- useReducer: Una alternativa a useState. Acepta un reducer de tipo (state, action) => newState y devuelve el estado actual emparejado con un método dispatch. (Si está familiarizado con Redux, ya sabe cómo funciona). (https://es.reactjs.org/docs/hooks-reference.html#usereducer)
- useCallback: https://es.reactjs.org/docs/hooks-reference.html#usecallback
- useMemo: https://es.reactjs.org/docs/hooks-reference.html#usememo
- useRef: https://es.reactjs.org/docs/hooks-reference.html#useref
- useImperativehandle: https://es.reactjs.org/docs/hooks-reference.html#useimperativehandle
- useLayoutEffect: https://es.reactjs.org/docs/hooks-reference.html#uselayouteffect
- useDebugValue: https://es.reactjs.org/docs/hooks-reference.html#usedebugvalue

# ¿Qué es GraphQL?

En un lenguaje creado por facebook que nos permite recuperar los datos
que justamente necesitamos en nuestra aplicación. Nos permite definir los tipos de datos. Optimizará los recursos de nuestra red y los resultados serán predecibles al tener que solicitar los datos.

GraphQl no sustituye a REST.

GraphQl es:
- Lenguaje
- Un sólo endPoint
- Fetching justo
- Conexión a otras APIs

REST es:
- Aquitectura
- Múltiples endpoints
- Over y underfetching
- Conexión directa con base de datos

React Apollo es un cliente que nos va a permitir conectarnos a un servidor GraphQL.

Vamos a instalar npm i apollo-boost, una utilidad que nos permite inicializar nuestra conexión con un servidor de Apollo muy rápidamente y sin configuración, necesitaremos npm i react-apollo el cual es la integración de Apollo con React y finalmente npm i graphql.



RenderProps (https://es.reactjs.org/docs/render-props.html)

El término “render prop” se refiere a una técnica para compartir código entre componentes en React utilizando una propiedad cuyo valor es una función.

Un componente con una render prop toma una función que devuelve un elemento de React y lo llama en lugar de implementar su propia lógica de representació

HOC
