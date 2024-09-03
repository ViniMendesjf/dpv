<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#home" @click.prevent="showSection('home')">DPV</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavAltMarkup"
        aria-controls="navbarNavAltMarkup"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <a
            :class="{'nav-link': true, 'active': currentSection === 'quemSomos'}"
            href="#quem-somos"
            @click.prevent="showSection('quemSomos')"
          >Quem somos</a>
          <a
            :class="{'nav-link': true, 'active': currentSection === 'contato'}"
            href="#contato"
            @click.prevent="showSection('contato')"
          >Contato</a>
          <a
            :class="{'nav-link': true, 'active': currentSection === 'areasAtuacao'}"
            href="#areas-atuacao"
            @click.prevent="showSection('areasAtuacao')"
          >Áreas de Atuação</a>
          <a
            :class="{'nav-link': true, 'active': currentSection === 'publicacoes'}"
            href="#publicacoes"
            @click.prevent="showSection('publicacoes')"
          >Publicações</a>
          <a
            :class="{'nav-link': true, 'active': currentSection === 'processos'}"
            href="#processos"
            @click.prevent="showSection('processos')"
          >Processos</a>
          <a
            :class="{'nav-link': true, 'active': currentSection === 'areaRestrita'}"
            href="#area-restrita"
            @click.prevent="showSection('areaRestrita')"
          >Área Restrita</a>
        </div>
      </div>
    </div>
  </nav>

  <!-- Seções -->
  <section id="home" v-if="currentSection === 'home'">
    <div class="container mt-4">
      <h2>Bem-vindo ao DPV</h2>
      <p>Conteúdo inicial da página.</p>
    </div>
  </section>

  <section id="quem-somos" v-if="currentSection === 'quemSomos'">
    <div class="container mt-4">
      <div class="row align-items-center">
        <div class="col-md-6">
          <h2>Quem Somos Institucional</h2>
          <p>
            O Escritório <strong>DRUMMOND, PIVA E VALENTE ADVOGADOS ASSOCIADOS</strong> foi fundado em 2001, em razão do encontro de interesses de profissionais que, em comum e desde então, pretendiam buscar a Justiça em favor de seus clientes com seriedade, competência e ética. Teve como foco inicial o Direito Empresarial, Societário e Tributário, oferecendo serviços especialmente às empresas do setor industrial e moveleiro da cidade de Ubá/MG. A partir de 2006, ampliou a gama de serviços para atendimento também dos interesses de pessoas físicas, em reclamações trabalhistas, questões bancárias, de família, previdenciárias, advindas de relação de consumo, assim como aquelas geradoras de responsabilidade civil (dano material, moral etc.). A sociedade atualmente encontra-se em sua terceira formação e está regularmente inscrita junto à Ordem dos Advogados do Brasil, seção Minas Gerais, sob o n.º 1.595. Oferece um quadro de profissionais experientes e com sólida formação teórica, proporcionando a todos os seus clientes uma equipe multidisciplinar apta à identificação de soluções jurídicas inovadoras, seguras e eficazes.
            <br>
            <strong>Missão:</strong> Oferecer uma prestação de serviços com excelência e qualidade, buscando a solução das questões jurídicas em todas as áreas, por meio da promoção da justiça e do bem estar social, garantindo, sobretudo, a satisfação de seus clientes.
            </br>
            <br>
            <strong>Visão:</strong> Tornar-se referência na prestação de serviços jurídicos especializados não só nas comarcas em que atua diretamente, mas em todo o território nacional.
            </br>
            <br>
            <strong>Valores:</strong> A sociedade tem por ideais: excelência, comprometimento, integridade, ética, respeito, trabalho em equipe e valorização dos profissionais.
            </br>
          </p>
        </div>
        <div class="col-md-6 d-flex justify-content-end">
          <img
            src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQSSIIirdwIgT8AKQya7vvUY0WFIFB7Fhsc3w&s"
            alt="Imagem da Logo do Escritório"
            class="img-fluid"
            style="max-width: 80%;"
          />
        </div>
      </div>
    </div>
  </section>

  <section id="contato" v-if="currentSection === 'contato'">
    <div class="container mt-4">
      <div id="lawyerCarousel" class="carousel slide bg-wine" data-bs-ride="carousel" data-bs-interval="60000">
        <div class="carousel-inner">
          <!-- Slide 1 -->
          <div class="carousel-item active">
            <div class="text-center mb-4">
              <h2>Contato</h2>
              <p>Conheça nossos Advogados</p>
            </div>
            <div class="d-flex justify-content-center">
              <div class="row">
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dr. Dílio Procópio Dayrell Drummond de Alvarenga</h5>
                      <p class="card-text">OAB/MG 76.125 - OAB/RJ 212.975</p>
                      <p class="card-text">Email: dilio@dpv.adv.br</p>
                      <p class="card-text">Telefone: (32) 99987-1226</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dr. Rodrigo Valente Mota</h5>
                      <p class="card-text">OAB/MG 92.234</p>
                      <p class="card-text">Email: rodrigo.dpv.adv.br</p>
                      <p class="card-text">Telefone: (32) 99975-9330</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Slide 2 -->
          <div class="carousel-item">
            <div class="text-center mb-4">
              <h2>Contato</h2>
              <p>Conheça nossos Advogados</p>
            </div>
            <div class="d-flex justify-content-center">
              <div class="row">
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dr. Pedro Santos</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: pedro.santos@example.com</p>
                      <p class="card-text">Telefone: (31) 1122-3344</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dra. Ana Costa</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: ana.costa@example.com</p>
                      <p class="card-text">Telefone: (31) 2233-4455</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Slide 3 -->
          <div class="carousel-item">
            <div class="text-center mb-4">
              <h2>Contato</h2>
              <p>Conheça nossos Advogados</p>
            </div>
            <div class="d-flex justify-content-center">
              <div class="row">
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dr. Lucas Almeida</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: lucas.almeida@example.com</p>
                      <p class="card-text">Telefone: (31) 3344-5566</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dra. Juliana Mendes</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: juliana.mendes@example.com</p>
                      <p class="card-text">Telefone: (31) 4455-6677</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Slide 4 -->
          <div class="carousel-item">
            <div class="text-center mb-4">
              <h2>Contato</h2>
              <p>Conheça nossos Advogados</p>
            </div>
            <div class="d-flex justify-content-center">
              <div class="row">
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dr. Felipe Rocha</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: felipe.rocha@example.com</p>
                      <p class="card-text">Telefone: (31) 5566-7788</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dra. Renata Silva</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: renata.silva@example.com</p>
                      <p class="card-text">Telefone: (31) 6677-8899</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Slide 5 -->
          <div class="carousel-item">
            <div class="text-center mb-4">
              <h2>Contato</h2>
              <p>Conheça nossos Advogados</p>
            </div>
            <div class="d-flex justify-content-center">
              <div class="row">
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dr. João Fonseca</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: joao.fonseca@example.com</p>
                      <p class="card-text">Telefone: (31) 7788-9900</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dra. Mariana Oliveira</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: mariana.oliveira@example.com</p>
                      <p class="card-text">Telefone: (31) 8899-0011</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Slide 6 -->
          <div class="carousel-item">
            <div class="text-center mb-4">
              <h2>Contato</h2>
              <p>Conheça nossos Advogados</p>
            </div>
            <div class="d-flex justify-content-center">
              <div class="row">
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dr. Rafael Pereira</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: rafael.pereira@example.com</p>
                      <p class="card-text">Telefone: (31) 9900-1122</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-3">
                  <div class="card bg-white text-dark">
                    <div class="card-body">
                      <h5 class="card-title">Dra. Isabel Souza</h5>
                      <p class="card-text">OAB</p>
                      <p class="card-text">Email: isabel.souza@example.com</p>
                      <p class="card-text">Telefone: (31) 0011-2233</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <button
          class="carousel-control-prev"
          type="button"
          data-bs-target="#lawyerCarousel"
          data-bs-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Anterior</span>
        </button>
        <button
          class="carousel-control-next"
          type="button"
          data-bs-target="#lawyerCarousel"
          data-bs-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Próximo</span>
        </button>
      </div>
    </div>
  </section>
 
  <section id="areas-atuacao" v-if="currentSection === 'areasAtuacao'">
    <div class="container mt-4">
      <h2>Areas Atuação</h2>
      <p>Conteúdo das areas de atuação será inserido aqui.</p>
    </div>
  </section>


  <section id="publicacoes" v-if="currentSection === 'publicacoes'">
    <div class="container mt-4">
      <h2>Publicações</h2>
      <p>Conteúdo das publicações será inserido aqui.</p>
    </div>
  </section>

  <section id="processos" v-if="currentSection === 'processos'">
    <div class="container mt-4">
      <h2>Processos</h2>
      <p>Conteúdo dos processos será inserido aqui.</p>
    </div>
  </section>

  <section id="area-restrita" v-if="currentSection === 'areaRestrita'">
    <div class="container mt-4">
      <h2>Área Restrita</h2>
      <p>Conteúdo da área restrita será inserido aqui.</p>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      currentSection: "home",
    };
  },
  methods: {
    showSection(section) {
      this.currentSection = section;
    },
  },
};
</script>

<style>
.navbar-brand {
  font-weight: bold;
  color: #000000;
}

.navbar-nav .nav-link {
  font-weight: normal; /* Remove o negrito dos links por padrão */
}

.navbar-nav .nav-link.active {
  font-weight: bold;
  color: #940f14;
}

.carousel-item {
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: #ffffff; /* Cor do texto branca */
}

.card {
  height: 100%;
  margin: 10px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.card-body {
  color: #000000; /* Cor do texto dos cards */
  text-align: center;
}

.card:hover {
  transform: scale(1.05);
}

.carousel-item {
  padding: 15px;
}

.carousel-control-prev-icon,
.carousel-control-next-icon {
  background-color: #310000; /* Cor de fundo das setas */
  border-radius: 10%; /* Forma circular */
  height: 10px; /* Altura das setas */
  width: 10px; /* Largura das setas */
}

.bg-wine {
  background-color: #940f14;
}

/* Ajustes no estilo dos títulos das seções */
section h2 {
  font-weight: normal; /* Remove o negrito */
}
</style>
