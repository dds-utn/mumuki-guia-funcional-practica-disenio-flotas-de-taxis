Nos informaron que hasta el momento, la consultora anterior definió el siguiente tipo de dato (que nos pareció util mantener).

~~~
data Empresa = Persona {nombre :: String, flota :: [Auto] }
~~~
{: .language-haskell}

Si bien no tenemos definidos la forma del auto, sabemos que en nuestro sistema estos cuentan con el modelo, el año de su ultima revisión tecnica y el de su última matrícula.