class Carro {
    constructor(cor, modelo) {
      this.cor = cor;
      this.modelo = modelo;
      this.velocidadeAtual = 0;
      this.ligado = false;
    }
  
    ligar() {
      this.ligado = true;
      console.log("O carro está ligado.");
    }
  
    acelerar(velocidade) {
      if (this.ligado) {
        this.velocidadeAtual += velocidade;
        console.log(`Acelerando para ${this.velocidadeAtual} km/h.`);
      } else {
        console.log("O carro precisa estar ligado para acelerar.");
      }
    }
  
   
  
