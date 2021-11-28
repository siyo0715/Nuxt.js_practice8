<template>
  <section class="container">
    <div>
      <!-- クラシックモード↓(モジュールモードを使うためにindex.jsを削除した) -->
    <!-- <p>{{ $store.state.message }}</p> -->
    <!-- <button v-on:click="$store.commit('updateMessage')">Update</button> -->
    <!-- <button v-on:click="$store.commit('updateMessage', 'Commit with payload')">Update</button> -->
    <!-- <button v-on:click="$store.dispatch('updateMessageAction', 'Commit with payload')">dispatch</button> -->
      <!-- モジュールモード↓ -->
    <p>{{ $store.state.hello.message }}</p>
    <button v-on:click="$store.dispatch('hello/updateMessageAction', 'Dispatch with payload')">dispatch</button>
    </div>
  </section>
</template>

<script>

export default {
}
</script>
