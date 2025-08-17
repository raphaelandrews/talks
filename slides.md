---
layout: center
highlighter: shiki
css: unocss
colorSchema: dark
transition: fade-out
title: Gestão da Qualidade
lineNumbers: false
drawings:
  persist: false
mdc: true
clicks: 0
preload: false
glowSeed: 200
routerMode: hash
class: flex justify-center items-center gap-20 px-40 text-xl
---

<div translate-x--35>

# Cultura e Liderança

Gestão da Qualidade

</div>

<style>
  h1 {
    font-weight: bold
  }
</style>

---
class: flex justify-center items-center gap-20 px-40 text-xl
clicks: 2
glowSeed: 203
---

<div
  absolute text-6xl
  :class="$clicks < 1 ? 'text-white' : 'translate-y--18 scale-40 text-white/30'"
  transition duration-500 ease-in-out
>
  <span transition="all 1000! ease-in-out" :class="$clicks > 1 ? 'opacity-0' : ''">🎭 Cultura da Liderança</span>
</div>

<div flex flex-col items-center>
  <v-clicks>
    <div mt-4 transition="all ease-in-out" flex items-center
      duration-1500 :class="$slidev.nav.clicks > 1 ? 'translate-x-[-260px] translate-y-[-218px]' : ''">
      <h1 flex items-center font-bold transition="all duration-1000 ease-in-out" :class="$slidev.nav.clicks > 1 ? 'text-3xl!' : 'text-5xl!'">
        <span>✳️ Principais Características</span>
      </h1>
    </div>
  </v-clicks>
</div>

---
glowSeed: 203
---

<div flex="row ~" w-full justify-between>
  <div>
    <div text-left w-full h-full flex="~ col justify-center">
      <div class="font-bold text-3xl mb-8">✳️ Principais Características</div>
        <div class="space-y-2 list-decimal pl-4">
          <div v-click>🎯 Foco no cliente interno e externo</div>
          <div v-click>📈 Compromisso com a melhoria contínua</div>
          <div v-click>✅ Valorização da padronização de processos</div>
          <div v-click>🎉 Incentivo à participação e envolvimento de todos os colaboradores</div>
          <div v-click>💬 Comunicação clara e transparente</div>
        </div>
      </div>
  </div>
</div>

---
class: flex justify-center items-center gap-20 px40 text-xl overflow-hidden
clicks: 1
---

<div text-4xl absolute :class="$clicks < 1 ? 'text-white' : 'translate-y--18 scale-40 text-white/30'" transition duration-500 ease-in-out>
  <span>✨ Liderança</span>
</div>

<div flex flex-col items-center relative>
  <div
    mt-15
    :class="[
      $clicks === 0 ? 'opacity-0' : '',
      $clicks === 1 ? 'opacity-100' : '',
      $clicks > 1 ? 'opacity-30 blur-sm' : ''
    ]"
    transition duration-500
  >

  <h1 flex items-center text="5xl!">
    <span>📑 Papéis da Liderança</span>
  </h1>

  </div>
</div>

---
glowSeed: 203
---

<div flex="row ~" w-full justify-between>
  <div>
    <div text-left w-full h-full flex="~ col justify-center">
      <div class="font-bold text-3xl mb-8">📑 Papéis da Liderança</div>
        <div class="space-y-2 list-decimal pl-4">
          <div v-click>🎯 Definir uma visão clara para a qualidade, alinhada à missão e valores da organização</div>
          <div v-click>🌟 Servir como exemplo de comprometimento e responsabilidade</div>
          <div v-click>🤝 Promover um ambiente de confiança, abertura e cooperação</div>
          <div v-click>🧠 Incentivar a capacitação e o desenvolvimento de competências</div>
          <div v-click>🥳 Reconhecer e valorizar conquistas relacionadas à qualidade</div>
        </div>
      </div>
  </div>
</div>

---
class: py-10
clicks: 8
glowSeed: 350
---

# Integração e Benefícios

<span>Cultura da Qualidade e Liderança</span>

<div mt-6 />

<div grid grid-cols-2 gap-6>
  <div
    v-click="1"
    border="2 solid blue-800" bg="blue-800/20"
    rounded-lg overflow-hidden
    transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'opacity-0 translate-y-20' : 'opacity-100 translate-y-0'"
  >
    <div bg="blue-800/40" px-4 py-2 flex items-center>
      <span font-bold>⚙️ Integração</span>
    </div>
    <div px-5 py-3>
      <div
        v-for="(step, idx) in [
          'Programas de treinamento e capacitação contínua',
          'Estabelecimento de indicadores de desempenho',
          'Monitoramento de resultados',
          'Promoção de um ambiente de inovação e aprendizagem',
          'Reconhecimento de boas práticas que contribuam para a qualidade'
        ]"
        :key="step"
        flex items-center gap-2 py-1
        :class="$clicks < 1 ? 'opacity-0' : 'opacity-100'"
        :style="{ transitionDelay: `${200 + idx * 100}ms`, transitionProperty: 'all', transitionDuration: '500ms' }"
      >
        🔵
        <span>{{step}}</span>
      </div>
    </div>
  </div>

  <div
    v-click="2"
    border="2 solid lime-800" bg="lime-800/20"
    rounded-lg overflow-hidden
    transition duration-500 ease-in-out
    :class="$clicks < 2 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div bg="lime-800/40" px-4 py-2 flex items-center>
      <span font-bold>🎊 Benefícios</span>
    </div>
    <div px-5 py-4 flex flex-col gap-2>
      <div
        v-for="(item, idx) in [
          'Maior satisfação e fidelização de clientes',
          'Redução de custos com retrabalho e desperdícios',
          'Aumento da produtividade e da eficiência dos processos',
          'Fortalecimento da imagem institucional',
          'Engajamento e motivação dos colaboradores'
        ]"
        :key="item"
        v-click="2 + idx"
        flex items-center gap-2
        :class="$clicks < (2 + idx) ? 'opacity-0 translate-x--10' : 'opacity-100 translate-x-0'"
        transition duration-300 ease-in-out
      >
        ✅
        <span>{{item}}</span>
      </div>
    </div>
  </div>
