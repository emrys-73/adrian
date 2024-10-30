<script>

    const menu = [
        {
            title: "Discover Avlana",
            url: "https://avlana.co/",
            active: true,
        },
        {
            title: "Instagram",
            url: "https://www.instagram.com/adrianmontoya00/",
            active: true,
        },
        {
            title: "The Vlog",
            url: "https://www.youtube.com/@life_of_adrian",
            active: true,
        },
        {
            title: "The Story",
            url: "/",
            active: false,
        },

    ]
</script>


<div class="w-full flex flex-col sm:bg-[url('/hero2.jpg')] bg-[url('/hero_phone.jpg')] bg-cover bg-center h-screen relative justify-center items-center px-4 sm:flex-row">
    <div class="bg-gradient-to-b from-transparent to-black h-screen z-10 opacity-50 absolute"></div>

    <!-- Absolutely centered Montoya -->
    <div class="text-6xl lg:text-7xl xl:text-9xl text-white sm:text-primary font-sans uppercase font-bold flex bottom-4 w-full justify-start transition-all duration-500 ease-in-out sm:absolute sm:top-4 sm:left-8 sm:text-7xl">
        Adrian
    </div>
    <div class="text-6xl lg:text-7xl xl:text-9xl text-white sm:text-primary font-sans uppercase font-bold flex bottom-4 w-full justify-end transition-all duration-500 ease-in-out sm:absolute sm:bottom-6 sm:justify-center sm:text-7xl">
        Montoya
    </div>
    <span class="text-white tracking-wider text-lg absolute top-6 sm:hidden uppercase font-bold ">
        Building a tech startup in public
    </span>

    <div class="w-full h-full min-h-screen bg-transparent sm:flex hidden">

    </div>

    <div class="w-full h-full min-h-screen justify-center sm:items-start items-center flex-col sm:px-16 gap-8 hidden sm:flex">
        <span class="text-white tracking-wider text-lg absolute top-6 sm:flex sm:relative sm:text-5xl md:text-6xl lg:text-7xl sm:text-secondary sm:justify-start sm:items-center uppercase font-bold sm:max-w-[35vw] sm:ml-12 md:ml-32 ">
            Building a tech startup in public
        </span>
        <div class="w-full sm:px-16 flex flex-col gap-0 sm:items-end sm:justify-center z-40">
            {#each menu as m}
                {#if m.active}
                    <a href={m.url} class="text-md hover:text-lg font-bold uppercase text-white opacity-80 hover:opacity-100 transition-all ease-in-out duration-300 hover:py-1 hover:underline">
                        {m.title}
                    </a>
                {/if}
            {/each}
        </div>
    </div>


    <div class="absolute bottom-6 justify-center flex-col items-center sm:flex sm:flex-col sm:justify-start">
        {#each menu as m}
            {#if m.active}
                <a href={m.url} class="text-md font-bold uppercase text-secondary opacity-80 hover:opacity-100 transition-all ease-in-out duration-300 hover:py-1 hover:underline flex justify-center sm:hidden">
                    {m.title}
                </a>
            {/if}
        {/each}
    </div>
    
</div>