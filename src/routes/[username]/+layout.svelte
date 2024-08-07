<script lang="ts">
  import Calculator from "lucide-svelte/icons/calculator";
  import Calendar from "lucide-svelte/icons/calendar";
  import CreditCard from "lucide-svelte/icons/credit-card";
  import Settings from "lucide-svelte/icons/settings";
  import Smile from "lucide-svelte/icons/smile";
  import User from "lucide-svelte/icons/user";
  import { onMount } from "svelte";
  import * as Avatar from "$lib/components/ui/avatar/index.js";
  import * as Command from "$lib/components/ui/command/index.js";
  import * as HoverCard from "$lib/components/ui/hover-card/index.js";
  import { Separator } from "$lib/components/ui/separator/index.js";
  import * as ContextMenu from "$lib/components/ui/context-menu/index.js";
  import Button from "$lib/components/ui/button/button.svelte";
  import * as Drawer from "$lib/components/ui/drawer";
  import { Description } from "$lib/components/ui/dialog";
  import ScrollArea from "$lib/components/ui/scroll-area/scroll-area.svelte";





  let bookmarks = false;
  let fullUrls = true;

  const profileRadioValue = "benoit";

  let showBookmarks = false;
  let showFullURLs = true;

  let value = "pedro";

  let open = false;

  onMount(() => {
    function handleKeydown(e: KeyboardEvent) {
      if (e.key === "m" && (e.metaKey || e.ctrlKey)) {
        e.preventDefault();
        open = !open;
      }
    }

    document.addEventListener("keydown", handleKeydown);
    return () => {
      document.removeEventListener("keydown", handleKeydown);
    };
  });
let data = 'https://avatars.githubusercontent.com/u/91453437?v=4'
  export const prerender = true;
</script>

<svelte:head>
  <link rel="icon" href={data ? data: '%sveltekit.assets%/favicon.png' }  type="image/png"   style="border-radius: 50%;" />
</svelte:head>


