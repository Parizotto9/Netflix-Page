<template>
  <q-page class="dimme back ">
    <q-img src="../assets/logo.png" width="180px" class="q-ml-xl"></q-img>
    <div class="full-width column items-center">

      <q-card class=" my-card card items-center">
        <q-card-section>
          <div class="text-h4 text-bold get-in q-mt-xl">Entrar</div>
        </q-card-section>

        <q-card-section class="column items-center">
          <q-input class="input q-my-md " v-model="login" label="E-mail ou número de telefone"  />
          <q-input class="input" v-model="password" label="Senha"  />
          <q-btn style="background: red; color: white" no-caps label="Entrar" class="q-mt-xl button q-pa-sm text-bold" />
          <div class=" row justify-around items-center full-width q-mt-sm">
            <q-checkbox size="xs" v-model="remember" val="xs" label="Lembre-se de mim" color="grey" dark />
            <a href="" class="link">Precisa de ajuda?</a>
          </div>
          <q-card-section class="face column no-padding q-mb-xl">
            <span class="q-mt-sm"> <a href="" class="link text-weight-medium"> <q-icon size="2em" name="facebook" /> Conectar com Facebook </a></span>
            <div class="texto q-my-md"  >Novo por aqui? <a href="" class="assine">Assine agora.</a></div>
            <div class="texto2 q-mb-xl">Esta página é protegida pelo Google reCAPTCHA para garantir que você não é um robô. <a class="saiba" href="">Saiba mais.</a></div>
          </q-card-section>
        </q-card-section>


        <div class="footer column items-center full-width fixed-bottom ">
          <div class="footer-info q-mb-md q-mt-lg" style="font-size: 1.1rem">Dúvidas? Ligue <a href="" class="link2">0800-761-4631</a></div>
          <div class="row justify-around" style="width: 1000px">
          <div dark class="footer-info column"> 
           <a href="" class="link2 q-my-sm"> Perguntas frequentes</a> 
           <a href="" class="link2 q-my-sm"> Preferências de cookies</a> 
          </div>
          <div dark class="footer-info column">
            <a href="" class="link2 q-my-sm">Centro de ajuda</a>
            <a href="" class="link2 q-my-sm">Informações corporativas</a>
          </div>
          <div dark class="footer-info">
            <a href="" class="link2 q-mt-">Termos de uso</a>
          </div>
          <div dark class="footer-info">
            <a href="" class="link2">Privacidade</a>
          </div>
          </div>
        </div>
    </q-card>
    </div>

  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageIndex',
  data() {
    return {
      login: '',
      password: '',
      remember: ''

    }
  }
})
</script>

<style lang="scss">
.back {
  background-image: url(../assets/fundo.jpeg);
  background-size: cover;
}
.card {
  color: white;
  background: rgba(0, 0, 0, 0.84);
  width: 500px;
 }

.input {
  color: $grey-5;
  background: $grey-8;
  border-radius: 3px;
  width: 350px;
}

.get-in {
  margin-left: 60px;
}

.button {
  width: 350px;
  font-size: 1.3rem;
}

.link {
  text-decoration: none;
  color: grey;
}

.face {
  width: 350px;
}

.texto {
  color: grey;
  font-size: 1.3em;
}

.assine{
  color: white; 
  text-decoration: none;
}

.assine:hover {
  text-decoration: underline;
}

.saiba {
  color: $light-blue-8;
  text-decoration: none;
}

.saiba:hover {
  text-decoration: underline;
}

.texto2 {
  color: $grey-6
}

.footer {
  width: 600px;
  background-color: rgba(0,0,0,0.84);
}

.footer-info {
  color: $grey-6;
}

.link2 {
  text-decoration: none;
  color: $grey-6;  
}

.link2:hover {
  text-decoration: underline;
}
</style>
