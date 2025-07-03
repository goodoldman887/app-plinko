<script lang="ts">
  import rating from '$lib/assets/rating.svg';
  import _1red from '$lib/assets/1Red.webp';
  import _31bets from '$lib/assets/31 BETS.webp';
  import _7bets from '$lib/assets/7bets.webp';
  import _7gold from '$lib/assets/7Gold.webp';
  import _amonbet from '$lib/assets/Amonbet.webp';
  import _betfoxx from '$lib/assets/BetFoxx.webp';
  import _betmac from '$lib/assets/Betmac.webp';
  import _betnuvo from '$lib/assets/Betnuvo.webp';
  import _betti from '$lib/assets/Betti.webp';
  import _betzino from '$lib/assets/Betzino.webp';
  import _bigwins from '$lib/assets/Big Wins.webp';
  import _casobet from '$lib/assets/Casobet.webp';
  import _cosmobet from '$lib/assets/CosmoBet.webp';
  import _donbet from '$lib/assets/Donbet.webp';
  import _fortunica from '$lib/assets/Fortunica.webp';
  import _goldenlion from '$lib/assets/Golden Lion.webp';
  import _jackbit from '$lib/assets/Jackbit.webp';
  import _mystake from '$lib/assets/MyStake.webp';
  import _ninbet from '$lib/assets/NinBet.webp';
  import _pitbet from '$lib/assets/Pitbet.webp';
  import _qbet from '$lib/assets/Qbet.webp';
  import _rolletto from '$lib/assets/Rolletto.webp';
  import _spinmillion from '$lib/assets/Spin Million.webp';
  import _velobet from '$lib/assets/VeloBet.webp';
  import _winitbet from '$lib/assets/WinitBet.webp';
</script>

<!-- Начало витрины -->
<div class="showcase__wrapper">
  <!-- CosmoBet -->
  <div class="showcase">
    <div class="showcase__link">
      <div class="showcase__item">
        <div class="showcase__img"><img src={_cosmobet} alt="CosmoBet" /></div>
        <div class="showcase__title"><span>CosmoBet</span></div>
      </div>
      <div class="showcase__item showcase__item-right">
        <div class="showcase__rating">
          {#each Array(5) as _}
            <div class="showcase__rating-item"><img src={rating} alt="rating" /></div>
          {/each}
        </div>
        <div class="showcase__btn" style="cursor: pointer" on:click={() => window.location.href = 'https://applogic.top/5TRb1N'}>
          Play
        </div>
      </div>
    </div>
  </div>

  <!-- Fortunica -->
  <div class="showcase">
    <div class="showcase__link">
      <div class="showcase__item">
        <div class="showcase__img"><img src={_fortunica} alt="Fortunica" /></div>
        <div class="showcase__title"><span>Fortunica</span></div>
      </div>
      <div class="showcase__item showcase__item-right">
        <div class="showcase__rating">
          {#each Array(5) as _}
            <div class="showcase__rating-item"><img src={rating} alt="rating" /></div>
          {/each}
        </div>
        <div class="showcase__btn" style="cursor: pointer" on:click={() => window.location.href = 'https://applogic.top/5TRb1N'}>
          Play
        </div>
      </div>
    </div>
  </div>

  <!-- Jackbit -->
  <div class="showcase">
    <div class="showcase__link">
      <div class="showcase__item">
        <div class="showcase__img"><img src={_jackbit} alt="Jackbit" /></div>
        <div class="showcase__title"><span>Jackbit</span></div>
      </div>
      <div class="showcase__item showcase__item-right">
        <div class="showcase__rating">
          {#each Array(5) as _}
            <div class="showcase__rating-item"><img src={rating} alt="rating" /></div>
          {/each}
        </div>
        <div class="showcase__btn" style="cursor: pointer" on:click={() => window.location.href = 'https://applogic.top/5TRb1N'}>
          Play
        </div>
      </div>
    </div>
  </div>
</div>
<!-- Конец витрины -->

<style>
  :global(.showcase__wrapper) {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    padding-top: 1.5rem;
    padding-bottom: 1.5rem;
  }


  :global(.showcase) {
    background: #1c1a4b;
    border-radius: 0.5rem;
    overflow: hidden;
  }

  :global(.showcase__link) {
    display: flex;
    justify-content: space-between;
    align-items: center;
    text-decoration: none;
  }

  :global(.showcase__item) {
    padding: 1rem;
    display: flex;
    align-items: center;
  }

  :global(.showcase__item-right) {
    background: #151533;
    display: flex;
    align-items: center;
    padding: 1rem;
  }

  :global(.showcase__img img) {
    height: 40px;
    width: auto;
    border-radius: 0.25rem;
  }

  :global(.showcase__title span) {
    margin-left: 0.5rem;
    font-weight: 600;
    color: #ffffff;
    font-size: 1rem;
  }

  :global(.showcase__rating) {
    display: flex;
    gap: 0.25rem;
  }

  :global(.showcase__rating-item img) {
    height: 16px;
    width: 16px;
  }

  :global(.showcase__btn) {
    background: #5b6cff;
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 0.375rem;
    font-weight: 600;
    margin-left: 0.5rem;
  }

  :global(.showcase__btn:hover) {
    background: #1e4bb8;
  }
</style>