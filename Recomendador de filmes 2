let campoIdade;
let campoFantasia;
let campoAventura;

function setup() {
  createCanvas(800, 400);
  createElement('h2', "Recomendador de filmes")
  createSpan("Sua idade:");
  campoIdade = createInput("5");
  campoFantasia = createCheckbox("Gosta de fantasia?");
  campoAventura = createCheckbox("gosta de aventura?");
}

function draw() {
  background('white');
  let idade = campoIdade.value();
  let gostaDeFantasia = campoFantasia.checked();
  let gostaDeAventura = campoAventura.checked();
  let recomendacao = geraRecomendacao(idade, gostaDeAventura);
  
  fill(color(76, 0, 115)); 
  textAlign(CENTER, CENTER);
  textSize(38);
  text(recomendacao, width / 2, height / 2);
}

function geraRecomendacao(idade, gostaDeFantasia, gostaDeAventura) {
  if (idade >= 10){ 
    if (idade >= 12) {
      return "Jurassic World: O Mundo dos Dinossauros";
    }else {
      if (idade >= 14) {
        if(gostaDeFantasia || gostaDeAventura) {
          return "Jurassic Park 3";          
        } else{
         return "Uncharted: Fora do Mapa";
        }
      } else {
        if (gostaDeFantasia) {
          return "As aventuras de pi";
        } else {
          return "Homem aranha: no aranhaverso";
        }
      }
    }
  }else {
    if (gostaDeFantasia) {
      return "A viagem de chihiro";
    } else {
      return "O Estranho Mundo de Jack";
    }
  }
}
