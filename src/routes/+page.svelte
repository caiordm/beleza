<script>
    import Header from "$lib/Header.svelte";
    import {
    IconArrowAutofitContent,
        IconArrowRight,
        IconBraces,
        IconBrandInstagramFilled,
        IconBrandTwitter,
        IconBrandTwitterFilled,
        IconBrandYoutubeFilled,
        IconDiamond,
        IconMedal,
        IconRings,
    } from "@tabler/icons-svelte";
    import ServicoCard from "$lib/ServicoCard.svelte";
    import Footer from "$lib/Footer.svelte";
    import SeparatorLanding from "$lib/SeparatorLanding.svelte";
    import ProdutoLanding from "$lib/ProdutoLanding.svelte";
    // images
    import banner from "../images/banner.png";
    import corte1 from "../images/corte1.jpeg";
    import novidades from "../images/novidades.png"
    import cartierLogo from "../images/Catier.png"
    import gucciLogo from "../images/Gucci.png"
    import tiffanyLogo from "../images/Tiffany.png"
    import novidades2 from "../images/novidades2.png"
    import product1 from "../images/product1.png"
    import logo from "../images/logo.png"
</script>

<main>
    <header>
        <Header />
    </header>

    <section id="main_content" class="flex flex-col items-center bg-slate-50">
        <div id="banner" class="w-full flex flex-col items-center">
            <img src={banner} alt="Banner" class="w-full" />
            <a
                href="#"
                class="relative bottom-16 px-6 py-2 rounded-full text-white text-lg bg-gray-700 bg-clip-padding backdrop-filter backdrop-blur-xl bg-opacity-0"
                >EXPLORAR COLEÇÃO</a
            >
        </div>

        <div id="servicos" class="w-full pb-4 flex flex-col gap-6 items-center">
            <h2 class="text-2xl tracking-widest">SERVIÇOS</h2>
            <nav class="w-4/5 flex justify-around text-lg text-slate-500">
                <button class="text-slate-700 underline underline-offset-8">Tudo</button>
                <button>Pele</button>
                <button>Lábios</button>
                <button>Sobrancelhas</button>
            </nav>
            <div class="w-full flex flex-wrap items-center justify-center gap-4">
                <ServicoCard image={corte1} text='Micropigmentação Labial'/>
                <ServicoCard image={corte1} text='Limpeza de Pele'/>
                <ServicoCard image={corte1} text='Micropigmentação de sobrancelha'/>
                <ServicoCard image={corte1} text='Técnica Fio a Fio'/>
            </div>
            <a href="#" class="flex items-center">Explore mais <IconArrowRight/></a>
        </div>

        <SeparatorLanding/>

        <div id="marcas" class="w-full pb-4 flex flex-col gap-6 items-center">
            <h2 class="text-lg tracking-widest">MAGCOLORPIGMENTOS</h2>
            <div class="w-full px-4 flex flex-wrap items-center justify-center gap-6">
                <img src={cartierLogo} alt="Cartier">
                <img src={gucciLogo} alt="Gucci">
                <img src={tiffanyLogo} alt="Tiffany">
            </div>
        </div>

        <SeparatorLanding/>
        
        <div id="novidades" class="w-full pb-4 flex flex-col gap-6 items-center">
            <h2 class="text-2xl tracking-widest">NOVIDADES</h2>
            <div class="w-full flex flex-col gap-2">
                <img src={novidades} alt="Curso">
                <img src={novidades2} alt="Video Image">
            </div>
        </div>
        
        <SeparatorLanding/>

        <div id="produtos" class="w-full pb-4 flex flex-col gap-6 items-center">
            <h2 class="text-2xl tracking-widest">PRODUTOS</h2>
            <div class="w-full flex overflow-x-auto items-center justify-center gap-4 pl-[35%] py-4">
                <ProdutoLanding image={product1} title='Harris Tweed Three button Jacket' price='120'/>
                <ProdutoLanding image={product1} title='Harris Tweed Three button Jacket' price='120'/>
                <ProdutoLanding image={product1} title='Harris Tweed Three button Jacket' price='120'/>
                <ProdutoLanding image={product1} title='Harris Tweed Three button Jacket' price='120'/>
            </div>
            <a href="#" class="flex items-center">Explore mais <IconArrowRight/></a>
        </div>

        <div id="tendencias" class="w-full bg-slate-100 py-4 flex flex-col gap-2 items-center">
            <h2 class="text-2xl tracking-widest">@TENDÊNCIAS</h2>
            <div class="w-full flex flex-wrap items-center justify-start gap-2 py-4 px-8">
                <a href="#" class="px-4 py-2 text-slate-700 bg-white rounded-full">#2025</a>
                <a href="#" class="px-4 py-2 text-slate-700 bg-white rounded-full">#beleza</a>
                <a href="#" class="px-4 py-2 text-slate-700 bg-white rounded-full">#produtos</a>
                <a href="#" class="px-4 py-2 text-slate-700 bg-white rounded-full">#pele</a>
                <a href="#" class="px-4 py-2 text-slate-700 bg-white rounded-full">#cilios</a>
                <a href="#" class="px-4 py-2 text-slate-700 bg-white rounded-full">#sobrancelhas</a>
                <a href="#" class="px-4 py-2 text-slate-700 bg-white rounded-full">#labios</a>
            </div>
        </div>

        <div id="espaco" class="w-full bg-slate-50 py-4 flex flex-col gap-8 items-center">
            <img src={logo} alt="Logo" class="max-w-40">
            <div class="w-full flex flex-wrap items-center justify-center gap-4 text-sm text-slate-500">
                <span class="flex flex-col items-center text-center justify-center gap-2 max-w-44">
                    <img src={gucciLogo} alt="Logo">
                    <p>Ambiente aconchegante e acolhedor</p>
                </span>
                <span class="flex flex-col items-center text-center justify-center gap-2 max-w-44">
                    <img src={gucciLogo} alt="Logo">
                    <p>Você merece o melhor todos os dias</p>
                </span>
                <span class="flex flex-col items-center text-center justify-center gap-2 max-w-44">
                    <img src={gucciLogo} alt="Logo">
                    <p>Espaços elegantes e sofisticados</p>
                </span>
                <span class="flex flex-col items-center text-center justify-center gap-2 max-w-44">
                    <img src={gucciLogo} alt="Logo">
                    <p>Meu momento nosso compromisso</p>
                </span>
            </div>
        </div>
    </section>

    <footer class="w-full px-4 pt-8 pb-2 gap-6 flex flex-col bg-rose-200">
        <div class="w-full px-8 flex justify-around">
            <IconBrandTwitterFilled size="32" color="#334155" />
            <IconBrandInstagramFilled size="32" color="#334155" />
            <IconBrandYoutubeFilled size="32" color="#334155" />
        </div>
        <div class="w-2/5 self-center flex items-center justify-center gap-2">
            <div class="w-20 border-b border-b-slate-500 border-solid"></div>
            <IconDiamond />
            <div class="w-20 border-b border-b-slate-500 border-solid"></div>
        </div>
        <div class="flex flex-col text-center">
            <a
                class="text-slate-700 text-lg"
                href="mailto:espaçopauladiniz@gmail.com"
                >espaçopauladiniz@gmail.com</a
            >
            <a class="text-slate-700 text-lg" href="tel:81992401038">
                (81) 99240-1038</a
            >
            <span class="text-slate-700 text-lg">
                08:00 - 22:00 de Segunda à Sexta
            </span>
        </div>
        <SeparatorLanding/>
        <nav class="flex justify-around text-lg px-4">
            <a href="#">Sobre</a>
            <a href="#">Contato</a>
            <a href="#">Blog</a>
        </nav>
        <div class="flex flex-col items-center text-slate-500 text-sm">
            <span>Copyright© espaçopauladiniz</span>
            <span>Todos os Direitos Reservados.</span>
        </div>
    </footer>
</main>
