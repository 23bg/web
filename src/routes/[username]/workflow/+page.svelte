<script>
    import Button from "$lib/components/ui/button/button.svelte";
    import Separator from "$lib/components/ui/separator/separator.svelte";
    import ScrollArea from "$lib/components/ui/scroll-area/scroll-area.svelte";
    import { Input } from "$lib/components/ui/input";
    import * as Breadcrumb from "$lib/components/ui/breadcrumb/index";
    import Workflow from '$lib/custome/workflowcard/workflowCard.svelte'
  import WorkflowCard from "$lib/custome/workflowcard/workflowCard.svelte";

  let arr = Array(100)
  </script>
  
  <main class="w-full h-full">

      <div class="">
      <div class="my-7 w-full ">
        <Breadcrumb.Root class='mb-5 mx-1'>
            <Breadcrumb.List>
              <Breadcrumb.Item>
                <Breadcrumb.Link href='/[username]/dashboard'>Iamprathameshmore</Breadcrumb.Link>
              </Breadcrumb.Item>
              <Breadcrumb.Separator />
              <Breadcrumb.Item>
                <Breadcrumb.Link href="/[username]/workflow">Workflow</Breadcrumb.Link>
              </Breadcrumb.Item>
              <Breadcrumb.Separator />

            </Breadcrumb.List>
          </Breadcrumb.Root>
          <div class="text-4xl font-medium">Workflows</div>
          <p class="mx-1 my-3">Build, test, and deploy your code. Make code reviews, branch management, and issue triaging work the way you want. Select a workflow to get started.</p>
          <p class="mx-1 my-3">Skip this and <span class="text-indigo-600"> set up a workflow yourself</span> </p>

          <div>
            <Input size={52} prefix={'hello form '} class='w-64 bg-gray-200 border-transparent h-8' placeholder='Search Your Workflow'/>
          </div>
        </div> 
       
        <div >
          
    
  
          <div class="grid xl:grid-cols-4 gap-2 md:grid-cols-3  sm:grid-cols-2 grid-cols-1">
      
            {#each arr as arr}
               <div>
                <WorkflowCard/>
               </div>
            {/each}
    
          </div>
      </div>
  </div>

  </main>
  