<div class="h-screen w-screen overflow-hidden">
  <div class="hidden md:block">
    <nav
    class="w-full py-2 bg-gray-50 flex justify-between items-center border-b-2  px-7 2xl:px-56 lg:px-28 "
  >
    <div class="left-5 flex">
      <div class="flex justify-start items-center">
        <div>
          <Avatar.Root>
            <Avatar.Image
              src="https://avatars.githubusercontent.com/u/91453437?v=4"
              alt="@shadcn"
            />
            <Avatar.Fallback>CN</Avatar.Fallback>
          </Avatar.Root>
        </div>

        <div class="ml-3">
          <HoverCard.Root>
            <HoverCard.Trigger ><a href="/Iamprathameshmore">Iamprathameshmore</a></HoverCard.Trigger>
            <HoverCard.Content>
              SvelteKit - Web development, streamlined
            </HoverCard.Content>
          </HoverCard.Root>
        </div>
      </div>
      <Separator orientation="vertical" class=" mx-5 bg-black my-2" />
      <div class="flex justify-center items-center">
        <ul class="flex justify-center items-center ml-0">
          <li>
            <a href="/[username]/dashboard"><Button variant='link' class='p-2'>Dashboard</Button></a>
          </li>
          <li>
            <a href="/[username]/email"><Button variant='link' class='p-2'>
            
              Email
            </Button></a>
          </li>
          <li>
            <a href="/[username]/social"><Button variant='link' class='p-2'>
            
              Social
             </Button></a>
          </li>
          <li>
            <a href="/[username]/workflow"><Button variant='link' class='p-2'>
            
              Workflow
            </Button></a>
        </li>
          <li><a href="/[username]/managment"><Button variant='link' class='p-2'>
            
            Managment
          </Button></a></li>
          <li><a href="/[username]/settings"><Button variant='link' class='p-2'>
            
            Settings
          </Button></a></li>
        </ul>
      </div>
    </div>
    <!-- <div class="hidden xl:block">
      <Button class='bg-gray-300 rounded-lg w-48 justify-between items-center' size='sm' variant='outline'><p>Search</p> <div class="text-center px-2 bg-zinc-50 rounded py-0.5 "> Ctrl + M</div></Button>
    </div> -->
  </nav>
  </div>

  <div>
    <nav class="bottom-0 right-0 w-full flex justify-between items-center md:hidden fixed p-5 z-10 bg-gray-100 border-t-2">
      <div class="flex justify-start items-center">
        <div>
          <Avatar.Root>
            <Avatar.Image
              src="https://avatars.githubusercontent.com/u/91453437?v=4"
              alt="@shadcn"
            />
            <Avatar.Fallback>CN</Avatar.Fallback>
          </Avatar.Root>
        </div>

        <div class="ml-3">
          Iamprathameshmore
            
        </div>
      </div>
      <div>
        <Drawer.Root >
          <Drawer.Trigger>Menu</Drawer.Trigger>
          <Drawer.Content class='block md:hidden'>
            <Drawer.Header class='text-start mb-0 pb-0'>
            
              
              <Drawer.Title>
                <div class="flex justify-start items-center">
                  <div>
                    <Avatar.Root>
                      <Avatar.Image
                        src="https://avatars.githubusercontent.com/u/91453437?v=4"
                        alt="@shadcn"
                      />
                      <Avatar.Fallback>CN</Avatar.Fallback>
                    </Avatar.Root>
                  </div>
          
                  <div class="ml-3">
                    Iamprathameshmore
                      
                  </div>
                </div>
            </Drawer.Title>

            <!-- <Drawer.Description class='m-0 p-0'>Menu</Drawer.Description> -->

            </Drawer.Header>
            <Drawer.Footer class=''>
              <!-- <div class='my-2'>Menu</div> -->
              <Drawer.Close><a href="/[username]/dashboard"><Button class='w-full'>Dashboard</Button></a></Drawer.Close>
              <Drawer.Close><a href="/[username]/email"><Button class='w-full'>Email</Button></a></Drawer.Close>
              <Drawer.Close><a href="/[username]/social"><Button class='w-full'>Social</Button></a></Drawer.Close>
              <Drawer.Close><a href="/[username]/workflow"><Button class='w-full'>Workflows</Button></a></Drawer.Close>
              <Drawer.Close><a href="/[username]/settings"><Button class='w-full'>Settings</Button></a></Drawer.Close>
              <Drawer.Close>Cancel</Drawer.Close>
            </Drawer.Footer>
          </Drawer.Content>
        </Drawer.Root>
      </div>

    </nav>
  </div>
  <main  class="block md:hidden 2xl:mx-64 lg:mx-28 m-5 mb-36">
    <slot />
  </main>
  <div class="hidden md:block">
    <ContextMenu.Root >
      <ContextMenu.Trigger>
        <main class="w-screen h-screen">
          <ScrollArea class='h-screen'>
          <div class="2xl:mx-56 lg:mx-28 mb-36 m-5" >
            <slot />
          </div>
        </ScrollArea>
        </main>
      </ContextMenu.Trigger>
      <ContextMenu.Content class="w-64">
        <ContextMenu.Item inset>
          Back
          <ContextMenu.Shortcut>⌘[</ContextMenu.Shortcut>
        </ContextMenu.Item>
        <ContextMenu.Item inset>
          Forward
          <ContextMenu.Shortcut>⌘]</ContextMenu.Shortcut>
        </ContextMenu.Item>
        <ContextMenu.Item inset>
          Reload
          <ContextMenu.Shortcut>⌘R</ContextMenu.Shortcut>
        </ContextMenu.Item>
        <ContextMenu.Sub>
          <ContextMenu.SubTrigger inset>More Tools</ContextMenu.SubTrigger>
          <ContextMenu.SubContent class="w-48">
            <ContextMenu.Item>
              Save Page As...
              <ContextMenu.Shortcut>⇧⌘S</ContextMenu.Shortcut>
            </ContextMenu.Item>
            <ContextMenu.Item>Create Shortcut...</ContextMenu.Item>
            <ContextMenu.Item>Name Window...</ContextMenu.Item>
            <ContextMenu.Separator />
            <ContextMenu.Item>Developer Tools</ContextMenu.Item>
          </ContextMenu.SubContent>
        </ContextMenu.Sub>
        <ContextMenu.Separator />
        <ContextMenu.CheckboxItem bind:checked={showBookmarks}>
          Show Bookmarks Bar
          <ContextMenu.Shortcut>⌘⇧B</ContextMenu.Shortcut>
        </ContextMenu.CheckboxItem>
        <ContextMenu.CheckboxItem bind:checked={showFullURLs}>
          Show Full URLs
        </ContextMenu.CheckboxItem>
        <ContextMenu.Separator />
        <ContextMenu.RadioGroup bind:value>
          <ContextMenu.Label inset>People</ContextMenu.Label>
          <ContextMenu.Separator />
          <ContextMenu.RadioItem value="pedro">Pedro Duarte</ContextMenu.RadioItem
          >
          <ContextMenu.RadioItem value="colm">Colm Tuite</ContextMenu.RadioItem>
        </ContextMenu.RadioGroup>
      </ContextMenu.Content>
    </ContextMenu.Root>
  </div>

  <Command.Dialog bind:open>
    <Command.Input placeholder="Type a command or search..." />
    <Command.List>
      <Command.Empty>No results found.</Command.Empty>
      <Command.Group heading="Suggestions">
        <Command.Item>
          <Calendar class="mr-2 h-4 w-4" />
          <span>Calendar</span>
        </Command.Item>
        <Command.Item>
          <Smile class="mr-2 h-4 w-4" />
          <span>Search Emoji</span>
        </Command.Item>
        <Command.Item>
          <Calculator class="mr-2 h-4 w-4" />
          <span>Calculator</span>
        </Command.Item>
      </Command.Group>
      <Command.Separator />
      <Command.Group heading="Settings">
        <Command.Item>
          <User class="mr-2 h-4 w-4" />
          <span>Profile</span>
          <Command.Shortcut>⌘P</Command.Shortcut>
        </Command.Item>
        <Command.Item>
          <CreditCard class="mr-2 h-4 w-4" />
          <span>Billing</span>
          <Command.Shortcut>⌘B</Command.Shortcut>
        </Command.Item>
        <Command.Item>
          <Settings class="mr-2 h-4 w-4" />
          <span>Settings</span>
          <Command.Shortcut>⌘S</Command.Shortcut>
        </Command.Item>
      </Command.Group>
    </Command.List>
  </Command.Dialog>
</div>
