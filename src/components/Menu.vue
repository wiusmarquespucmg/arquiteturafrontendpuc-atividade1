<script setup>
const peple = {
  name: 'Jôtarô Kûjô',
  description: 'JoJo no Kimyō na Bōken (ジョジョの奇妙な冒険? lit. (As) Bizarras Aventuras de JoJo) é um mangá japonês escrito e ilustrado por Hirohiko Araki. O mangá foi publicado pela Shueisha em sua revista Weekly Shōnen Jump entre 1987 e 2004, e a partir de 2004 pela revista seinen Ultra Jump. É o segundo mangá mais longo da Shonen Jump com 127 volumes (apenas atrás de Kochi-Kame, concluído com 200 volumes) e ainda está em produção. O que fazia dele também, até meados de 2012, o mangá mais longo sem uma adaptação para televisão.[1]'
};
</script>

<template>
  <main>
    <div>
        <div class="menu">
            <ul class="menu_container--primary">
                <li class="menu_item--primary">
                    <router-link to="/blog">Blog</router-link>
                </li>
                <li  class="menu_item--primary">
                    <router-link to="/about">Sobre</router-link>
                </li>
                <li class="menu_item--primary">
                    <router-link to="/description">descricao</router-link>
                </li>
            </ul>
        </div>
        <div class="menu-content--primary">
            <div>
                <img class="menu_content--avatar" src="../assets/icons/jojo.png" alt="">
            </div>
            <div>
                <h1 class="menu_content--nome">{{ peple.name }}</h1>
                <p class="menu_content--description">
                    {{ peple.description }}
                </p>
            </div>
        </div>
    </div>
  </main>
</template>

<style scoped>

.menu {
    display: flex;
    align-items: center;
    width: 100%;
    height: 60px;
    justify-content: center;
    background-color: #2576de;
}

.menu_container--primary{
    width: 100%;
    display: flex;
    max-width: 300px;
}
.menu_item--primary {
    display: flex;
    width: 100%;
    justify-content: center;
    color: white;
    text-transform: uppercase;
}

.menu_item--primary > a{
    color: white;
    cursor: pointer;
    font-size: 14px;
    color: inherit;
    text-decoration: none;
}

.menu-content--primary{
    width: 100%;
    background-color: #2576de;
    display: flex;
    justify-content: center;
    align-items: center;
}

.menu_content--avatar{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    margin-right: 50px;
    border: 2px solid white;
    background-color: white;
}
.menu_content--nome{
    color: white;
    font-size: 40px;
    margin-top: 10px;
}

.menu_content--description{
    color: white;
    font-size: 12px;
    margin-top: 10px;
    max-width: 400px;
}
</style>
