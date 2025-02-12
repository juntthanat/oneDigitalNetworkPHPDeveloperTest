<script></script>

<template>
  <div id="title">Nomad [E]</div>
  <div id="descriptionContainer">
    <div id="titleDescription">
      Know Productivity - Efficiency - Passion - Creativity with no limits. A
      crisp IPS display boasts everything from pomodoro timer, to a playful
      Tamagotchi-style companion, a trusty clock and much more.
    </div>
    <div>
      <div className="subtitle">Backed by science</div>
      <div className="subtitleDescription">
        The integrated pomodoro timer leverages a scientifically proven
        work/rest methodology that is adaptable to any workflow - empowering you
        to accomplish more in less time.
      </div>
    </div>
    <div>
      <div className="subtitle">Mechanical & hotswap</div>
      <div className="subtitleDescription">
        We redesigned our custom keycaps to hug your fingertips even more
        perfectly than before. Mounted on our custom tuned “Atomic” MX Gateron
        hotswap switches, so you can try different switches without needing to
        desolder them.
      </div>
    </div>
  </div>
</template>

<style>
#title {
  font-size: 22px;
  font-weight: 600;
  height: 34px;
  width: 325px;
  margin-bottom: 16px;
}
#descriptionContainer {
  display: flex;
  flex-direction: column;
  gap: 24px;
}
#titleDescription {
  font-size: 18px;
  font-weight: 400;
  line-height: 26px;
}
.subtitle{
  font-size: 18px;
  font-weight: 600;
  line-height: 26px;
}
.subtitleDescription{
  font-size: 18px;
  font-weight: 400;
  line-height: 26px;
}
</style>
