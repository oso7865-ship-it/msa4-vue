<script setup>

</script>

<template>
  <h1>어서오세요</h1>
  <h2>아이디와 비밀번호를 입력해주세요.</h2>
  <form action="" method="get">
    <label for="id">ID</label>
    <input type="text" name="id" required="">
    <label for="pw">PassWord</label>
    <input type="password" name="pw" required="">
    <button type="sumbit">보내기</button>
    <h3>보안문자를 입력해주세요.</h3>
    <div class="box">qeozx31</div>
    <input type="text" required="">
    
    
  </form>
</template>

<style scoped>

form {
  margin: auto;
  padding: 10px;
  margin-top: 0%;
  width: 400px;
  border: 1px solid black;
  align-items: center;
  display: flex;
  flex-direction: column;
  gap: 5px;
}

input {
  width: 150px;
}
.box {
  border: 1px solid black;
  width: 200px;
  height: 50px;
  align-content: center;
  font-size: 24px;
}
</style>