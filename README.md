# RELOJ_ALEJANDRO_CARPETA_1001
En este repositorio se encontrara el código fuente del reloj y la aplicación que es ejecutable en los diferentes sistemas operativos




    horizontal_position = 0

    def setup():
        size(500, 100)




    def draw():

        global horizontal_position
    
        background(map(second(), 0, 59, 255, 0))
    
        noStroke()
        
        fill(map(second(), 0, 59, 0, 255))
    
        circle( horizontal_position, 50, 50)
    
        if horizontal_position > width:
    
            horizontal_position = 0
    
        else:
    
            horizontal_position = map(second(), 59, 0, width, 0)


