<script setup>
import {ref,onMounted} from "vue"; const pr2=document.querySelector("#pr2"); const imageUrl=ref(""); const proxyUrl=ref(""); const isLoading=ref(false);

const genTktlr=async()=>{
  alert(2);
  proxyUrl.value=`/api/proxy?url=${encodeURIComponent(pr.value)}`;
  //img.src=proxyUrl.value;
  alert("PRX: "+proxyUrl.value);
};

onMounted(()=>{
  window.onload=function(){
    setTimeout(function(){
      //imageUrl.value=document.getElementById("ee").src;
      genTktlr();
    },1800);
  }
});
</script>
