<template>

  <div class="locale-switcher">
    {{ $i18n.locale }}
    <select v-model="$i18n.locale">

      <option value="en">English</option>

      <option value="ar">Arabic</option>

    </select>

  </div>

</template>
