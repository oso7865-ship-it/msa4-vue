<script setup>
// js 코드 작성 부분
import { ref } from 'vue';
import ConditionalRendering from './components/ConditionalRendering.vue';
import DataBinding from './components/DataBinding.vue';
import EventHandling from './components/EventHandling.vue';
import LifeCycle from './components/LifeCycle.vue';
import ListRendering from './components/ListRendering.vue';
import MyTransition from './components/MyTransition.vue';
import Props from './components/Props.vue';
import ProtoType from './components/ProtoType.vue';
import Slot from './components/Slot.vue';
import Watchers from './components/Watchers.vue';


const flgLifeCycle = ref(true);
</script>

<template>
<!-- HTML 작성 부분 -->
  <DataBinding v-if="false" />
  <EventHandling v-if="false"/>
  <ConditionalRendering v-if="false"/>
  <ListRendering v-if="false"/>
  <Watchers v-if="false"/>
  <Props v-if="false"/>
  <Slot v-if="false"/>
  <MyTransition v-if="false"/>
  <ProtoType v-if="false"/>
  <LifeCycle v-if="flgLifeCycle"/>
  <button type="button" @click="flgLifeCycle = !flgLifeCycle">라이프사이클 컴포넌트 토글</button>
</template>

<style>
/* CSS 작성부분 */
</style>