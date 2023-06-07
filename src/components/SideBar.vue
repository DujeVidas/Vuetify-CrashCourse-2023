<template>
  <VNavigationDrawer expand-on-hover rail>
    <VList>
      <VListItem
        prepend-avatar="https://static.vecteezy.com/system/resources/previews/009/749/751/non_2x/avatar-man-icon-cartoon-male-profile-mascot-illustration-head-face-business-user-logo-free-vector.jpg"
        title="Duje Vidas"
        subtitle="dujevidas123@gmailcom"
      ></VListItem>
      <VDivider></VDivider>
      <VList density="compact" nav>
        <VListItem
          prepend-icon="mdi-image"
          title="Color Gallery"
          value="color"
          @click="$emit('selectOption', true)"
        ></VListItem>
        <VListItem
          prepend-icon="mdi-dialpad"
          title="Grayspace Gallery"
          value="gray"
          @click="$emit('selectOption', false)"
        ></VListItem>
      </VList>
    </VList>
  </VNavigationDrawer>
</template>

<script>
export default {
    emits:['selectOption'],
}
</script>
