<template>
  <button class="bvi-icon bvi-open">OK!</button>
</template>

<script>
import { Bvi } from '@/components/bvi/bvi.js';

export default {
  mounted(){
    try{
      // eslint-disable-next-line no-undef, no-unused-vars
      let bviInit = new Bvi({
        target : '.bvi-open', 
        theme : "white", // Цвет сайта
        font : "Ubuntu", // Шрифт
        fontSize : 16, // Размер шрифта
        letterSpacing : "normal", // Межбуквенный интервал
        lineHeight : "normal", // Междустрочный интервал
        reload : true, // Перезагрузка страницы при выключении плагина
        fixed : false, // Фиксирование панели для слабовидящих вверху страницы
        speech : false, // Синтез речи
        panelHide : false // Скрывает панель для слабовидящих и показывает иконку панели.
      });
    }
    catch(e){
      console.log(e);
    }
  }
}
</script>

<style lang="css">
@import "@/components/bvi/bvi.css";
.bvi-icon{
  cursor: pointer;
}
</style>