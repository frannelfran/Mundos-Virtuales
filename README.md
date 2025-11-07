 Paula Díaz Jorge, Franco Alla, Javier Gómez Alayón

# **SEMINARIO**

## Mundos virtuales: Introducción a la programación de gráficos 3D

<img width="1085" height="1084" alt="image" src="https://github.com/user-attachments/assets/55b16397-262a-4a7a-b4d0-5d8fc0210a20" />

## **Índice** {#índice}

[**Índice	2**](#índice)

[1\. Qué funciones se pueden usar en los scripts de Unity para llevar a cabo traslaciones, rotaciones y escalados.	4](#qué-funciones-se-pueden-usar-en-los-scripts-de-unity-para-llevar-a-cabo-traslaciones,-rotaciones-y-escalados.)

[2\. ¿Cómo trasladarías la cámara 2 metros en cada uno de los ejes y luego la rotas 30º alrededor del eje Y?. Rota la cámara alrededor del eje Y 30ª y desplázate 2 metros en cada uno de los ejes. ¿Obtendrías el mismo resultado en ambos casos?. Justifica el resultado.	4](#¿cómo-trasladarías-la-cámara-2-metros-en-cada-uno-de-los-ejes-y-luego-la-rotas-30º-alrededor-del-eje-y?.-rota-la-cámara-alrededor-del-eje-y-30ª-y-desplázate-2-metros-en-cada-uno-de-los-ejes.-¿obtendrías-el-mismo-resultado-en-ambos-casos?.-justifica-el-resultado.)

[a. Primero trasladar y luego rotar	4](#primero-trasladar-y-luego-rotar)

[b. Rotar primero y luego trasladar	4](#rotar-primero-y-luego-trasladar)

[3\. Sitúa la esfera de radio 1 en el campo de visión de la cámara y configura un volumen de vista que la recorte parcialmente.	5](#sitúa-la-esfera-de-radio-1-en-el-campo-de-visión-de-la-cámara-y-configura-un-volumen-de-vista-que-la-recorte-parcialmente.)

[4\. Sitúa la esfera de radio 1 en el campo de visión de la cámara y configura el volumen de vista para que la deje fuera de la vista.	6](#sitúa-la-esfera-de-radio-1-en-el-campo-de-visión-de-la-cámara-y-configura-el-volumen-de-vista-para-que-la-deje-fuera-de-la-vista.)

[5\. Cómo puedes aumentar el ángulo de la cámara. Qué efecto tiene disminuir el ángulo de la cámara.	6](#cómo-puedes-aumentar-el-ángulo-de-la-cámara.-qué-efecto-tiene-disminuir-el-ángulo-de-la-cámara.)

[6\. Es correcta la siguiente afirmación: Para realizar la proyección al espacio 2D, en el inspector de la cámara, cambiaremos el valor de projection, asignándole el valor de orthographic	7](#es-correcta-la-siguiente-afirmación:-para-realizar-la-proyección-al-espacio-2d,-en-el-inspector-de-la-cámara,-cambiaremos-el-valor-de-projection,-asignándole-el-valor-de-orthographic)

[7\. Especifica las rotaciones que se han indicado en los ejercicios previos con la utilidad quaternion.	7](#especifica-las-rotaciones-que-se-han-indicado-en-los-ejercicios-previos-con-la-utilidad-quaternion.)

[8\. ¿Como puedes averiguar la matriz de proyección en perspectiva que se ha usado para proyectar la escena al último frame renderizado?	7](#¿como-puedes-averiguar-la-matriz-de-proyección-en-perspectiva-que-se-ha-usado-para-proyectar-la-escena-al-último-frame-renderizado?)

[9\. ¿Cómo puedes averiguar la matriz de proyección en perspectiva ortográfica que se ha usado para proyectar la escena al último frame renderizado?	8](#¿cómo-puedes-averiguar-la-matriz-de-proyección-en-perspectiva-ortográfica-que-se-ha-usado-para-proyectar-la-escena-al-último-frame-renderizado?)

[10\. ¿Cómo puedes obtener la matriz de transformación entre el sistema de coordenadas local y el mundial?	8](#¿cómo-puedes-obtener-la-matriz-de-transformación-entre-el-sistema-de-coordenadas-local-y-el-mundial?)

[11\. Cómo puedes obtener la matriz para cambiar al sistema de referencia de vista	9](#cómo-puedes-obtener-la-matriz-para-cambiar-al-sistema-de-referencia-de-vista)

[12\. Especifica la matriz de la proyección usado en un instante de la ejecución del ejercicio 1 de la práctica 1\.	9](#especifica-la-matriz-de-la-proyección-usado-en-un-instante-de-la-ejecución-del-ejercicio-1-de-la-práctica-1.)

[13\. Especifica la matriz de modelo y vista de la escena del ejercicio 1 de la práctica 1\.	10](#especifica-la-matriz-de-modelo-y-vista-de-la-escena-del-ejercicio-1-de-la-práctica-1.)

[14\. Aplica una rotación en el start de uno de los objetos de la escena y muestra la matriz de cambio al sistema de referencias mundial.	11](#aplica-una-rotación-en-el-start-de-uno-de-los-objetos-de-la-escena-y-muestra-la-matriz-de-cambio-al-sistema-de-referencias-mundial.)

[15\. ¿Cómo puedes calcular las coordenadas del sistema de referencia de un objeto con las siguientes propiedades del Transform:?:	11](#¿cómo-puedes-calcular-las-coordenadas-del-sistema-de-referencia-de-un-objeto-con-las-siguientes-propiedades-del-transform:?:)

[Position (3, 1, 1), Rotation (45, 0, 45\)	11](#position-\(3,-1,-1\),-rotation-\(45,-0,-45\))

[16\. Crea una escena en Unity con los siguientes elementos: cámara principal, plano base (como suelo) y tres cubos de distinto color (rojo, verde, azul) colocados en posiciones distintas en el espacio. Realiza un pequeño script de depuración adjunto a la cámara que permita visualizar en consola o en pantalla las matrices de transformación (Model, View, Projection) y sus resultados sobre un vértice de cada cubo.	12](#crea-una-escena-en-unity-con-los-siguientes-elementos:-cámara-principal,-plano-base-\(como-suelo\)-y-tres-cubos-de-distinto-color-\(rojo,-verde,-azul\)-colocados-en-posiciones-distintas-en-el-espacio.-realiza-un-pequeño-script-de-depuración-adjunto-a-la-cámara-que-permita-visualizar-en-consola-o-en-pantalla-las-matrices-de-transformación-\(model,-view,-projection\)-y-sus-resultados-sobre-un-vértice-de-cada-cubo.)

[17\. Dibujar en un programa de dibujo el recorrido de las coordenadas de un vértice específico del cubo rojo:	14](#dibujar-en-un-programa-de-dibujo-el-recorrido-de-las-coordenadas-de-un-vértice-específico-del-cubo-rojo:)

[Local → World → Camera/View → Clip → NDC → Viewport. Indicar cómo cambia su valor en cada espacio. Aplicar la transformación manualmente a un punto (por ejemplo, el vértice (0.5, 0.5, 0.5)) y registrar los resultados paso a paso.	14](#local-→-world-→-camera/view-→-clip-→-ndc-→-viewport.-indicar-cómo-cambia-su-valor-en-cada-espacio.-aplicar-la-transformación-manualmente-a-un-punto-\(por-ejemplo,-el-vértice-\(0.5,-0.5,-0.5\)\)-y-registrar-los-resultados-paso-a-paso.)

[18\. Mover o rotar uno de los cubos y mostrar cómo cambian los valores de su matriz de modelo. Rotar la cámara y mostrar cómo se modifica la matriz de vista. Cambiar entre proyección ortográfica y perspectiva y comparar las diferencias numéricas en la matriz de proyección.	16](#mover-o-rotar-uno-de-los-cubos-y-mostrar-cómo-cambian-los-valores-de-su-matriz-de-modelo.-rotar-la-cámara-y-mostrar-cómo-se-modifica-la-matriz-de-vista.-cambiar-entre-proyección-ortográfica-y-perspectiva-y-comparar-las-diferencias-numéricas-en-la-matriz-de-proyección.)

## 

1. ### **Qué funciones se pueden usar en los scripts de Unity para llevar a cabo traslaciones, rotaciones y escalados.** {#qué-funciones-se-pueden-usar-en-los-scripts-de-unity-para-llevar-a-cabo-traslaciones,-rotaciones-y-escalados.}

* Transform.**translate** → Para realizar translaciones  
* Transform.**rotate** → Para realizar rotaciones  
* Transform.**localScale** → Para escalar (Cambiar el tamaño del objeto)

2. ### **¿Cómo trasladarías la cámara 2 metros en cada uno de los ejes y luego la rotas 30º alrededor del eje Y?. Rota la cámara alrededor del eje Y 30ª y desplázate 2 metros en cada uno de los ejes. ¿Obtendrías el mismo resultado en ambos casos?. Justifica el resultado.** {#¿cómo-trasladarías-la-cámara-2-metros-en-cada-uno-de-los-ejes-y-luego-la-rotas-30º-alrededor-del-eje-y?.-rota-la-cámara-alrededor-del-eje-y-30ª-y-desplázate-2-metros-en-cada-uno-de-los-ejes.-¿obtendrías-el-mismo-resultado-en-ambos-casos?.-justifica-el-resultado.}

   1. #### Primero trasladar y luego rotar {#primero-trasladar-y-luego-rotar}

```c#
// Trasladar 2 metros en cada eje
transform.Translate(new Vector3(2, 2, 2), Space.Self);
// Rotar 30° alrededor del eje Y
transform.Rotate(0, 30, 0);
```

El resultado de este código es que la cámara primero se mueve a la posición (2,2,2) y luego se rota los 30 grados, esto no afecta en hacia dónde se mueve ya que ya ha realizado el desplazamiento.

2. #### Rotar primero y luego trasladar {#rotar-primero-y-luego-trasladar}

```c#
// Rotar 30° alrededor del eje Y
transform.Rotate(0, 30, 0);
// Trasladar 2 metros en cada eje local
transform.Translate(new Vector3(2, 2, 2), Space.Self);
```

El resultado para este caso es diferente al anterior, ya que si al principio rotamos el objeto 30 grados, este cambia su eje de referencia, por lo que el desplazamiento se realiza en base a su nueva orientación.

3. ### **Sitúa la esfera de radio 1 en el campo de visión de la cámara y configura un volumen de vista que la recorte parcialmente.** {#sitúa-la-esfera-de-radio-1-en-el-campo-de-visión-de-la-cámara-y-configura-un-volumen-de-vista-que-la-recorte-parcialmente.}

   Para este ejercicio hemos situado la cámara en el origen (0, 0, 0\)  y la esfera a 5 de distancia (0, 0, 5\. Se ajusta el plano cercano (`nearClipPlane`) de la cámara de forma que corte el volumen de la esfera  y para que se viese la esfera como en la imagen, el volumen de vista se tuvo que poner de la siguiente manera:

```c#
camara.transform.rotation = Quaternion.identity;
camara.nearClipPlane = 4.5f; // Recorta parte frontal de la esfera
camara.farClipPlane = 100f; // Mantiene el plano alejado
camara.fieldOfView = 60f; // Ajusta el campo de visión
```

<img width="794" height="406" alt="image" src="https://github.com/user-attachments/assets/f88812aa-e26a-4888-877a-3230f838b409" />


4. ### **Sitúa la esfera de radio 1 en el campo de visión de la cámara y configura el volumen de vista para que la deje fuera de la vista.** {#sitúa-la-esfera-de-radio-1-en-el-campo-de-visión-de-la-cámara-y-configura-el-volumen-de-vista-para-que-la-deje-fuera-de-la-vista.}

En este caso, la cámara se encuentra en el origen (0, 0, 0\) mirando hacia el eje Z positivo, y la esfera está situada en (0, 0, 0.5) con radio 1\. Al establecer:

```c#
camara.transform.rotation = Quaternion.identity;
camara.nearClipPlane = 1.0f;  // Empieza a renderizar desde z = 1
     camara.farClipPlane = 100f;
     camara.fieldOfView = 60f;
```

El plano cercano de la cámara comienza en z \= 1, por lo que toda la esfera queda antes de ese plano y, en consecuencia, fuera del volumen de vista, no siendo visible en la escena.

<img width="790" height="391" alt="image" src="https://github.com/user-attachments/assets/323bfaaf-7e4f-4759-a75d-e519b1894360" />


5. ### **Cómo puedes aumentar el ángulo de la cámara. Qué efecto tiene disminuir el ángulo de la cámara.** {#cómo-puedes-aumentar-el-ángulo-de-la-cámara.-qué-efecto-tiene-disminuir-el-ángulo-de-la-cámara.}

   El ángulo de la cámara se puede modificar con fieldOfView de la siguiente manera:

```c#
Camera.main.fieldOfView = 90f;
```

		Con esto lo que se está haciendo es aumentar el ángulo de visión de la cámara. 

6. ### **Es correcta la siguiente afirmación: Para realizar la proyección al espacio 2D, en el inspector de la cámara, cambiaremos el valor de projection, asignándole el valor de orthographic** {#es-correcta-la-siguiente-afirmación:-para-realizar-la-proyección-al-espacio-2d,-en-el-inspector-de-la-cámara,-cambiaremos-el-valor-de-projection,-asignándole-el-valor-de-orthographic}

   Si, ya que en Unity para realizar una proyección al espacio 2D se tiene que cambiar el tipo de proyección de la cámara a Orthographic, esto se hace para eliminar la perspectiva, lo que es lo mismo, hacer que los objetos no se deformen con la distancia.

7. ###  **Especifica las rotaciones que se han indicado en los ejercicios previos con la utilidad quaternion.** {#especifica-las-rotaciones-que-se-han-indicado-en-los-ejercicios-previos-con-la-utilidad-quaternion.}

   Usando cuaterniones, las rotaciones que se han indicado en los ejercicios anteriores serían:

```c#
// Rotar 30° alrededor del eje Y
transform.rotation = Quaternion.Euler(0, 30, 0);
```

   

8. ### **¿Como puedes averiguar la matriz de proyección en perspectiva que se ha usado para proyectar la escena al último frame renderizado?** {#¿como-puedes-averiguar-la-matriz-de-proyección-en-perspectiva-que-se-ha-usado-para-proyectar-la-escena-al-último-frame-renderizado?}

En Unity, la matriz de proyección en perspectiva se obtiene directamente desde la cámara activa.

```c#
Matrix4x4 projectionMatrix = Camera.main.projectionMatrix;
```

### 

9. ### **¿Cómo puedes averiguar la matriz de proyección en perspectiva ortográfica que se ha usado para proyectar la escena al último frame renderizado?** {#¿cómo-puedes-averiguar-la-matriz-de-proyección-en-perspectiva-ortográfica-que-se-ha-usado-para-proyectar-la-escena-al-último-frame-renderizado?}

Si la cámara está en modo orthographic, la obtienes de la misma forma:

```c#
Matrix4x4 projectionMatrix = Camera.main.projectionMatrix;
```

En este caso, la matriz no aplica perspectiva, es decir, los objetos no disminuyen de tamaño con la distancia.

Se puede comprobar si la cámara es ortográfica de la siguiente manera:

```c#
if (Camera.main.orthographic)
	...
```

10. ### **¿Cómo puedes obtener la matriz de transformación entre el sistema de coordenadas local y el mundial?** {#¿cómo-puedes-obtener-la-matriz-de-transformación-entre-el-sistema-de-coordenadas-local-y-el-mundial?}

    Del sistema de coordenadas local al mundial se hace con la propiedad `localToWorldMatrix` de cualquier objeto `Transform`:

```c#
Matrix4x4 localToWorld = transform.localToWorldMatrix;
```

		De mundial a local es de la siguiente manera:

```c#
Matrix4x4 worldToLocal = transform.worldToLocalMatrix;
```

11. ###  **Cómo puedes obtener la matriz para cambiar al sistema de referencia de vista** {#cómo-puedes-obtener-la-matriz-para-cambiar-al-sistema-de-referencia-de-vista}

La matriz de vista transforma las coordenadas del sistema mundial al sistema de referencia de la cámara. Puede obtenerse de dos maneras equivalentes:

```c#
Matrix4x4 viewMatrix = Camera.main.worldToCameraMatrix;
Matrix4x4 viewMatrix = Camera.main.transform.worldToLocalMatrix;
```

12. ###  **Especifica la matriz de la proyección usado en un instante de la ejecución del ejercicio 1 de la práctica 1\.** {#especifica-la-matriz-de-la-proyección-usado-en-un-instante-de-la-ejecución-del-ejercicio-1-de-la-práctica-1.}

Con los valores de la cámara:

* fieldOfView \= 60°  
* aspect \= 16/9  
* nearClipPlane \= 0.3f  
* farClipPlane \= 1000f

La matriz de proyección perspectiva es:

```c#
[1.03, 0.00, 0.00, 0.00]
[0.00, 1.83, 0.00, 0.00]
[0.00, 0.00, -1.00, -0.60]
[0.00, 0.00, -1.00, 0.00]
```

### 

13. ### **Especifica la matriz de modelo y vista de la escena del ejercicio 1 de la práctica 1\.** {#especifica-la-matriz-de-modelo-y-vista-de-la-escena-del-ejercicio-1-de-la-práctica-1.}

    1. Matriz de modelo:

       <img width="632" height="179" alt="image" src="https://github.com/user-attachments/assets/8bccf467-6031-4a6f-b160-2b1418b11e95" />

    2. Matriz de vista:

		<img width="636" height="182" alt="image" src="https://github.com/user-attachments/assets/9abb7c20-e3e7-4168-a0dd-cea4f400b29d" />

14. ### **Aplica una rotación en el start de uno de los objetos de la escena y muestra la matriz de cambio al sistema de referencias mundial.** {#aplica-una-rotación-en-el-start-de-uno-de-los-objetos-de-la-escena-y-muestra-la-matriz-de-cambio-al-sistema-de-referencias-mundial.}

	<img width="637" height="139" alt="image" src="https://github.com/user-attachments/assets/8ccb9431-fb04-4f32-9672-5f7547b988a1" />

15. ### **¿Cómo puedes calcular las coordenadas del sistema de referencia de un objeto con las siguientes propiedades del Transform:?:**  {#¿cómo-puedes-calcular-las-coordenadas-del-sistema-de-referencia-de-un-objeto-con-las-siguientes-propiedades-del-transform:?:}

### **Position (3, 1, 1), Rotation (45, 0, 45\)** {#position-(3,-1,-1),-rotation-(45,-0,-45)}

Puedes utilizar la funcionalidad que te dá Unity para crear una matriz en base a una posición, una rotación y una escala de la siguiente manera:

```c#
Matrix4x4 modelMatrix = Matrix4x4.TRS(
    new Vector3(3, 1, 1),
    Quaternion.Euler(45, 0, 45),
    Vector3.one
);
Debug.Log(modelMatrix);
```

	

16. ### **Crea una escena en Unity con los siguientes elementos: cámara principal, plano base (como suelo) y tres cubos de distinto color (rojo, verde, azul) colocados en posiciones distintas en el espacio. Realiza un pequeño script de depuración adjunto a la cámara que permita visualizar en consola o en pantalla las matrices de transformación (Model, View, Projection) y sus resultados sobre un vértice de cada cubo.** {#crea-una-escena-en-unity-con-los-siguientes-elementos:-cámara-principal,-plano-base-(como-suelo)-y-tres-cubos-de-distinto-color-(rojo,-verde,-azul)-colocados-en-posiciones-distintas-en-el-espacio.-realiza-un-pequeño-script-de-depuración-adjunto-a-la-cámara-que-permita-visualizar-en-consola-o-en-pantalla-las-matrices-de-transformación-(model,-view,-projection)-y-sus-resultados-sobre-un-vértice-de-cada-cubo.}

Para responder esta pregunta en vez de poner 9 imágenes voy a poner el código que he utilizado para obtener las respuestas y además una imagen de todos los logs.

```c#
// Transforms de los cubos en la escena
    public Transform cuboRojo;
    public Transform cuboVerde;
    public Transform cuboAzul;
    // Vértice local a transformar (esquina del cubo)
    public Vector3 verticeLocal = new Vector3(0.5f, 0.5f, 0.5f);
    void Start()
    {
        ImprimirMatrices(cuboRojo, "Cubo Rojo");
        ImprimirMatrices(cuboVerde, "Cubo Verde");
        ImprimirMatrices(cuboAzul, "Cubo Azul");
    }
    void ImprimirMatrices(Transform objeto, string nombre)
    {
        Vector3 posicionMundialVertice = objeto.position + verticeLocal; // Cojo el vértice del cubo.
        Matrix4x4 matrizModelo = objeto.localToWorldMatrix;
        Matrix4x4 matrizVista = Camera.main.worldToCameraMatrix;
        Matrix4x4 matrizProyeccion = Camera.main.projectionMatrix;
        Debug.Log($"------ {nombre} ------");
        Debug.Log("Matriz de Modelo:\n" + matrizModelo);
        Debug.Log("Matriz de Vista:\n" + matrizVista);
        Debug.Log("Matriz de Proyección:\n" + matrizProyeccion);
    }

```

<img width="636" height="1218" alt="image" src="https://github.com/user-attachments/assets/6c7a6fb2-37d8-4bfd-8d56-0987f4f72f59" />

17. ### **Dibujar en un programa de dibujo el recorrido de las coordenadas de un vértice específico del cubo rojo:** {#dibujar-en-un-programa-de-dibujo-el-recorrido-de-las-coordenadas-de-un-vértice-específico-del-cubo-rojo:}

    ### **Local → World → Camera/View → Clip → NDC → Viewport. Indicar cómo cambia su valor en cada espacio. Aplicar la transformación manualmente a un punto (por ejemplo, el vértice (0.5, 0.5, 0.5)) y registrar los resultados paso a paso.** {#local-→-world-→-camera/view-→-clip-→-ndc-→-viewport.-indicar-cómo-cambia-su-valor-en-cada-espacio.-aplicar-la-transformación-manualmente-a-un-punto-(por-ejemplo,-el-vértice-(0.5,-0.5,-0.5))-y-registrar-los-resultados-paso-a-paso.}

<img width="1226" height="446" alt="image" src="https://github.com/user-attachments/assets/9ecfb928-411d-4e95-b7ad-b80b2497664b" />

El vértice local (0.5, 0.5, 0.5, 1\) se transforma por el modelo M (aquí asumido identidad) manteniéndose como World \= (0.5, 0.5, 0.5, 1); la matriz de vista lleva ese punto al espacio cámara como Eye \= (1.683012702, 0.5, 2.183012702, 1); la matriz de proyección produce el vector de clip Clip \= (1.683012702, −0.866025405, −7.78750391, −7.183012702), cuyo componente w (w\_clip \= −7.183012702) controla la perspectiva; al dividir por w se obtiene NDC \= (x\_ndc, y\_ndc, z\_ndc) \= (−0.22827792, 1.02056576, 1.08415566), valores fuera del rango típico \[−1,1\] en y y z que indican que el vértice queda fuera del frustum; finalmente, mapeando NDC a pantalla con width \= 740.85 px y height \= 605.11 px resulta x\_px ≈ 285.9 px y y\_px ≈ −6.2 px (origen superior), por lo que la proyección coloca el punto fuera del área visible; la causa principal de los grandes cambios numéricos es la multiplicación por la matriz de proyección seguida de la división no lineal por w, que amplifica o invierte componentes según la profundidad y las convenciones de cámara.

18. ### **Mover o rotar uno de los cubos y mostrar cómo cambian los valores de su matriz de modelo. Rotar la cámara y mostrar cómo se modifica la matriz de vista. Cambiar entre proyección ortográfica y perspectiva y comparar las diferencias numéricas en la matriz de proyección.** {#mover-o-rotar-uno-de-los-cubos-y-mostrar-cómo-cambian-los-valores-de-su-matriz-de-modelo.-rotar-la-cámara-y-mostrar-cómo-se-modifica-la-matriz-de-vista.-cambiar-entre-proyección-ortográfica-y-perspectiva-y-comparar-las-diferencias-numéricas-en-la-matriz-de-proyección.}

Vamos a dividir la respuesta en tres:

1. Mover o rotar un cubo:  
   1. Normal

   <img width="624" height="186" alt="image" src="https://github.com/user-attachments/assets/065e2361-9f32-45f3-a0f8-bd111e5514d0" />

   2. Movido

      <img width="622" height="190" alt="image" src="https://github.com/user-attachments/assets/544dc47a-d7a3-44d7-aeb3-5c65ceb85256" />

   3. Rotado

   	<img width="632" height="186" alt="image" src="https://github.com/user-attachments/assets/459991c0-ea8d-49c7-ad8f-6e20c7ece053" />


2. Rotación de la cámara  
   1. Normal

		<img width="654" height="188" alt="image" src="https://github.com/user-attachments/assets/48c5c59e-4017-406f-826d-96d1640eaf56" />


2. Rotada

   <img width="646" height="183" alt="image" src="https://github.com/user-attachments/assets/dcb19381-41ce-41cd-9a02-20d1d1b10c2e" />


3. Cambio de perspectiva de la cámara  
   1. Normal

     <img width="634" height="187" alt="image" src="https://github.com/user-attachments/assets/353511c5-d720-45cd-b7bd-4890db2c48b4" />

   2. Ortográfica 

   	<img width="636" height="178" alt="image" src="https://github.com/user-attachments/assets/3f2cfe90-db8b-4767-a1b1-db98da072436" />
