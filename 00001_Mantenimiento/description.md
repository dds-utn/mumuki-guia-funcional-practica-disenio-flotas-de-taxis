Nos informaron que hasta el momento, la consultora anterior definió el siguiente tipo de dato (que nos pareció util mantener).

~~~haskell
data Empresa = Persona {nombre :: String, flota :: [Auto] }
~~~

Si bien no tenemos definidos la forma del auto, sabemos es necesario conocer su modelo, el año de la ultima revisión tecnica y el de su última matrícula.

Regularmente, a la empresa se le puede exigir renovar la verificación técnica de:

  * Los autos viejos (son aquellos que tienen más de tres años).
  
  * Sobre los autos malos. Este criterio ya es un poquito más complejo. Hay varios factores que influyen para saber si un auto es malo. Algunos, pero no todos, pueden ser:
    * Si fué fabricado en el 2000.
    * Si en alguna parte del modelo se encuentra "daewo" o "smart".
    * Si el modelo es capicua.
    * Si no hay números.
    * Si hay más de 10 números.
    

  * Todos los modelos que comiencen con "FORD" y cuya última revisión sea en el 2015 (nos enteramos que hubieron muchas coimas).
  
De la misma forma, aveces va a ser necesario rematricular a:
  * Todos los autos.
  * Los que sean autos viejos.
  * Los que hayan sido revisados hace más de N años.
  

> Definir rematricularTodos, rematricularViejos y rematricularRevisadosHaceMasDe


_Puede llegar a ser util la función isInfixOf, cuya firma es_

~~~haskell
isInfixOf :: Eq a => [a] -> [a] -> Bool
> isInfixOf "Haskell" "I really like Haskell
 True
~~~