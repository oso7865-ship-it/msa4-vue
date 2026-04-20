<script setup>
// 자식 컴포넌트에서는 difineProps()를 이용해 넘어온 데이터 선언
// - 이때 부모 컴포넌트에서 넘겨줄 때 사용한 키를 사용해 선언
// - 데이터 타입도 지정

// const props = defineProps({
//   'cnt': Number,
//   'page': Number
// });

defineProps(['cnt', 'page']);

// 위 둘중 하나의 방법으로 하면 됨

// 자식 컴포넌트에서는 difineEmits()를 이용해 넘어온 컴포넌트 이벤트 선언
//  - 이때 부모 컴포넌트에서 넘겨줄 때 사용한 이벤트 명을 사용해 선언
defineEmits(['minusCnt'])
// const emit = defineEmits(['minusCnt']) 선언시 @이벤트="emit"('minusCnt', 10)

// 위 둘중 하나의 방법으로 하면 됨

</script>

<template>
  <h1>{{ page }}프롭스 자식 컴포넌트: {{ cnt }}</h1>
  <button type="button" @click="$emit('minusCnt', 10)">감소(자식쪽)</button>
</template>

<style scoped>

</style>