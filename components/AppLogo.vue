<template>
  <div class="VueToNuxtLogo">
    <div class="tangerine tangerine--pulp">
      <i class="tangerine tangerine--dot" />
      <i class="tangerine tangerine--dot" />
      <i class="tangerine tangerine--dot" />
      <i class="tangerine tangerine--dot" />
      <i class="tangerine tangerine--dot" />
    </div>
    <div class="tangerine tangerine--leaf"></div>
  </div>
</template>

<style>
.VueToNuxtLogo {
  display: inline-block;
  animation: turn 2s linear forwards 1s;
  position: relative;
  overflow: hidden;
  height: 180px;
  width: 245px;
}

.tangerine--leaf {
  position: absolute;
  top: 10%;
  left: 50%;
  background-color: #78C10A;
  height: 20%;
  width: 20%;
  transform: translate(-50%, -50%);
  border-radius: 100% 0;
  overflow: hidden;
}
.tangerine--leaf::after {
  content: "";
  clear:both;
  display: block;
  height: 100%;
  border: 3px solid rgba(66, 134, 23, .5);
  transform: rotate(-36deg);
  margin-top: 20px;
}

.tangerine--pulp {
  position: absolute;
  bottom: 0;
  background-color: #EF8227;
  height: 90%;
  width: 90%;
  border-radius: 100%;

  display: flex;
}

.tangerine--pulp > i {
  display: inline-block;
  width: 2px;
  height: 5px;
  background-color: #C6391C;
  flex:none;
}

</style>

