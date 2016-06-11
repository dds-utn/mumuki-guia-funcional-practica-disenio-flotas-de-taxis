Nos informaron que hasta el momento, la consultora anterior definió el siguiente tipo de dato (que nos pareció util mantener).

~~~haskell
data Empresa = Persona {nombre :: String, flota :: [Auto] }
~~~

Si bien no tenemos definidos la forma del auto, sabemos es necesario conocer su modelo, el año de la ultima revisión tecnica y el de su última matrícula.

Regularmente, la empresa va a necesitar realizar mantenimiento sobre sus coches. 