<template>
  <q-page class="column justify-center items-center">
    <div class="row items-center justify-around q-mt-xl container-logo">
      <q-img src="../assets/logo-white.png" width="50px" />
      <strong class="">Giovane</strong>
    </div>
    <q-icon name="expand_more" size="28px" class="q-icon-arrow" />
    <q-card class="my-card q-ma-lg" flat border-radius>
      <q-card-section horizontal class="q-pa-lg">
        <div class="container-card">
          <q-icon name="payment" size="35px" class="q-icon-card" />
          <span class="q-mx-xs card-desc">Cartão de crédito</span>
          <div class="info-container q-mt-md">
            <strong class="text-uppercase">Fatura Atual</strong>
            <h4 class="q-ma-none">R$8450,00</h4>
            <div>
              <span>Limite Disponivel</span>
              <strong class="q-ml-sm text-uppercase">R$ 5.000,00</strong>
            </div>
          </div>
        </div>
        <q-card-action vertical class="column justify-center">
          <div class="div-orange"></div>
          <div class="div-blue"></div>
          <div class="div-green"></div>
        </q-card-action>
      </q-card-section>
      <div
        class="bottom-container row items-center justify-between q-pa-sm q-mb-md q-mx-sm"
      >
        <q-icon size="25px" name="fastfood" />
        <span class="q-mx-sm"
          >Compra mais recente em ### no valor de R$ 10,00 hoje</span
        >
        <q-icon name="keyboard_arrow_right" size="25px" class="q-icon-arrow" />
      </div>
    </q-card>

    <q-scroll-area horizontal class="q-mt-xl menu">
      <div class="row no-wrap">
        <q-card class="card-items column justify-between">
          <q-card-section>
            <q-icon name="person_add" size="35px" class="" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Indicar amigos</strong>
          </q-card-section>
        </q-card>

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="monetization_on" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Depositar</strong>
          </q-card-section>
        </q-card>

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="payments" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Transferir</strong>
          </q-card-section>
        </q-card>

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="receipt" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Pagar</strong>
          </q-card-section>
        </q-card>

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="qr_code" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>QR Code</strong>
          </q-card-section>
        </q-card>
      </div>
    </q-scroll-area>
  </q-page>
</template>

<script>
export default {
  name: "PageIndex",
};
</script>
<style lang="scss">
.container-logo {
  width: 40%;
  strong {
    color: $white;
    font-size: 22px;
  }
}
.q-icon-arrow {
  color: $white;
}
.my-card {
  width: 100%;
  max-width: 330px;
  min-height: 200px;
}
.container-card {
  width: 95%;
}
.q-icon-card {
  color: gray;
}
.info-container {
  height: 100px;
  h4 {
    color: $blue;
    font-weight: bold;
  }
  strong:first-child {
    color: $blue;
  }
  span {
    color: $gray;
  }
  strong {
    color: $green;
  }
}
.div-orange {
  height: 40%;
  width: 7px;
  background-color: $orange;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}
.div-blue {
  height: 50%;
  width: 7px;
  background-color: $blue;
}
.div-green {
  height: 10%;
  width: 7px;
  background-color: $green;
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
}
.bottom-container {
  .q-icon {
    color: gray;
  }
  span {
    color: gray;
    width: 70%;
  }
}
.card-items {
  height: 130px;
  width: 100px;
  background-color: $purple-1;
  color: $white;
  cursor: pointer;
}
.q-scrollarea {
  width: 330px;
  height: 150px;
  overflow: hidden;
  bottom: 0;
}
.card-desc {
  color: gray;
  font-size: 1.1rem;
  font-weight: normal;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
</style>