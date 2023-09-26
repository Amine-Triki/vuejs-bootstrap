<template>
    <footer class="footer pt-2 pb-2 bg-success ">
        <p id="Rights" class="container text-center "> </p>
    </footer>
    
</template>


<script>
export default {
    name : 'AppFooter' ,
    mounted(){
    let year = new Date().getFullYear();
document.getElementById("Rights").innerHTML = `${year} &copy Amine Triki || All Rights Reserved`;
}
}

</script>