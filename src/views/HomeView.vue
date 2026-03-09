<script setup>
</script>

<template>
  <main>
    <div class="container">
      <div>
        <p class="topLine">
          Des millions de petites annonces et autant d'occasions de se faire plaisir
        </p>
        <div class="bloc">
          <img />
          <div>
            <p>C'est le moment de vendre</p>
            <div class="publish-btn">
              <RouterLink to="/publish">
                <font-awesome-icon :icon="['fa', 'plus-square']" />
                <span>Déposer une annonce</span>
              </RouterLink>
            </div>
          </div>
          <img />
        </div>
        <div class="offersbloc">

        </div>
        <div class="pagination">

        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.bloc {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: var(--orange-pale);
  border-radius: 20px;
  margin-bottom: 35px;
}

.topLine {
  text-align: center;
  font-size: 24px;
  font-weight: 600;
  margin: 30px 0;
}

main {
  min-height: calc(100vh - var(--header-height) - var(--footer-height));
  margin-top: var(--header-height);
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: calc(100vh - var(--header-height) - var(--footer-height));
  padding-bottom: 40px;
}
</style>