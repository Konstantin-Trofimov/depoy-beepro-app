<template>
 <button class="oval-button">
  <div class="pyramid">
   <span></span>
   <span></span>
   <span></span>
  </div>
  <span class="text-field">{{text}}</span>
 </button>
</template>

<script>
 export default {
  props: {
   text: {
    type: String,
    default: 'Show more'
   }
  }
}
</script>

<style>
 .oval-button {
  width: 175.86px;
  height: 37.5px;
  border: 2px solid var(--special-color);
  border-radius: 28px;
  background: transparent;
  padding: 0 24px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  cursor: pointer;
 }

 .oval-button .text-field {
  font-weight: 700;
  line-height: 200%;
  display: flex;
  align-items: center;
  color: var(--special-color);
 }

 .oval-button .pyramid {
  width: 16px;
  height: 12px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
 }

 .oval-button .pyramid span{
   height: 2px;
   background: var(--special-color);
 }

 .oval-button .pyramid span:nth-child(1) {width: 16px;}
 .oval-button .pyramid span:nth-child(2) {width: 12px;}
 .oval-button .pyramid span:nth-child(3) {width: 6px;}
 </style>