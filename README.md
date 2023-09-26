var balwaneq = function(x, y) {

ellipse(x, y + 307, 150, 150);
ellipse(x, y + 225, 130, 130);
ellipse(x, y + 152, 120,120);
triangle(x, 20, x + 80, 100, x - 60, 100);
};
    
var pozycja = 100;
var predkosc = 10;


draw = function() {
        
    background(255, 221, 0);
    balwaneq(pozycja, 0);
    pozycja = pozycja + predkosc;
    
    if (pozycja === 400) {
        predkosc = -10;
        
    } if (pozycja === 0) {
        predkosc = 10;
    }
    
};
