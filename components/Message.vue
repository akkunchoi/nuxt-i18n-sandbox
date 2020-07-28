<template>
  <div>
    <h6>$t</h6>
    <p>({{ $t('hello') }})</p><!-- 親の定義は子に反映されない -->
    <p>({{ $t('hoge') }})</p>
    <p>({{ $t('a.b') }})</p>

    <h6>v-t</h6>
    <p v-t="'hoge'"></p>
    <p v-t="'a.b'"></p>
  </div>
</template>

<style>

@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>

<i18n src="../assets/messages.yml" lang="yaml"></18n>
// 先に読み込まれた方が反映されるので、以下影響しない
<i18n src="../assets/messages.ja.yml" lang="yaml" locale="ja"></18n>
