# Taller 2
[Inicio](/README.md)
1.  - Casa:
        1. Tender la cama después de ir al baño. 
        2. Desayunar una vez alistado todas las cosas para salir.
        3. Encender el computador una vez se regresa a casa.
    - Universidad:
        1. Desayunar apenas se llega a la universidad.
        2. Buscar personas conocidas con las cuales almorzar.
        3. Estudiar en la biblioteca de Ciencia y Tecnología o el edifcio Insignia.
        4. Asistir a todas las clases que haya en el día.
        5. Trabajar en los tiempos libre entre clases y después de clases.
    - Transporte:
        1. Buscar un espacio cómodo para estar de pie en el bus y poner la maleta en el suelo.
        2. Sentarse en una silla vacía cuando alguna de estas esté disponible.
        3. Cerrar la ventana si se está en una zona o silla al lado de la ventana.
        4. Dar el asiento a una persona mayor, con bebé en brazos o con movilidad reducida.
2. Se utlizó ChatGPT para realizar el código del AC probabilístico usando los siguientes prompts:
    ### Prompt 1
    2. Suponga una enfermedad, o un incendio forestal, o una moda, desarrolle un modelo de difusión usando ACs probabilísticos. O simule un robot con dos ruedas que evite obstáculos.
    ### Prompt 2
    Prefiero el primer enfoque
    ### Prompt 3
    El fenómeno a modelar será un incendio forestal. La cuadrícula será: árbol, ardiendo, quemado. Las reglas serán: las mismas reglas que estableciste. Para la simulación hacemos la que dices. Esto lo pienso implementar con Python
    ## Resultado
    [AC probabilístico](./Untitled.ipynb)
3. Se utlizó ChatGPT para realizar el código para el mapa de Voronoi usando los siguientes prompts
    ### Prompt 1
    La ciudad escogida es San Gil, Santander, Colombia. Obtén las coordenadas de cada droguería o farmacía (son sinónimos como ya sabes)
    ### Prompt 2
    Localiza todas las droguerías en en la ciudad descrita junto con sus coordenadas, viendo Google Maps son más de 5 
    ### Prompt 3
    A partir de la primera opción y tomando el código base para generar el diagrama de Voronoi escribe un nuevo código en python
    ### Prompt 4
    Para el código anterior hubo el siguiente error:

    ---------------------------------------------------------------------------
    QhullError                                Traceback (most recent call last)
    <ipython-input-1-6c4c8c29d46c> in <cell line: 0>()
        17 
        18 # Crear el diagrama de Voronoi
    ---> 19 vor = Voronoi(puntos)
        20 
        21 # Dibujar el diagrama de Voronoi

    _qhull.pyx in scipy.spatial._qhull.Voronoi.__init__()

    _qhull.pyx in scipy.spatial._qhull._Qhull.__init__()

    QhullError: QH6154 Qhull precision error: Initial simplex is flat (facet 2 is coplanar with the interior point)

    While executing:  | qhull v Qz Qbb Qc
    Options selected for Qhull 2019.1.r 2019/06/21:
    run-id 1709982886  voronoi  Qz-infinity-point  Qbbound-last  Qcoplanar-keep
    _pre-merge  _zero-centrum  Qinterior-keep  Pgood  _max-width 0.0015
    Error-roundoff 1e-13  _one-merge 7.1e-13  Visible-distance 2e-13
    U-max-coplanar 2e-13  Width-outside 4.1e-13  _wide-facet 1.2e-12
    _maxoutside 8.1e-13

    The input to qhull appears to be less than 3 dimensional, or a
    computation has overflowed.

    Qhull could not construct a clearly convex simplex from points:
    - p5(v4):   6.6   -73    73
    - p4(v3):   6.6   -73 0.015
    - p3(v2):   6.6   -73 0.032
    - p1(v1):   6.6   -73     0

    The center point is coplanar with a facet, or a vertex is coplanar
    with a neighboring facet.  The maximum round off error for
    computing distances is 1e-13.  The center point, facets and distances
    to the center point are as follows:

    center point    6.556   -73.13     18.3

    facet p4 p3 p1 distance= -5.5e-07
    facet p5 p3 p1 distance= 1.5e-14
    facet p5 p4 p1 distance= -6.7e-15
    facet p5 p4 p3 distance= -2.1e-14

    These points either have a maximum or minimum x-coordinate, or
    they maximize the determinant for k coordinates.  Trial points
    are first selected from points that maximize a coordinate.

    The min and max coordinates for each dimension are:
    0:     6.556     6.557  difference= 0.0015
    1:    -73.14  -2.225e-308  difference= 73.14
    2:         0     73.13  difference= 73.13

    If the input should be full dimensional, you have several options that
    may determine an initial simplex:
    - use 'QJ'  to joggle the input and make it full dimensional
    - use 'QbB' to scale the points to the unit cube
    - use 'QR0' to randomly rotate the input for different maximum points
    - use 'Qs'  to search all points for the initial simplex
    - use 'En'  to specify a maximum roundoff error less than 1e-13.
    - trace execution with 'T3' to see the determinant for each point.

    If the input is lower dimensional:
    - use 'QJ' to joggle the input and make it full dimensional
    - use 'Qbk:0Bk:0' to delete coordinate k from the input.  You should
        pick the coordinate with the least range.  The hull will have the
        correct topology.
    - determine the flat containing the points, rotate the points
        into a coordinate plane, and delete the other coordinates.
    - add one or more points to make the input full dimensional.
    Las coordenadas de las droguerías fueron incertadas manualmente para mayor precisión. ya que no se puedieron extraer mediante 'Overpass Turbo'
    ## Resultado
    [Mapa de Voronoi](./Untitled.ipynb)
4. 