<script>
    
    import Button from '$lib/components/ui/button/button.svelte';
    import * as HoverCard from "$lib/components/ui/hover-card/index";
</script>

<main class="h-screen w-screen overflow-hidden">
    <div class="flex justify-center items-center h-full w-full">
        <div class="w-72 text-start p-5">
            <div class="text-3xl font-semibold py-3">
                Verification 
            </div>
            <div class="text-start">
                hello, User we Send you link to your
                    <HoverCard.Root>
                        <HoverCard.Trigger>
                            <a href="/iamprathameshmore/dashboard">
                    <Button variant='link' size='default' class='px-1'>
                        Iamprathameshmore@gmail
                    </Button></a>
                    </HoverCard.Trigger>
                    <HoverCard.Content>
                      SvelteKit - Web development, streamlined
                    </HoverCard.Content>
                  </HoverCard.Root> 
       <br> click to this link and you are able to signin 
            </div>
        </div>
    </div>
</main>