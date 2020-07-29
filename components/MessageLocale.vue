<template>
  <div>
    <p v-t="'hoge'"></p>
    <p v-t="'fuga'"></p>
  </div>
</template>

<style>

@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>

<i18n locale="ja">
  {
    "ja": {
      "hoge": "***"
    },
    "hoge": "hoge!!!",
    "fuga": "fuga!!!"
  }
</i18n>
<i18n src="../assets/messages.ja.yml" lang="yaml" locale="ja" />
<i18n src="../assets/messages.en.yml" lang="yaml" locale="en"></18n>
