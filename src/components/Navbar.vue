<template>
  <header>
      <div class="logo">
          <img src="@/assets/rainbow.svg" alt="rainbow logo">
      </div>
      <nav>
          <ul>
              <li>home</li>
              <li>about</li>
              <li>glossary</li>
              <li>story</li>
              <li>contribute</li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">

header {

    .logo img {
        position: absolute;
        top: 20px;
        left: 100px;
        width: 50px;
    }

    nav {
        display: flex;
        justify-content: flex-end;
        
        ul{
            display: flex;
            list-style: none;
            padding-right: 100px;
            justify-content: flex-end;
            background: #ffffff;
            margin-top: 40px;
    
            li {
                padding: 20px 20px;
                border-radius: 50px;
            }
        }
    }
    
}

</style>