<script>
  // @ts-nocheck

  import Button from "$lib/components/ui/button/button.svelte";
  import Separator from "$lib/components/ui/separator/separator.svelte";
  import ScrollArea from "$lib/components/ui/scroll-area/scroll-area.svelte";
  import { Input } from "$lib/components/ui/input";
  import * as Breadcrumb from "$lib/components/ui/breadcrumb/index";
  import Socialmediacard from "$lib/custome/socialmedia/socialmediacard.svelte";
  let arr = new Array(100);
</script>

<main class="w-full h-full">
  <div class=" ">
    <div class="my-7 w-full">
      <Breadcrumb.Root class="mb-5 mx-1">
        <Breadcrumb.List>
          <Breadcrumb.Item>
            <Breadcrumb.Link>Iamprathameshmore</Breadcrumb.Link>
          </Breadcrumb.Item>
          <Breadcrumb.Separator />
          <Breadcrumb.Item>
            <Breadcrumb.Link href="/">Social</Breadcrumb.Link>
          </Breadcrumb.Item>
          <Breadcrumb.Separator />
        </Breadcrumb.List>
      </Breadcrumb.Root>

      <div class="text-4xl font-medium">Social Media Control</div>
      <p class="mx-1 my-3">
        Build, test, and deploy your code. Make code reviews, branch management,
        and issue triaging work the way you want. Select a workflow to get
        started.
      </p>
      <p class="mx-1 my-3">
        Skip this and <span class="text-indigo-600">
          set up a workflow yourself</span
        >
      </p>

      <div class="flex justify-center items-start mb-28 my-5">
        <div>
          <div class="hidden md:block mr-2 border-2 bg-gray-50 p-5 rounded-lg">
            <div class="h-full flex-col justify-start items-start w-64">
              <div class="my-2">
                <h1 class="text-md font-semibold">Perosnal Settings</h1>
                <Separator class="my-2 pr-4 h-0.5" />
                <ul class="">
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>

                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                </ul>
              </div>
              <div class="my-2">
                <h1 class="text-md font-semibold">Password And Security</h1>
                <Separator class="my-2 pr-4" />
                <ul class="">
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                </ul>
              </div>
              <div class="my-2">
                <h1 class="text-md font-semibold">
                  Code, planning, and automation
                </h1>
                <Separator class="my-2 pr-4 h-0.5" />
                <ul class="">
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                  <li>
                    <a href="/"
                      ><Button
                        variant="ghost"
                        class="flex w-full justify-start hover:bg-gray-300"
                        >hello</Button
                      ></a
                    >
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>

        <div class="w-full h-full">
       
          <div
          class="grid gap-3 xl:grid-cols-4 lg:grid-cols-3 sm:grid-cols-2 w-full"
        >
           {#each arr as arr}
          
            <Socialmediacard
            url={"https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/636e0a69f118df70ad7828d4_icon_clyde_blurple_RGB.svg"}
            social={"discrod"}
           />
           {/each}
          </div>
        </div>
      </div>
    </div>
  </div>
</main>
