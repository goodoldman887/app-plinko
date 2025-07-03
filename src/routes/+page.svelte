<script lang="ts">
  import logo from '$lib/assets/logo.svg';
  import Balance from '$lib/components/Balance.svelte';
  import LiveStatsWindow from '$lib/components/LiveStatsWindow/LiveStatsWindow.svelte';
  import Plinko from '$lib/components/Plinko';
  import SettingsWindow from '$lib/components/SettingsWindow';
  import Sidebar from '$lib/components/Sidebar';
  import CasinoShowcase from '$lib/components/CasinoShowcase.svelte';
  import { setBalanceFromLocalStorage, writeBalanceToLocalStorage } from '$lib/utils/game';
  

  $effect(() => {
    setBalanceFromLocalStorage();
  });
</script>

<style>
  /* Component spacing */
  .section {
    margin: 2rem 0;
  }

  /* Global styles */
  :global(body) {
    margin: 0;
    font-family: 'Inter', sans-serif;
    background: #111827;
    color: #e5e7eb;
  }

  /* Prose styling for description section */
  :global(section.prose) {
    background: #1f2937;
    padding: 2rem;
    border-radius: 0.5rem;
    box-shadow: 0 6px 10px rgba(0,0,0,0.4);
  }

  /* Heading sizes */
  :global(.prose h1) {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }
  :global(.prose h2) {
    margin-top: 2rem;
    border-bottom: 1px solid #2d3748;
    padding-bottom: 0.5rem;
    font-size: 1.75rem;
  }
  :global(.prose h3) {
    margin-top: 1.5rem;
    font-size: 1.25rem;
  }

  /* Table styling within prose */
  :global(.prose table) {
    width: 100%;
    border-collapse: collapse;
    text-align: center;
    margin: 0 auto;
  }
  :global(.prose th),
  :global(.prose td) {
    padding: 0.75rem;
    border: none;
  }
  :global(.prose thead) {
    background: #2d3748;
  }
  :global(.prose thead th) {
    font-weight: bold;
    color: #edf2f7;
  }
  :global(.prose tbody tr:nth-child(odd)) {
    background: #2a303c;
  }
  :global(.prose tbody tr:nth-child(even)) {
    background: #1f2937;
  }
</style>

<div class="relative flex min-h-dvh w-full flex-col bg-gray-900 text-gray-100">
  <!-- Navigation -->
  <nav class="sticky top-0 z-10 w-full bg-gray-800 px-5 py-3 drop-shadow-md">
  <div class="relative mx-auto flex h-14 max-w-7xl items-center">
    <!-- Logo on the left -->
    <img src={logo} alt="logo" class="h-6 sm:h-7" />
    <!-- Balance centered -->
    <div class="absolute left-1/2 top-1/2 transform -translate-x-1/2 -translate-y-1/2">
      <Balance />
    </div>
  </div>
</nav>

  <!-- Main Content -->
  <main class="flex-1">
    <div class="mx-auto w-full max-w-7xl px-5">
    <!-- 1. Demo at the top -->
    <section id="plinko-demo" class="section demo px-5">
      <div class="mx-auto mt-5 min-w-[300px] max-w-xl drop-shadow-xl md:mt-10 lg:max-w-7xl">
        <div class="flex flex-col-reverse overflow-hidden rounded-lg lg:w-full lg:flex-row">
          <Sidebar />
          <div class="flex-1"><Plinko /></div>
        </div>
      </div>
    </section>

    <!-- 2. Showcase under the demo -->
    <section class="section showcase mx-auto px-5 mt-8 min-w-[300px] max-w-xl md:mt-10 lg:max-w-7xl">
      <CasinoShowcase />
    </section>

    <!-- 3. Description section -->
  <!-- Full provided text translated to English -->


