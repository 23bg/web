<script>
  import Button from "$lib/components/ui/button/button.svelte";
  import Iconsspace from "./iconsspace.svelte";

  let arr = new Array(7);

    
</script>
<div class="w-full flex h-full justify-start items-start bg-gray-50 border-2 p-3 rounded-lg">
    <div>
    
        <div class="text-lg font-semibold px-1">
          Whatsapp Auto Reply
        </div>
        
      
      
      <div class="text-xs  px-1 py-2">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cupiditate praesentium soluta ex dicta, repellat tenetur numquam sit deserunt officia iure dolor molestias sint inventore esse quasi! Laboriosam numquam animi molestiae. 
      </div>
     
      <div class="grid lg:grid-cols-5 h-full grid-cols-5 gap-1">
        {#each arr as arr}
           <Iconsspace/>
        {/each}
       
        
        
        
      </div>
    <a href="/iamprathameshmore" target="_blank" class="px-0.5"><Button variant='link' class='p-0 text-xs m-0 text-gray-500 hover:text-indigo-500'>Read Document</Button></a>
       
      
        
     
     
    </div>
  </div>