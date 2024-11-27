solución taller 2: 

def calcArea (b: Int, h: Double, f:(Int, Double)=> Double) = f(b, h)
def calcTrapecio (b: Int, B: Int, h: Double, f:(Int, Int, Double)=> Double) = f(b, B, h)

val areaTriangulo = (b: Int, h: Double) => (b*h)/2
val paralelogramo = (b: Int, h: Double) => (b*h)
val cuadrado = (b: Int, h: Double) => (b*h)
val rombo = (D: Int, d: Double) => (D*d)/2
val trapecio = (b: Int, B: Int, h: Double) => ((b+B)*h)/2
val polRegular = (p: Int, a: Double) => (p*a)/2
val polIRegular = (p: Int, l: Int, a: Double) => (p*l*a)/2
val areaCirc = (r: Int, pi: Double)=> (pi*(r*r))/2

calcArea(3, 4.5, areaTriangulo)
calcArea(3, 4.5, paralelogramo)
calcArea(3, 4.5, rombo)
calcTrapecio(3, 6, 4.5, trapecio)
calcTrapecio(6, 7, 4.5, polIRegular)
calcArea(5, 3.14, areaCirc)