<section id="description" class="prose prose-invert section description mx-auto w-full max-w-7xl">
<h1 id="intro">Plinko Cassino: Visão Geral e Regras do Jogo</h1>
<p>Explore agora mesmo o universo vibrante do Plinko! Para começar, crie sua conta no site oficial, aproveite o bônus de boas-vindas e consulte as respostas para todas as suas dúvidas nas seções detalhadas abaixo.</p>
<h2 id="quick-info">Informações Rápidas do Jogo</h2>
<table><thead><tr><th>Item</th><th>Detalhes</th></tr></thead><tbody><tr><td>🌐 Site Oficial</td><td>www.plinko.org</td></tr><tr><td>🎮 Tipo de Jogo</td><td>Apostas, Slot</td></tr><tr><td>💻 Plataformas</td><td>Stake, Roobet, e outros cassinos online</td></tr><tr><td>⚙️ Funcionamento</td><td>Movimento aleatório da ficha por uma estrutura de pinos</td></tr><tr><td>🎯 Objetivo</td><td>Ficha rebate nos pinos e para em um compartimento de prêmio</td></tr><tr><td>💵 Apostas</td><td>Moedas fiduciárias e criptomoedas</td></tr><tr><td>🎲 Níveis de Risco</td><td>Baixo, Médio, Alto</td></tr><tr><td>🆓 Versão Grátis</td><td>Disponível na maioria dos sites</td></tr><tr><td>🔑 Funcionalidades</td><td>Login fácil, versões variadas, bônus diversos</td></tr></tbody></table>
<h2 id="how-to-start">Como Começar a Jogar Plinko</h2>
<ol><li><strong>Defina a Aposta:</strong> Escolha o valor da ficha antes de iniciar—isso influencia seus ganhos.</li><li><strong>Escolha o Nível de Risco:</strong> Baixo, médio ou alto—o risco altera os multiplicadores e a volatilidade.</li><li><strong>Solte a Ficha:</strong> Clique em “Iniciar” e acompanhe a trajetória da ficha.</li><li><strong>Receba o Prêmio:</strong> Assim que a ficha parar em um compartimento, receba o valor multiplicado pelo prêmio correspondente.</li></ol>
<h2 id="general-info">Informações Gerais Sobre o Plinko Online</h2>
<ul><li><strong>Sorte e Estratégia:</strong> O caminho da ficha é imprevisível, mas a escolha do risco traz um toque de estratégia.</li><li><strong>Diversidade de Formatos:</strong> A quantidade de pinos e prêmios varia conforme o site; alguns oferecem animações e minijogos.</li><li><strong>Uso de Criptomoedas:</strong> Depósitos e saques imediatos via Bitcoin, Ethereum e outras moedas digitais.</li><li><strong>RNG Confiável:</strong> Cassinos licenciados utilizam geradores de números aleatórios certificados para garantir justiça.</li><li><strong>Licenciamento:</strong> Dê preferência a plataformas legais e regulamentadas para jogar com segurança.</li></ul>
<h2 id="reviews">Opinião dos Jogadores</h2>
<ul><li>Equilíbrio interessante entre riscos e recompensas.</li><li>Chance de grandes prêmios em uma só rodada.</li><li>Interface intuitiva para iniciantes e experientes.</li></ul>
<h2 id="strategies">Dicas e Estratégias</h2>
<ul><li><strong>Aposta Fixa:</strong> Mantenha o valor das apostas estável para controlar possíveis perdas.</li><li><strong>Martingale:</strong> Dobre o valor após perder e volte ao valor inicial após ganhar. Exige saldo alto.</li><li><strong>Anti-Martingale:</strong> Aumente a aposta após ganhar e diminua após perder para aproveitar sequências positivas.</li><li><strong>Modo Grátis:</strong> Treine sem riscos para experimentar diferentes estratégias e níveis de risco.</li><li><strong>Gestão de Banca:</strong> Defina limites de ganhos e perdas para não ultrapassar seu orçamento.</li></ul>
<h2 id="versions">Diferentes Versões do Plinko</h2>
<ul><li><strong>Plinko Slot:</strong> Une a dinâmica do Plinko com recursos de caça-níquel, como bônus e símbolos especiais.</li><li><strong>Plinko Cripto:</strong> Anonimato e transações rápidas via blockchain, além de promoções exclusivas em cripto.</li><li><strong>Variações por Desenvolvedor:</strong> BGaming traz gráficos vibrantes; Spribe oferece recursos interativos e bônus únicos.</li></ul>
<h2 id="getting-started">Como Iniciar no Plinko</h2>
<ol><li>Analise as plataformas conferindo licenças, avaliações e métodos de pagamento.</li><li>Cadastre-se e faça a verificação, se solicitado.</li><li>Escolha entre modo de demonstração e apostas reais.</li><li>Adicione saldo via cartão, carteira digital ou criptomoeda.</li><li>Configure valor da ficha e nível de risco.</li><li>Solte a ficha e divirta-se!</li></ol>
<h2 id="recommendations">Recomendações Importantes</h2>
<ul><li>Jogue com responsabilidade, estipulando limites de tempo e de valor.</li><li>Aproveite promoções—bônus de boas-vindas e giros grátis aumentam seu saldo.</li><li>Confira opiniões de outros usuários antes de escolher onde jogar.</li></ul>
<h2 id="real-money">Plinko com Dinheiro Real</h2>
<p>Apostar dinheiro de verdade deixa o Plinko ainda mais emocionante:</p>
<ul><li>O valor pago depende do tamanho da aposta, risco escolhido e multiplicador do prêmio.</li><li>Bônus e giros grátis ampliam suas chances ao oferecer créditos extras.</li><li>Prefira sempre cassinos legalizados para garantir sua segurança.</li></ul>
<h2 id="demo-mode">Modo de Demonstração</h2>
<p>Aproveite o modo grátis para:</p>
<ul><li>Compreender o funcionamento dos saltos da ficha.</li><li>Observar como os prêmios mudam de acordo com o risco.</li><li>Experimentar estratégias sem gastar dinheiro.</li></ul>
<h2 id="faq">Perguntas Frequentes</h2>
<h3>O que é o Plinko Cassino?</h3><p>Trata-se de um jogo de apostas onde uma ficha cai em um tabuleiro de pinos, e o prêmio depende de onde ela para.</p><h3>É legalizado?</h3><p>A legalidade varia conforme o país e licenciamento do site. Sempre verifique as normas locais antes de se cadastrar.</p><h3>É possível ganhar mesmo?</h3><p>Sim, com sorte e uma boa gestão de saldo.</p><h3>Vale a pena usar criptomoeda?</h3><p>Criptomoedas garantem anonimato e rapidez, mas exigem conhecimento básico de blockchain.</p><h3>Existem estratégias?</h3><p>Apesar do resultado ser aleatório, optar por níveis de risco e controlar as apostas pode minimizar perdas.</p>
</section>
      </div>
