# adaptador.js

class Pato {
  quack() {
    console.log("Quack");
  }
}

class AdaptadorPato {
  constructor(pato) {
    this.pato = pato;
  }
  
  grasnar() {
    this.pato.quack();
  }
}

const pato = new Pato();
const adaptadorPato = new AdaptadorPato(pato);

adaptadorPato.grasnar();
