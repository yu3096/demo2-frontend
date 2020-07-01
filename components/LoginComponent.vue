<template>
  <form class="col-5">
    <div class="form-group row">
      <label for="id" class="col-3 col-form-label col-form-label">로그인 ID</label>
      <div class="col-9">
        <input type="text" class="form-control form-control" id="id" placeholder="아이디">
      </div>
    </div>
    <div class="form-group row">
      <label for="pw" class="col-3 col-form-label col-form-label">로그인 PW</label>
      <div class="col-9">
        <input type="text" class="form-control form-control" id="pw" placeholder="비밀번호">
      </div>
    </div>
    <div class="col-auto">
      <button type="submit" class="btn btn-primary">Submit</button>
    </div>
  </form>
</template>

<script>
    export default {
        name: "LoginComponent"
    }
</script>

<style lang="scss" scoped>
  form {
    margin: auto;
    padding: 30px;
    position: absolute;
    top: 40%;
    left: 35%;
    /*
    background: lighten($primary, 4%);
    position: relative;
    border-radius: 1rem;
    */
  }

  button[type=submit] {
    width: calc((1.5em + 1rem + 2px) * 2);
    height: calc((1.5em + 1rem + 2px) * 2);
    border-radius: 50%;
    position: absolute;
    right: 9px;
    top: 50%;
    border: 5px solid lighten($primary, 10%);
    background: $primary;
    font-size: 18px;
    color: #fff;
    font-weight: normal;
    text-shadow: 1px 1px 2px #000;
    box-sizing: border-box;
  }
</style>
