<template>
  <div class="error">
    <h1>[Widget Name] failed to load</h1>
    <p>
      Please try to reload the page. If the problem persists please contact your
      local order desk administrator
    </p>

      <!-- <div style="backgroundColor:red">hello</div>
      <div style="backgroundColor:green">Bye</div> -->
  </div>
</template>

<style scoped>
.error {
  padding: 32px;
  background-color: #ffffff;
  height: 566px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
}

/* Small phone: from 0 to 480px */
@media only screen and (max-width: 480px) {
  .error{
  height: 428px;

  }
}
</style>