</div>

<style>
  h1 {
    font-weight: bold
  }
</style>

---
layout: intro
class: px-24
glowSeed: 205
---

<div flex items-center justify-center>
  <div
    v-click flex flex-col gap-2 items-center justify-center transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'translate-x--20' : 'translate-x-0'"
  >
    <div font-bold text-3xl text-center>
      📚
      <br>
      Gestão da Qualidade
    </div>
  </div>
  <div
    v-after pl-15 pr-15 transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'scale-80' : 'scale-100'"
  >
    <div i-carbon:close text-8xl />
  </div>
  <div
    v-after flex flex-col gap-2 items-center justify-center transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'translate-x-20' : 'translate-x-0'"
  >
    <div font-bold text-3xl text-center>
      🖥️
      <br>
      Desenvolvimento <br> de Software
    </div>
  </div>
</div>

---
class: py-10
glowSeed: 100
---

# Principais Objetivos

<span>Qualidade no Desenvolvimento de Software</span>

<div mt-4 />

<div flex flex-col gap-3>

<v-clicks>

<div border="2 solid blue-800/50" rounded-lg>
  <div flex items-center text-base bg="blue-800/30" px-3 py-2 text-blue-300>
    🤗&nbsp;<em>Satisfação do Cliente</em>
  </div>
  <div bg="blue-800/10" px-4 py-3>
    <div>
      <span>
        Entregar um software que atenda as expectativas do usuário final.
      </span>
    </div>
  </div>
</div>

<div border="2 solid teal-800/50" rounded-lg>
  <div flex items-center text-base bg="teal-800/30" px-3 py-2 text-teal-300>
    💸&nbsp;<em>Redução de Custos</em>
  </div>
  <div bg="teal-800/10" px-4 py-3>
    <div>
      <span>
        Identificar e corrigir bugs no início, evitando mais trabalho e custos futuramente.
      </span>
    </div>
  </div>
</div>

<div border="2 solid cyan-800/50" rounded-lg>
  <div flex items-center text-base bg="cyan-800/30" px-3 py-2 text-cyan-300>
     📈&nbsp;<em>Aumento da Confiabilidade</em>
  </div>
  <div bg="cyan-800/10" px-4 py-3>
    <div>
      <span>
        Garantir que o software opere de forma consistente e sem falhas, mesmo sob condições diversas.
      </span>
    </div>
  </div>
</div>

<div border="2 solid rose-800/50" rounded-lg>
  <div flex items-center text-base bg="rose-800/30" px-3 py-2 text-rose-300>
      ⚖️&nbsp;<em>Conformidade Regulatória</em>
  </div>
  <div bg="rose-800/10" px-4 py-3>
    <div>
      <span>
        Atender a normas e regulamentações específicas do setor.
      </span>
    </div>
  </div>
</div>

</v-clicks>

</div>

<style>
  h1 {
    font-weight: bold
  }
</style>

---
class: flex justify-center items-center gap-20 px-40 text-xl
clicks: 2
glowSeed: 203
---

<div
  absolute text-6xl
  :class="$clicks < 1 ? 'text-white' : 'translate-y--18 scale-40 text-white/30'"
  transition duration-500 ease-in-out
>
  <span transition="all 1000! ease-in-out" :class="$clicks > 1 ? 'opacity-0' : ''">🤔 Como atingir os objetivos?</span>
</div>

<div flex flex-col items-center>
  <v-clicks>
    <div mt-4 transition="all ease-in-out" flex flex-col flex-start
      duration-1500 :class="$slidev.nav.clicks > 1 ? 'translate-x-[-280px] translate-y-[-218px]' : ''">
      <h1 flex items-center font-bold transition="all duration-1000 ease-in-out" :class="$slidev.nav.clicks > 1 ? 'text-3xl! mb-3!' : 'text-5xl!'">
        <span>🏛️ Pilares Fundamentais</span>
      </h1>
       <span text-sm transition="all ease-in-out" :class="$slidev.nav.clicks > 1 ? 'opacity-50' : 'opacity-0'">Gestão da Qualidade no Desenvolvimento de Software</span>
    </div>
  </v-clicks>
</div>