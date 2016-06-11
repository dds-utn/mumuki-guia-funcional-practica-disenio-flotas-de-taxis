Nos informaron que hasta el momento, la consultora anterior definió el siguiente tipo de dato (que nos pareció util mantener).

```haskell
type Anio = Int

data Empresa = Persona {nombre :: String, flota :: [Auto] }
data Auto = Auto {  modelo :: String, 
                    anioFabricacion :: Anio, 
                    anioUltimaMatricula :: Anio, 
                    anioUltimaRevisionTecnica :: Anio }
```

Regularmente, a la empresa se le puede exigir renovar la verificación técnica de sus autos, así como rematricularlos. Veamos estos requerimientos con mas detalle:

### 1. Rematriculaciones

Se trata de dada una empresa, actualizar el año de rematriculación de sus autos. Queremos: 
  * `rematricularViejos`: rematricular a todos los autos que sean viejos  (aquellos que tienen más de tres años) 
  * `rematricularRevisadosHace`: rematricular a todos los autos que hayan sido revisados hace mas de N anios

### 2. Revisiones

Queremos también también actualizar el año de revisión de los autos de la empresa:

  * `revisarViejos`: revisa los autos  viejos  (son aquellos que tienen más de tres años)
  * `revisarMalos`: revisa los autos malos. Hay varios factores que influyen para saber si un auto es malo:
    * Si en alguna parte del modelo se encuentra "daewo" o "smart".
    * Si el modelo es capicua.
    * Si el modelo es fordQu.
  * `revisarMalaTandaDeRevisiones`: hubo una mala tanda de revisiones de 2015 a los reno60, así que queremos revisarlos a estos modelos que hayan sido revisados por última vez en dicho año
  
> Escribí las funciones `rematricularRevisadosHace`, `rematricularViejos`, `revisarMalaTandaDeRevisiones`, `revisarMalos` y `revisarViejos`
