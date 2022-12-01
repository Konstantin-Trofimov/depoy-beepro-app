<template>
 <button class="button">{{text}}</button>
</template>

<script>
 export default {
  props: {
   text: {
    type: String,
    default: 'Log in'
   }
  }
}
</script>

<style>
 .button {
  font-weight: 700;
  line-height: 200%;
  padding: 12px 48px;
  background: var(--special-color);
  border-radius: 8px;
  color: var(--black-color);
  border: none;
  cursor: pointer;
 }

 
 @media (max-width: 1440px) {
  .button {
  font-weight: 700;
  line-height: 200%;
  padding: 10px 28px;
  background: var(--special-color);
  border-radius: 8px;
  color: var(--black-color);
  border: none;
  cursor: pointer;
 }
}
</style>