</main>

  <!-- Modals -->
  <SettingsWindow />
  <LiveStatsWindow />

  <!-- Footer -->
  <footer class="px-5 pt-16 pb-4 text-sm text-gray-400">
    <div class="mx-auto max-w-4xl">
      <div aria-hidden="true" class="h-px bg-gray-700 mb-4"></div>
      <div class="flex justify-end">
        <a href="https://github.com/goodoldman887/plinko_game" target="_blank" class="hover:opacity-75">
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" viewBox="0 0 24 24">
            <path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 17.07 3.633 16.7 3.633 16.7c-1.087-.743.084-.728.084-.728 1.205.084 1.84 1.237 1.84 1.237 1.07 1.835 2.809 1.305 3.495.998.108-.776.418-1.305.762-1.605-2.665-.3-5.467-1.332-5.467-5.93 0-1.31.47-2.38 1.236-3.22-.124-.303-.536-1.523.117-3.176 0 0 1.008-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.29-1.552 3.297-1.23 3.297-1.23.654 1.653.242 2.873.118 3.176.77.84 1.235 1.91 1.235 3.22 0 4.61-2.804 5.628-5.475 5.922.43.37.823 1.102.823 2.222 0 1.606-.014 2.896-.014 3.286 0 .32.218.694.825.576C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/>
          </svg>
        </a>
      </div>
    </div>
  </footer>
</div>
