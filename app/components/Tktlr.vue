<script setup>
import {ref,onMounted} from "vue"; const imageUrl=ref(""); const proxyUrl=ref(""); const isLoading=ref(false);

const genTktlr=async()=>{
  alert(2);
  proxyUrl.value=`/api/proxy?url=${encodeURIComponent(imageUrl.value)}`;
  //img.src=proxyUrl.value;
  alert(proxyUrl.value);
};

onMounted(()=>{
  //window.onload=function(){
    setTimeout(function(){
      imageUrl.value=document.getElementById("ee").src;
      genTktlr();
    },1800);
  //}
});
</script>
