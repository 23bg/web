<script>
  import Button from "$lib/components/ui/button/button.svelte";
  export let url='';
  export let social='';
  
</script>

<main>
    <div class="w-full h-full bg-gray-50 border-2 p-3 rounded-lg flex justify-center items-center">
        
            
            <div class="mx-5">
                <div class="h-28 w-28 p-5 rounded-full flex justify-center items-center border-2">
                    <img src={url} alt="" class="">
                </div>

                <div class=" w-full font-semibold flex text-center">
                    <a href={`/iamprathameshmore/social/${social}`} class="w-full"> <Button variant='link' class='w-full px-0 text-lg' ><p class="font-medium">{social}</p></Button></a>
                </div>

            </div>
    </div>
    
</main>