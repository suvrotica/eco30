<script>
  import ThemeToggle from './ThemeToggle.svelte';
</script>




<section>
    


  
    <nav>
        <ul>
            <li><div class="logo-container">
                <div class="box box-eco30">ECO30</div>
                <div class="box box-docs">DOCS</div>
              </div>
            </li>
        </ul>
        <ul>
            <li dir="rtl">Ecologically Sustainable by 2030</li>
            <li><ThemeToggle /></li>
        </ul>
    </nav>
</section>

<style>
    section {
        margin: auto;
        width: 95%;
    }

   

.logo-container {
  display: flex;
}

.box {
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  font-size: 24px;
  width: 100px;
  height: 50px;
  margin: 0;
  padding: 0;
}

.box-eco30 {
  background-color: rgb(241, 187, 104);
  color: black;
  border-right: none;
}

.box-docs {
  background-color: rgb(56, 14, 14);
  color: rgb(174, 180, 211);
  border-left: none;
}

</style>
