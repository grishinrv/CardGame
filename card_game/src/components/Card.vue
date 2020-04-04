<template>
    <div class="card">
        <div class="miniCell glueLeft testCell">
            <p>3</p>
        </div>
        <div class="imageContainer">
            <!-- переделать на получение картинки из props компонента,
                используя синтаксис привязки
             -->
            <img class="avatar embeded" alt="Место под картинку"
src="https://cdnb.artstation.com/p/assets/images/images/018/433/397/large/anton-evsyukov-blood-elf.jpg?1559343941"/>
        </div>
        <div class="rowCell glueBottom testCell">
            <div class="miniCell">
                <img class="embeded"
src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSVq047Xkq-mdmT8MLMad8bre5PVevJ7jCZKklptIrqCVE0caXE&usqp=CAU"/>
            <!-- переделать на получение значений атаки и защиты из props компонента,
                используя синтаксис привязки
             -->
                <p class="over">2</p>
            </div>
            <div class="miniCell">
                <p class="over">4</p>
                <svg class="bi bi-shield-shaded" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" d="M5.443 1.991a60.17 60.17 0 00-2.725.802.454.454 0 00-.315.366C1.87 7.056 3.1 9.9 4.567 11.773c.736.94 1.533 1.636 2.197 2.093.333.228.626.394.857.5.116.053.21.089.282.11A.73.73 0 008 14.5c.007-.001.038-.005.097-.023.072-.022.166-.058.282-.111.23-.106.525-.272.857-.5a10.197 10.197 0 002.197-2.093C12.9 9.9 14.13 7.056 13.597 3.159a.454.454 0 00-.315-.366c-.626-.2-1.682-.526-2.725-.802C9.491 1.71 8.51 1.5 8 1.5c-.51 0-1.49.21-2.557.491zm-.256-.966C6.23.749 7.337.5 8 .5c.662 0 1.77.249 2.813.525a61.09 61.09 0 012.772.815c.528.168.926.623 1.003 1.184.573 4.197-.756 7.307-2.367 9.365a11.191 11.191 0 01-2.418 2.3 6.942 6.942 0 01-1.007.586c-.27.124-.558.225-.796.225s-.526-.101-.796-.225a6.908 6.908 0 01-1.007-.586 11.192 11.192 0 01-2.417-2.3C2.167 10.331.839 7.221 1.412 3.024A1.454 1.454 0 012.415 1.84a61.11 61.11 0 012.772-.815z" clip-rule="evenodd"/>
                <path d="M8 2.25c.909 0 3.188.685 4.254 1.022a.94.94 0 01.656.773c.814 6.424-4.13 9.452-4.91 9.452V2.25z"/>
                </svg>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    // описать принимаемые компонентом данные
}
</script>

<style scoped>
.card {
    width: 140px;
    height: 220px;
    border: 2px solid black;
    background-color: burlywood;
}
div{
    padding: 0;
}
.testCell{
    border: 1px dashed grey;
}
.miniCell{
    width: 17%;
    max-height: 25px;
    padding-left: 1px;
    padding-right: 1px;
    position: relative;
}
.glueBottom{
    margin-top:auto;
}
.glueRight{
    margin-left: auto;
}
.glueLeft{
    margin-right: auto;
}
.rowCell{
    width: 100%;
    height: 25px;
    display: flex;
    justify-content: space-between;
    align-content: space-around;
}
.imageContainer{
    width: 100%;
    height: 70%;
    margin-left: auto;
    margin-right: auto;
    border-radius: 50%;
    transform: scaleX(0.8);
    float: top;
}
.avatar{
    border-radius: 50%;
    position: relative;
    left: 10%;
}
.embeded{
    max-width: 100%;
    max-height: 100%;
    display: block;
}
.over{
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 10;
  font-size: large;
  color: red;
}
</style>